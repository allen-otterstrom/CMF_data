---
layout: default 
title: Historical Census of Manufactures Microdata 
--- 
<h1>
  Welcome to the Census of Manufactures Historical Data Portal 
</h1>
<div class="homepage-text">
  This site provides access to newly digitized, detailed manufacturing data from the U.S. Census of Manufactures, spanning the mid-19th century.
  Here you'll find cleaned and structured datasets, documentation of coverage and methodology, and tools for exploring county- and industry-level patterns over time. 
</div>
<div class="image-container"> 
  <img src="{{ '/assets/images/Belchers.jpg' | relative_url }}" alt="Historical photo 1"> 
  <img src="{{ '/assets/images/belchers_sheet.png' | relative_url }}" alt="Historical photo 2"> 
</div>
<div class="button-container"> 
  <a href="{{ '/get-data' | relative_url }}">Get the data</a> 
  <a href="{{ '/about' | relative_url }}">About the data</a> 
  <a href="{{ '/explore' | relative_url }}">Explore the data</a> 
</div>
<style>
  body.page-index {
    background-color: #fff;  /* same as header */
    color: #222;             /* optional: text color */
}
  /* Make the main header bigger on the homepage */
body.page-index h1 {
    font-size: 3em;   /* increase size as desired */
    font-family: 'Bodoni Moda', serif; /* optional: match your header style */
    /*font-family: 'Arial';*/
    font-weight: 400;  /* optional: lighter weight */
    margin-bottom: 1em; /* spacing below header */
}
@media (max-width: 768px) {
  body.page-index h1 {
    font-size: 1.5em;
    margin: 1em .75rem 0 .75rem;
  }
}
</style>
