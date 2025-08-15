---
layout: default
title: Historical Census of Manufactures Microdata
---

<style>
/* Remove content box only for this page */
body.page-index main {
  background: none;
  box-shadow: none;
  padding: 0;
  max-width: 100%;
}

/* Hero section with big images and text */
.hero-container {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 2rem;
  margin-bottom: 2rem;
}

.hero-images {
  flex: 2;
  display: flex;
  gap: 1rem;
}

.hero-images img {
  width: 100%;
  height: auto;
  border-radius: 6px;
  object-fit: cover;
}

.hero-text {
  flex: 1;
  min-width: 250px;
}

/* Vertical buttons */
.button-container {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  margin-top: 1.5rem;
}

.button-container a {
  display: inline-block;
  padding: 0.8rem 1.2rem;
  background: #4a6fa5;
  color: white;
  text-decoration: none;
  text-align: center;
  border-radius: 5px;
  font-weight: bold;
}

.button-container a:hover {
  background: #3c5a85;
}
</style>

<div class="hero-container">
  <div class="hero-images">
    <img src="/CMF_data/assets/images/Belchers.jpg" alt="Historical photo 1">
    <img src="/CMF_data/assets/images/belchers_sheet.png" alt="Historical photo 2">
  </div>
  <div class="hero-text">
    <h3>Welcome to the Census of Manufactures Historical Data Portal</h3>
    <p>
      This site provides access to newly digitized, detailed manufacturing data from the U.S. Census of Manufactures, spanning the mid-19th century. 
      Here you’ll find cleaned and structured datasets, documentation of coverage and methodology, and tools for exploring county- and industry-level patterns over time.
    </p>
    <div class="button-container">
      <a href="get-data.html">Get the data</a>
      <a href="about.html">About the data</a>
      <a href="explore.html">Explore the data</a>
    </div>
  </div>
</div>
