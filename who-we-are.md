---
layout: default
title: Who We Are
---

<style>
  /* Container for the PI cards */
.pi-container {
  display: flex;
  flex-wrap: wrap;
  gap: 30px;
  justify-content: space-between; /* spreads them out */
}

.pi-card {
  flex: 1;                 /* each takes equal width */
  min-width: 200px;        /* prevents shrinking too much */
  text-align: center;
}


  /* Portraits */
  .pi-card img {
    width: 150px;
    height: 200px;
    object-fit: cover;
    display: block;
    margin: 0 auto;
    border: none;
  }

  /* Names */
  .pi-card p {
    margin: 10px 0 5px 0;
    text-align: center;
  }

  /* Links */
  .pi-card a {
    display: inline-block;
    text-align: center;
    text-decoration: none;
    color: black;
    font-weight: bold;
    text-decoration: none; /* removes underline */
  }

  .pi-card a:hover {
    text-decoration: underline;
  }

  /* Multi-column lists */
  .multi-col {
    columns: 2;          /* number of columns */
    -webkit-columns: 2;  /* Chrome/Safari */
    -moz-columns: 2;     /* Firefox */
  }
  .multi-col {
    columns: 2;          
    -webkit-columns: 2;  
    -moz-columns: 2;     
  }

  /* More columns for RA section */
  .multi-col-4 {
    columns: 4;          
    -webkit-columns: 4;  
    -moz-columns: 4;     
    list-style-position: inside; /* keep bullets aligned */
    padding-left: 20px;  /* spacing for bullets */
  }

  .multi-col-2 {
    columns: 2;          
    -webkit-columns: 2;  
    -moz-columns: 2;     
    list-style-position: inside; /* keep bullets aligned */
    padding-left: 20px;  /* spacing for bullets */
  }

.pi-card a:hover {
  text-decoration: underline; /* optional: underline on hover */
}
  /* Mobile responsive - change 4 columns to 2 on small screens */
@media (max-width: 768px) {
  .multi-col-4 {
    columns: 2;          
    -webkit-columns: 2;  
    -moz-columns: 2;     
  }
}

</style>



# Principal Investigators
<div class="pi-container">
  <div class="pi-card">
    <img src="{{ '/assets/images/richard_hornbeck_portrait.jpg' | relative_url }}" alt="Richard Hornbeck">
    <a href="https://voices.uchicago.edu/richardhornbeck/" target="_blank">Richard Hornbeck</a>
    <p>Professor of Economics</p>
    <p>The University of Chicago Booth School of Business</p>
  </div>

  <div class="pi-card">
    <img src="{{ '/assets/images/anders_humlum_portrait.webp' | relative_url }}" alt="Anders Humlum">
    <a href="https://www.andershumlum.com/" target="_blank">Anders Humlum</a>
    <p>Assistant Professor of Economics</p>
    <p>The University of Chicago Booth School of Business</p>
  </div>

  <div class="pi-card">
    <img src="{{ '/assets/images/martin_rotemberg_portrait.jpeg' | relative_url }}" alt="Martin Rotemberg">
    <a href="https://sites.google.com/view/mrotemberg/" target="_blank">Martin Rotemberg</a>
    <p>Associate Professor of Economics</p>
    <p>New York University</p>
  </div>
</div>

# Collaborators
<div class="pi-container">
  <div class="pi-card">
    <img src="{{ '/assets/images/shanon_portrait.jpeg' | relative_url }}" alt="Shanon Hsuan-Ming Hsu">
    <a href="https://shanonhmhsu.com/" target="_blank">Shanon Hsuan-Ming Hsu</a>
    <p>Visiting Scholar in Economics</p>
    <p>Harvard University</p>
  </div>

  <div class="pi-container">
  <div class="pi-card">
    <img src="{{ '/assets/images/Ruveyda_portrait.jpg' | relative_url }}" alt="Ruveyda Nur Gozen">
    <a href="https://sites.google.com/view/ruveydagozen" target="_blank">Ruveyda Nur Gozen</a>
    <p>Assistant Professor of Economics</p>
    <p>Cardiff Business School</p>
  </div>
</div>

# Current Full-Time and Graduate Research Assistants
- Allen Otterstrom (Research Professional, Booth School of Business, University of Chicago)
- Benjamin Lualdi (Economics PhD Student, Booth School of Business, University of Chicago)

# Former Full-Time and Graduate Research Assistants
<ul class="multi-col-2">
<li>Samuel Abers</li>
<li>Jiaxuan Lu</li>
<li>Bo-Yu Chen</li> 
<li>Vivian Li</li>  
<li>Terence Chau</li>  
<li>Ali Doxey</li>  
<li>Natalie Yang</li>  
<li>Will Cockriel</li>  
<li>Julius Luettge</li>  
<li>Andrea Cerrato</li>  
</ul>
# Part-time Student Research Assistants
<ul class="multi-col-4">
  <li>Paul Wang</li>
  <li>Tony Li</li>
  <li>Uday Malik</li>
  <li>Howard Li</li>
  <li>Eric Zhu</li>
  <li>Elliot Lin</li>
  <li>Alexandra Zhou</li>
  <li>Chenhao Yu</li>
  <li>Cynthia Ji</li>
  <li>David Kirchenbauer</li>
  <li>Ding Ding</li>
  <li>Eugenia Huang</li>
  <li>Evelyn Nie</li>
  <li>Jizhou Wang</li>
  <li>Kuitai Wang</li>
  <li>Leann Lee</li>
  <li>Risa Takashima</li>
  <li>Adrianna Nehme</li>
  <li>Annie Liu</li>
  <li>Astrid Ouyang</li>
  <li>Cheresa Turek</li>
  <li>Clara Ee</li>
  <li>Jihee You</li>
  <li>Joyce Wang</li>
  <li>Kathy Yao</li>
  <li>Mona Khairy</li>
  <li>Nathan Unah</li>
  <li>Neel Lahiri</li>
  <li>Polly Ren</li>
  <li>Scarlett Li</li>
  <li>Tony Brooks</li>
  <li>Yuerong Zhuang</li>
</ul>

# Additional Support
We thank the team at Digital Divide Data (DDD) for their tremendous effort with data entry.

# Acknowledgments
We gratefully acknowledge financial support from the following institutions:
- Becker Friedman Institute
- National Science Foundation
- Initiative on Global Markets at the University of Chicago Booth School of Business
- Neubauer Family Faculty Fellowship
- NBER Innovation Policy grant program
