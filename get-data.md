---
layout: default
title: Get the Data
---

# Download the Data

Select a year you would like. You will then be able to download the data.

<label for="data-dropdown"><strong>Select Year / Schedule:</strong></label>
<select id="data-dropdown" onchange="updateSelectedFile(this.value)">
  <option value="">-- Choose a file --</option>
  <option value="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/all_data.zip">All Data</option>
  <option value="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/cmf_1850.csv">1850</option>
  <option value="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/cmf_1860.csv">1860</option>
  <option value="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/cmf_1870.csv">1870</option>
  <option value="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/cmf_1880_general_schedule.csv">1880 General Schedule</option>
  <option value="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/cmf_1880_ss1.csv">1880 Special Schedule 1</option>
  <option value="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/cmf_1880_ss2.csv">1880 Special Schedule 2</option>
  <option value="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/cmf_1880_ss3.csv">1880 Special Schedule 3</option>
  <option value="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/cmf_1880_ss4.csv">1880 Special Schedule 4</option>
  <option value="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/cmf_1880_ss5.csv">1880 Special Schedule 5</option>
  <option value="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/cmf_1880_ss6.csv">1880 Special Schedule 6</option>
  <option value="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/cmf_1880_ss7.csv">1880 Special Schedule 7</option>
  <option value="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/cmf_1880_ss8.csv">1880 Special Schedule 8</option>
  <option value="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/cmf_1880_ss9.csv">1880 Special Schedule 9</option>
  <option value="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/cmf_1880_ss10.csv">1880 Special Schedule 10</option>
  <option value="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/cmf_1880_ss11.csv">1880 Special Schedule 11</option>
  <option value="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/cmf_1880_ss12.csv">1880 Special Schedule 12</option>
</select>

<span id="selected-file" style="margin-left: 15px; font-weight: bold; font-size: 1.2em;">No file selected</span>
<br><br>
<a id="download-button" class="button" href="#" style="pointer-events: none; opacity: 0.5;">Download Selected File</a>

<br><br>
<a class="button" href="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/codebook.xlsx" download>Download Codebook</a>

# Example Images

<label for="images-dropdown"><strong>Select Image:</strong></label>
<select id="images-dropdown" onchange="openImageModal(this.value, this.options[this.selectedIndex].text)">
  <option value="">-- Choose an image --</option>
  <option value="/CMF_data/assets/images/1850_CMF.jpg">1850 Manuscript Image</option>
  <option value="/CMF_data/assets/images/1860_CMF.jpg">1860 Manuscript Image</option>
  <option value="/CMF_data/assets/images/1870_CMF.jpeg">1870 Manuscript Image</option>
  <option value="/CMF_data/assets/images/1880_gss_CMF.jpg">1880 General Schedule Image</option>
  <option value="/CMF_data/assets/images/1880_ss1_CMF_agimp.jpg">1880 Special Schedule 1 Image</option>
  <option value="/CMF_data/assets/images/1880_ss2_CMF_paper.jpg">1880 Special Schedule 2 Image</option>
  <option value="/CMF_data/assets/images/1880_ss34_CMF_bootsleather.jpg">1880 Special Schedules 3 & 4 Image</option>
  <option value="/CMF_data/assets/images/1880_ss56_CMF_lumberbrick.jpg">1880 Special Schedules 5 & 6 Image</option>
  <option value="/CMF_data/assets/images/1880_ss78_CMF_flourcheese.jpg">1880 Special Schedules 7 & 8 Image</option>
  <option value="/CMF_data/assets/images/1880_ss910_CMF_meatsalt.jpg">1880 Special Schedules 9 & 10 Image</option>
  <option value="/CMF_data/assets/images/1880_ss1112_CMF_coalquarry.jpg">1880 Special Schedule 11 & 12 Image</option>
</select>

# Additional Links

<div class="button-grid">
  <a class="button" href="{{ '/county_ind_tab' | relative_url }}">County-Industry Tabulations</a>
  <a class="button" href="{{ '/raw_data_code' | relative_url }}">Raw Data and Code</a>
  <a class="button" href="{{ '/search' | relative_url }}">Search CMF Images</a>
  <a class="button" href="{{ '/add-on' | relative_url }}" class="button">Contribute</a>
</div>

<script>
let selectedFile = "";
let selectedFileLabel = "";

// Data dropdown
function updateSelectedFile(fileUrl) {
  const dropdown = document.getElementById('data-dropdown');
  const selectedOption = dropdown.options[dropdown.selectedIndex];
  selectedFile = selectedOption.value;
  selectedFileLabel = selectedOption.text;
  
  const downloadButton = document.getElementById('download-button');
  const fileDisplay = document.getElementById('selected-file');
  
  if (selectedFile) {
    fileDisplay.textContent = selectedFileLabel;
    downloadButton.href = selectedFile;
    downloadButton.download = selectedFile.split('/').pop();
    downloadButton.style.pointerEvents = 'auto';
    downloadButton.style.opacity = '1';
  } else {
    fileDisplay.textContent = "No file selected";
    downloadButton.href = '#';
    downloadButton.removeAttribute('download');
    downloadButton.style.pointerEvents = 'none';
    downloadButton.style.opacity = '0.5';
  }
}


// Image modal
function openImageModal(src, label) {
  if (!src) return;
  const modal = document.getElementById("imageModal");
  const modalImg = document.getElementById("modalImg");
  const caption = document.getElementById("caption");
  modal.style.display = "flex";
  modalImg.src = src;
  caption.textContent = label || src.split('/').pop();
}

function closeImageModal() {
  document.getElementById("imageModal").style.display = "none";
}

// Close modal on backdrop click
document.getElementById("imageModal").addEventListener("click", function(e) {
  if (e.target === this) closeImageModal();
});

// Close modal on ESC key
document.addEventListener("keydown", function(e) {
  const modal = document.getElementById("imageModal");
  if (modal.style.display === "flex" && e.key === "Escape") {
    closeImageModal();
  }
});

// Preload images
window.addEventListener("load", function() {
  const dropdown = document.getElementById("images-dropdown");
  for (let i = 0; i < dropdown.options.length; i++) {
    if (dropdown.options[i].value) new Image().src = dropdown.options[i].value;
  }
});
</script>

<!-- Modal -->
<div id="imageModal" class="modal">
  <span class="close" onclick="closeImageModal()">&times;</span>
  <img class="modal-content" id="modalImg" alt="">
  <div id="caption"></div>
</div>

<style>
.modal {
  display: none;
  position: fixed;
  z-index: 1000;
  left: 0; top: 0;
  width: 100%; height: 100%;
  background-color: rgba(0,0,0,0.9);
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.modal-content {
  max-width: 90%;
  max-height: 80vh;
  border-radius: 8px;
}

.close {
  position: absolute;
  top: 15px; right: 35px;
  color: #fff;
  font-size: 40px;
  font-weight: bold;
  cursor: pointer;
}

#caption {
  margin-top: 10px;
  color: #fff;
  font-size: 1.1em;
  text-align: center;
}
</style>
