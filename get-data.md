---
layout: default
title: Get the Data
---

# Download the Data

<label for="data-dropdown"><strong>Select Year / Schedule:</strong></label>
<select id="data-dropdown" onchange="downloadFile(this.value)">
  <option value="">-- Choose a file --</option>
  <option value="1850.csv">1850</option>
  <option value="1860.csv">1860</option>
  <option value="1870.csv">1870</option>
  <option value="1880_general.csv">1880 General Schedule</option>
  <option value="1880_special1.csv">1880 Special Schedule 1</option>
  <option value="1880_special2.csv">1880 Special Schedule 2</option>
  <option value="1880_special3.csv">1880 Special Schedule 3</option>
  <option value="1880_special4.csv">1880 Special Schedule 4</option>
  <option value="1880_special5.csv">1880 Special Schedule 5</option>
  <option value="1880_special6.csv">1880 Special Schedule 6</option>
  <option value="1880_special7.csv">1880 Special Schedule 7</option>
  <option value="1880_special8.csv">1880 Special Schedule 8</option>
  <option value="1880_special9.csv">1880 Special Schedule 9</option>
  <option value="1880_special10.csv">1880 Special Schedule 10</option>
  <option value="1880_special11.csv">1880 Special Schedule 11</option>
  <option value="1880_special12.csv">1880 Special Schedule 12</option>
</select>

<!-- Codebook button right under the dropdown -->
<br><br>
<a class="button" href="codebook.pdf" download>Download Codebook</a>

# Example Images

<label for="images-dropdown"><strong>Select Image:</strong></label>
<select id="images-dropdown" onchange="downloadFile(this.value)">
  <option value="">-- Choose an image --</option>
  <option value="images/photo1.jpg">1850 Manuscript Image</option>
  <option value="images/photo2.jpg">1860 Manuscript Image</option>
  <option value="images/photo3.jpg">1870 Manuscript Image</option>
  <option value="images/photo4.jpg">1880 General Schedule Image</option>
  <option value="images/photo5.jpg">1880 Special Schedule 1 Image</option>
  <option value="images/photo6.jpg">1880 Special Schedule 2 Image</option>
  <option value="images/photo7.jpg">1880 Special Schedule 3 Image</option>
  <option value="images/photo8.jpg">1880 Special Schedule 4 Image</option>
  <option value="images/photo9.jpg">1880 Special Schedule 5 Image</option>
  <option value="images/photo10.jpg">1880 Special Schedule 6 Image</option>
  <option value="images/photo11.jpg">1880 Special Schedule 7 Image</option>
  <option value="images/photo12.jpg">1880 Special Schedule 8 Image</option>
  <option value="images/photo13.jpg">1880 Special Schedule 9 Image</option>
  <option value="images/photo14.jpg">1880 Special Schedule 10 Image</option>
  <option value="images/photo15.jpg">1880 Special Schedule 11 Image</option>
  <option value="images/photo16.jpg">1880 Special Schedule 12 Image</option>
</select>

# Additional Links

<div class="button-grid">
  <a class="button" href="additional-data.html">Additional Data</a>
  <a class="button" href="navigation.html">Navigation</a>
  <a class="button" href="data-structure.html">Data Structure</a>
</div>

<script>
function downloadFile(fileUrl) {
  if (!fileUrl) return;
  const link = document.createElement('a');
  link.href = fileUrl;
  link.download = fileUrl.split('/').pop(); // suggested filename
  document.body.appendChild(link);
  link.click();
  document.body.removeChild(link);
}
</script>
