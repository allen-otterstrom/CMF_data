---
layout: default
title: Get the Data
---

# Download the Data

<label for="data-dropdown"><strong>Select Year / Schedule:</strong></label>
<select id="data-dropdown" onchange="updateSelectedFile(this.value)">
  <option value="">-- Choose a file --</option>
  <option value="all_appended.csv">All Data</option>
  <option value="https://pub-cefce323449a4829a6786170686f724a.r2.dev/website_materials/cmf_1850.csv">1850</option>
  <option value="https://pub-cefce323449a4829a6786170686f724a.r2.dev/website_materials/cmf_1860.csv">1860</option>
  <option value="https://pub-cefce323449a4829a6786170686f724a.r2.dev/website_materials/cmf_1870.csv">1870</option>
  <option value="https://pub-cefce323449a4829a6786170686f724a.r2.dev/website_materials/cmf_1880_general_schedule.csv">1880 General Schedule</option>
  <option value="https://pub-cefce323449a4829a6786170686f724a.r2.dev/website_materials/cmf_1880_ss1.csv">1880 Special Schedule 1</option>
  <option value="https://pub-cefce323449a4829a6786170686f724a.r2.dev/website_materials/cmf_1880_ss2.csv">1880 Special Schedule 2</option>
  <option value="https://pub-cefce323449a4829a6786170686f724a.r2.dev/website_materials/cmf_1880_ss3.csv">1880 Special Schedule 3</option>
  <option value="https://pub-cefce323449a4829a6786170686f724a.r2.dev/website_materials/cmf_1880_ss4.csv">1880 Special Schedule 4</option>
  <option value="https://pub-cefce323449a4829a6786170686f724a.r2.dev/website_materials/cmf_1880_ss5.csv">1880 Special Schedule 5</option>
  <option value="https://pub-cefce323449a4829a6786170686f724a.r2.dev/website_materials/cmf_1880_ss6.csv">1880 Special Schedule 6</option>
  <option value="https://pub-cefce323449a4829a6786170686f724a.r2.dev/website_materials/cmf_1880_ss7.csv">1880 Special Schedule 7</option>
  <option value="https://pub-cefce323449a4829a6786170686f724a.r2.dev/website_materials/cmf_1880_ss8.csv">1880 Special Schedule 8</option>
  <option value="https://pub-cefce323449a4829a6786170686f724a.r2.dev/website_materials/cmf_1880_ss9.csv">1880 Special Schedule 9</option>
  <option value="https://pub-cefce323449a4829a6786170686f724a.r2.dev/website_materials/cmf_1880_ss10.csv">1880 Special Schedule 10</option>
  <option value="https://pub-cefce323449a4829a6786170686f724a.r2.dev/website_materials/cmf_1880_ss11.csv">1880 Special Schedule 11</option>
  <option value="https://pub-cefce323449a4829a6786170686f724a.r2.dev/website_materials/cmf_1880_ss12.csv">1880 Special Schedule 12</option>
</select>

<!-- Selected file name and download button -->
<span id="selected-file" style="margin-left: 15px; font-weight: bold; font-size: 1.2em;">No file selected</span>
<br><br>
<a id="download-button" class="button" href="#" onclick="downloadSelectedFile()">Download Selected File</a>

<br><br>
<a class="button" href="codebook.pdf" download>Download Codebook</a>

# Example Images

<label for="images-dropdown"><strong>Select Image:</strong></label>
<select id="images-dropdown" onchange="openImageModal(this.value)">
  <option value="">-- Choose an image --</option>
  <option value="/CMF_data/assets/images/1850_CMF.jpg">1850 Manuscript Image</option>
  <option value="/CMF_data/assets/images/1860_CMF.jpg">1860 Manuscript Image</option>
  <option value="/CMF_data/assets/images/1870_CMF.jpg">1870 Manuscript Image</option>
  <option value="/CMF_data/assets/images/1880_gss_CMF.jpg">1880 General Schedule Image</option>
  <option value="/CMF_data/assets/images/1880_ss1_CMF_agimp.jpg">1880 Special Schedule 1 Image</option>
  <option value="/CMF_data/assets/images/1880_ss2_CMF_paper.jpg">1880 Special Schedule 2 Image</option>
  <option value="/CMF_data/assets/images/1880_ss34_CMF_bootsleather.jpg">1880 Special Schedules 3 & 4 Image</option>
  <option value="/CMF_data/assets/images/1880_ss56_CMF_lumberbrick.jpg">1880 Special Schedules 5 & 6 Image</option>
  <option value="/CMF_data/assets/images/1880_ss78_CMF_flourcheese.jpg">1880 Special Schedules 7 & 8 Image</option>
  <option value="/CMF_data/assets/images/1880_ss910_CMF_meatsalt.jpg">1880 Special Schedules 9 & 10 Image</option>
  <option value="/CMF_data/assets/images/1880_ss1112_CMF_coalquarry.jpg">1880 Special Schedulea 11 & 12 Image</option>
</select>


# Additional Links

<div class="button-grid">
  <a class="button" href="additional-data.html">Additional Data</a>
  <a class="button" href="navigation.html">CMF Manuscript Navigation</a>
  <a class="button" href="data-structure.html">CMF Data Structure</a>
  <a class="button" href="search.html">CMF Images</a>
</div>

<script>
let selectedFile = "";
let selectedImage = "";

function updateSelectedFile(fileUrl) {
  const dropdown = document.getElementById('data-dropdown');
  selectedFile = dropdown.value;
  document.getElementById('selected-file').textContent = selectedFile || "No file selected";
}

function updateSelectedImage(fileUrl) {
  const dropdown = document.getElementById('images-dropdown');
  selectedImage = dropdown.value;
  document.getElementById('selected-image').textContent = selectedImage || "No image selected";
}

function downloadSelectedFile() {
  if (!selectedFile) {
    alert("Please select a file to download.");
    return;
  }
  const link = document.createElement('a');
  link.href = selectedFile;
  link.download = selectedFile.split('/').pop();
  document.body.appendChild(link);
  link.click();
  document.body.removeChild(link);
}

function downloadSelectedImage() {
  if (!selectedImage) {
    alert("Please select an image to download.");
    return;
  }
  const link = document.createElement('a');
  link.href = selectedImage;
  link.download = selectedImage.split('/').pop();
  document.body.appendChild(link);
  link.click();
  document.body.removeChild(link);
}
</script>

<script>
let selectedFile = "";

function updateSelectedFile(fileUrl) {
  const dropdown = document.getElementById('data-dropdown');
  selectedFile = dropdown.value;
  document.getElementById('selected-file').textContent = selectedFile || "No file selected";
}

function downloadSelectedFile() {
  if (!selectedFile) {
    alert("Please select a file to download.");
    return;
  }
  const link = document.createElement('a');
  link.href = selectedFile;
  link.download = selectedFile.split('/').pop();
  document.body.appendChild(link);
  link.click();
  document.body.removeChild(link);
}
</script>

<!-- The Modal -->
<div id="imageModal" class="modal">
  <span class="close" onclick="closeImageModal()">&times;</span>
  <img class="modal-content" id="modalImg">
  <div id="caption"></div>
</div>

<style>
/* Modal styles */
.modal {
  display: none; 
  position: fixed; 
  z-index: 1000; 
  padding-top: 60px; 
  left: 0;
  top: 0;
  width: 100%; 
  height: 100%; 
  overflow: auto; 
  background-color: rgba(0,0,0,0.8);
}

.modal-content {
  margin: auto;
  display: block;
  max-width: 90%;
  max-height: 80%;
  border-radius: 8px;
}

.close {
  position: absolute;
  top: 15px;
  right: 35px;
  color: white;
  font-size: 40px;
  font-weight: bold;
  cursor: pointer;
}

#caption {
  margin: auto;
  display: block;
  text-align: center;
  color: white;
  padding: 10px 0;
}
</style>

<script>
function openImageModal(src) {
  if (!src) return;
  var modal = document.getElementById("imageModal");
  var modalImg = document.getElementById("modalImg");
  var caption = document.getElementById("caption");
  modal.style.display = "block";
  modalImg.src = src;
  caption.textContent = src.split('/').pop();
}

function closeImageModal() {
  var modal = document.getElementById("imageModal");
  modal.style.display = "none";
}
</script>
