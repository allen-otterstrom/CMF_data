---
layout: default
title: Historical Census of Manufactures Microdata
---

<style>
/* Remove box background only for index page */
body.page-index main,
body.page-index .wrapper,
body.page-index .container {
  max-width: 100% !important;
  background: none !important;
  box-shadow: none !important;
  padding: 0 !important;
}

/* Two-column layout */
.home-content {
  display: flex;
  align-items: flex-start;
  gap: 3rem;
  padding: 2rem;
  max-width: 1100px;
  margin: 0 auto;
}

/* Left text column */
.home-text {
  flex: 0 0 40%;
  max-width: 40%;
}

/* Right image column */
.home-images {
  flex: 0 0 60%;
  max-width: 60%;
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
  align-items: center; /* center horizontally */
}

/* Smaller image size and fade-in */
.home-images img {
  width: 70%;
  height: auto;
  object-fit: cover;
  opacity: 0;
  animation: fadeIn 1.2s ease-in forwards;
}

.home-images img:nth-child(2) {
  animation-delay: 0.4s;
}

/* Fade-in animation */
@keyframes fadeIn {
  to {
    opacity: 1;
  }
}

/* Buttons */
.button-container {
  display: flex;
  flex-direction: column;
  gap: 1.5rem; /* more vertical spacing */
  margin-top: 2rem;
}

.button-container a {
  display: block;
  padding: 1rem 1.5rem; /* taller buttons */
  background: #4a6fa5;
  color: white;
  text-decoration: none;
  text-align: center;
  border-radius: 6px;
  font-weight: bold;
  font-size: 1.1rem;
}

.button-container a:hover {
  background: #3c5a85;
}

/* Stack columns on smaller screens */
@media (max-width: 768px) {
  .home-content {
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
  .home-text,
  .home-images {
    max-width: 100%;
    flex: 1;
  }
  .home-images img {
    width: 80%;
  }
}
</style>

<div class="home-content">
  <div class="home-text">
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

  <div class="home-images">
    <img src="/CMF_data/assets/images/Belchers.jpg" alt="Historical photo 1">
    <img src="/CMF_data/assets/images/belchers_sheet.png" alt="Historical photo 2">
  </div>
</div>
