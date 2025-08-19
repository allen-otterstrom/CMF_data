---
layout: default
title: Image Search
---

# Search Census Manuscript Images

Type part of a filename (e.g., county, state, or year) to find an image.  
The list will appear below with links to the full-size scans.

<input type="text" id="searchBox" placeholder="Search for an image..." style="width: 100%; padding: 0.6em; font-size: 1em; margin-top: 1em;">

<div id="results" style="margin-top: 1.5em;"></div>

<script>
let images = null; // will hold the JSON once loaded

async function loadImages() {
  if (!images) {
    const response = await fetch("assets/image_links.json");  // adjust path if needed
    images = await response.json();
  }
}

document.getElementById("searchBox").addEventListener("input", async function(e) {
  const query = e.target.value.toLowerCase().trim();
  const resultsDiv = document.getElementById("results");
  resultsDiv.innerHTML = "";

  if (query.length < 2) return; 

  await loadImages(); // fetch JSON once

  const matches = images
    .filter(img => img.filename.toLowerCase().includes(query))
    .slice(0, 50); // limit results

  if (matches.length === 0) {
    resultsDiv.textContent = "No matches found.";
    return;
  }

  matches.forEach(img => {
    const link = document.createElement("a");
    link.href = img.url;
    link.textContent = img.filename;
    link.target = "_blank";
    link.style.display = "block";
    link.style.marginBottom = "0.5em";
    resultsDiv.appendChild(link);
  });
});
</script>
