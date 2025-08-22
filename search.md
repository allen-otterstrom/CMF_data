---
layout: default
title: Image Search
---

# Search Census Manuscript Images

Type part of a filename, state, year, or industry (e.g., `PA steel`) to find an image.  
The list will appear below with links to the full-size scans.

<input type="text" id="searchBox" placeholder="Search for an image..." style="width: 100%; padding: 0.6em; font-size: 1em; margin-top: 1em;">

<div id="results" style="margin-top: 1.5em;"></div>

<script>
let images = null; // will hold the JSON once loaded
const jsonFiles = [
  "assets/image_links_1850.json",
  "assets/image_links_1860.json",
  "assets/image_links_1870.json",
  "assets/image_links_1880.json"
];

async function loadImages() {
  if (!images) {
    images = [];
    // Load each JSON file and append results
    for (const file of jsonFiles) {
      const response = await fetch(file);
      const data = await response.json();
      images = images.concat(data);
    }
  }
}

document.getElementById("searchBox").addEventListener("input", async function(e) {
  const query = e.target.value.toLowerCase().trim();
  const resultsDiv = document.getElementById("results");
  resultsDiv.innerHTML = "";

  if (query.length < 2) return; 

  await loadImages(); // fetch JSONs once

  // Split into individual words so "PA steel" works
  const terms = query.split(/\s+/);

  const matches = images.filter(img => {
    const haystack = [
      img.filename,
      img.year,
      img.state,
      img.state_long,
      img.industries
    ].join(" ").toLowerCase();

    return terms.every(term => haystack.includes(term));
  }).slice(0, 50);

  if (matches.length === 0) {
    resultsDiv.textContent = "No matches found.";
    return;
  }

  matches.forEach(img => {
    const link = document.createElement("a");
    link.href = img.url;
    link.textContent = `${img.filename} (${img.state_long}, ${img.year}) - ${img.industries}`;
    link.target = "_blank";
    link.style.display = "block";
    link.style.marginBottom = "0.5em";
    resultsDiv.appendChild(link);
  });
});
</script>
