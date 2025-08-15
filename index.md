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
  align-items: center; /* vertical center */
  justify-content: center; /* horizontal center of both halves */
  padding: 2rem;
  height: calc(100vh - 120px); /* adjust for banner height */
}

/* Columns */
.home-text, .home-images {
  flex: 0 0 50%;
  max-width: 50%;
  display: flex;
  justify-content: center; /* center block in column */
  align-items: center;
}

/* Text block */
.text-block {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly; /* evenly space heading, paragraph, buttons */
  align-items: center;
  text-align: center;
  width: 80%; /* fixed width inside column */
  height: 70%; /* gives vertical spacing room */
}

/* Heading + paragraph */
.text-block h3 {
  margin: 0;
  font-size: 2rem;
}
.text-block p {
  font-size: 1.1rem;
  line-height: 1.5;
  margin: 0;
}

/* Button container */
.button-container {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
  width: 100%;
}

/* Bigger buttons */
.button-container a {
  display: block;
  padding: 1.5rem; /* much taller */
  background: #4a6fa5;
  color: white;
  text-decoration: none;
  text-align: center;
  border-radius: 8px;
  font-weight: bold;
  font-size: 1.3rem; /* larger text */
}

.button-container a:hover {
  background: #3c5a85;
}

/* Images */
.home-images {
  flex-direction: column;
  gap: 1.5rem;
}

.home-images img {
  width: 60%;
  height: auto;
  opacity: 0;
  animation: fadeIn 1.2s ease-in forwards;
}
.home-images img:nth-child(2) {
  animation-delay: 0.4s;
}

@keyframes fadeIn {
  to {
    opacity: 1;
  }
}

/* Responsive */
@media (max-width: 768px) {
  .home-content {
    flex-direction: column;
    height: auto;
  }
  .home-text,
  .home-images {
    max-width: 100%;
    flex: 1;
  }
  .text-block {
    width: 90%;
    height: auto;
  }
  .home-images img {
    width: 80%;
  }
}
</style>

<div class="home-content">
  <div class="home-text">
    <div class="text-block">
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

  <div class="home-images">
    <img src="/CMF_data/assets/images/Belchers.jpg" alt="Historical photo 1">
    <img src="/CMF_data/assets/images/belchers_sheet.png" alt="Historical photo 2">
  </div>
</div>
