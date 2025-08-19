---
layout: default
title: Additional Data
---

# Additional Data

<div class="button-grid">
  <div class="button-item">
    <a class="button" href="/CMF_data/raw_data.zip" download>Raw Data</a>
    <div class="description">Download the raw transcriptions of the CMF manuscripts.</div>
  </div>
  <div class="button-item">
    <a class="button" href="/CMF_data/cleaning_files.zip" download>Cleaning Files</a>
    <div class="description">Scripts, code and crosswalks used to clean the data.</div>
  </div>
  <div class="button-item">
    <a class="button" href="/CMF_data/county_ind_data.zip" download>County-Ind Data</a>
    <div class="description">Transcribed and cleaned county-industry level data originally published by the Census Bureau.</div>
  </div>
</div>

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

.button {
  padding: 0.6em 1em;
  background-color: #007BFF;
  color: white;
  text-decoration: none;
  border-radius: 4px;
}

.button:hover {
  background-color: #0056b3;
}

.description {
  font-size: 0.95em;
  color: #333;
}
