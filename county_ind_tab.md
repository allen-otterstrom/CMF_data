---
layout: default
title: County Industry Tabulations
---

# County-Industry Tabulations

We additionally digitized county- and industry-level manufacturing data for 1860, 1870, and 1880 from the original published tabulations of the Census of Manufactures. In 1860, the Census of Manufactures also included data for enterprises outside of manufacturing—specifically fisheries and mining—which are incorporated in our dataset.

The county–industry tabulations list many industries in each decade, with some variation across years, which we concorded to enable consistent analysis. We standardized industry names within each county to match those from the national industry tabulations: 639 industries in 1860, 412 in 1870, and 331 in 1880 (over 1,100 distinct names in total). We then aggregated these into 193 cross-decade categories, and further into 31 broad industry groups.

Beginning in 1870, the county–industry data exclude certain “neighborhood industries,” such as blacksmithing, and other small industries with total revenues below $10,000. To account for these, we added an “other” industry category—representing less than 1% of total revenue—that captures named but otherwise uncategorized minor industries.


<div class="button-grid">
  <div class="button-item">
    <a class="button" href="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/ci_data.zip" download>County-Industry</a>
    <div class="description">Download the county-industry tabulations for all years</div>

<style>
.button-grid {
  display: flex;
  flex-direction: column;
  gap: 1em; /* space between rows */
}

.button-item {
  display: flex;
  align-items: center;
  gap: 1em; /* space between button and description */
}

.description {
  font-size: 0.95em;
  color: #333;
}
</style>
