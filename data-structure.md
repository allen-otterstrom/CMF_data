---
layout: default
title: Data Structure
prev: /navigation
next: /coverage
hide_back: true
---



# Prepared CMF Data Structure

An observation in the prepared data is one establishment, and is uniquely identified by the variables file_name and firm_number, and schedule in the 1880 special schedules. The following table shows the number of variables and observations in each cleaned dataset:

<table border="1" cellspacing="0" cellpadding="5">
  <thead>
    <tr>
      <th>Dataset File Name</th>
      <th>Observations</th>
      <th>Variables</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>1850</td><td>124,873</td><td>329</td></tr>
    <tr><td>1860</td><td>121,168</td><td>443</td></tr>
    <tr><td>1870</td><td>203,353</td><td>753</td></tr>
    <tr><td>1880 General Schedule</td><td>170,811</td><td>102</td></tr>
    <tr><td>1880 SS1</td><td>1,981</td><td>204</td></tr>
    <tr><td>1880 SS2</td><td>677</td><td>271</td></tr>
    <tr><td>1880 SS3</td><td>2,161</td><td>85</td></tr>
    <tr><td>1880 SS4</td><td>3,083</td><td>121</td></tr>
    <tr><td>1880 SS5</td><td>24,240</td><td>120</td></tr>
    <tr><td>1880 SS6</td><td>4,856</td><td>82</td></tr>
    <tr><td>1880 SS7</td><td>23,251</td><td>136</td></tr>
    <tr><td>1880 SS8</td><td>3,508</td><td>96</td></tr>
    <tr><td>1880 SS9</td><td>4,632</td><td>104</td></tr>
    <tr><td>1880 SS10</td><td>128</td><td>70</td></tr>
    <tr><td>1880 SS11</td><td>2</td><td>82</td></tr>
    <tr><td>1880 SS12</td><td>1,381</td><td>97</td></tr>
  </tbody>
</table>

### Variable Availability

In the following variable availability tables, checks indicate that the variables are available, stars indicate that specified variables can be constructed from available data, and dashes mark variables that are unknowable.

#### Manuscript Variables

The following table lists out variables original to the manuscripts, and their availability by year. Since there are many manuscript variables unique to 1880, those are ommitted in this table.

<table border="1" cellspacing="0" cellpadding="5">
  <thead>
    <tr>
      <th>Variable</th>
      <th>1850</th>
      <th>1860</th>
      <th>1870</th>
      <th>1880</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Firm Name</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td></tr>
    <tr><td>Industry</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td></tr>
    <tr><td>Capital</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td></tr>
    <tr><td>Materials Quantity</td><td>✓</td><td>✓</td><td>✓</td><td>-</td></tr>
    <tr><td>Materials Kind</td><td>✓</td><td>✓</td><td>✓</td><td>-</td></tr>
    <tr><td>Materials Unit of Measure</td><td>✓</td><td>✓</td><td>✓</td><td>-</td></tr>
    <tr><td>Materials Value</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Number of Male Hands</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Number of Female Hands</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Number of Children Hands</td><td>-</td><td>-</td><td>✓</td><td>★</td></tr>
    <tr><td>Mean Male Wage</td><td>✓</td><td>✓</td><td>-</td><td>-</td></tr>
    <tr><td>Mean Female Wage</td><td>✓</td><td>✓</td><td>-</td><td>-</td></tr>
    <tr><td>Total Wages</td><td>★</td><td>★</td><td>✓</td><td>✓</td></tr>
    <tr><td>Months Active</td><td>-</td><td>-</td><td>✓</td><td>★</td></tr>
    <tr><td>Production Quantity</td><td>✓</td><td>✓</td><td>✓</td><td>-</td></tr>
    <tr><td>Production Kinds</td><td>✓</td><td>✓</td><td>✓</td><td>-</td></tr>
    <tr><td>Production Values</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Production Unit of Measure</td><td>✓</td><td>✓</td><td>✓</td><td>-</td></tr>
    <tr><td>Power Kind</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Machine Description</td><td>★</td><td>★</td><td>✓</td><td>★</td></tr>
    <tr><td>Number of Machines</td><td>-</td><td>-</td><td>✓</td><td>★</td></tr>
    <tr><td>Horsepower Measure</td><td>-</td><td>-</td><td>✓</td><td>★</td></tr>
    <tr><td>State</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td></tr>
    <tr><td>County</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td></tr>
    <tr><td>Township</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td></tr>
    <tr><td>Closest Post Office</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td></tr>
  </tbody>
</table>



#### Constructed Variables

The following table lists out the constructed variables available in the prepared data. An important note is that there are no 1880 general schedule constructed variables that are unique.

<table border="1" cellspacing="0" cellpadding="5">
  <thead>
    <tr>
      <th>Variable</th>
      <th>1850</th>
      <th>1860</th>
      <th>1870</th>
      <th>1880</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Broadest Industry Category</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td></tr>
    <tr><td>Cleaned Industry</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td></tr>
    <tr><td>Cleaned Material Kind</td><td>✓</td><td>✓</td><td>✓</td><td>-</td></tr>
    <tr><td>Cleaned Number of Children</td><td>-</td><td>-</td><td>✓</td><td>★</td></tr>
    <tr><td>Cleaned Product Kind</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Cleaned Total Wages</td><td>-</td><td>-</td><td>✓</td><td>★</td></tr>
    <tr><td>Detailed Industry Category</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td></tr>
    <tr><td>Establishment Number</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td></tr>
    <tr><td>FIPS Code</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td></tr>
    <tr><td>Granular Industry Category</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td></tr>
    <tr><td>Image File Name</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td></tr>
    <tr><td>Is Maker</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td></tr>
    <tr><td>Is Manufacturer</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Is Shop</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Is a Factory</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td></tr>
    <tr><td>Leontief Industry Category</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td></tr>
    <tr><td>Machine Category</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Machine Kind</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Machine Unit</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Material Kind Attribute</td><td>✓</td><td>✓</td><td>✓</td><td>-</td></tr>
    <tr><td>Material Units</td><td>✓</td><td>✓</td><td>✓</td><td>-</td></tr>
    <tr><td>Material Unsure</td><td>✓</td><td>✓</td><td>✓</td><td>-</td></tr>
    <tr><td>Material is Miscellaneous</td><td>✓</td><td>✓</td><td>✓</td><td>-</td></tr>
    <tr><td>Material is Note</td><td>✓</td><td>✓</td><td>✓</td><td>-</td></tr>
    <tr><td>Material is Service</td><td>✓</td><td>✓</td><td>✓</td><td>-</td></tr>
    <tr><td>Product Kind Attribute</td><td>✓</td><td>✓</td><td>✓</td><td>-</td></tr>
    <tr><td>Product is Miscellaneous</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Product is Note</td><td>✓</td><td>✓</td><td>✓</td><td>-</td></tr>
    <tr><td>Product is Service</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Product is Units</td><td>✓</td><td>✓</td><td>✓</td><td>-</td></tr>
    <tr><td>Product is Unsure</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Uses Hand Power</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Uses Horse Power</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Uses Steam Power</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Uses Water Power</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
    <tr><td>Uses Wind Power</td><td>✓</td><td>✓</td><td>✓</td><td>★</td></tr>
  </tbody>
</table>

#### Unique 1880 General Schedule variables

There are a number of unique variables in 1880 that have analogous variables or are constructable in other years.

<table border="1" cellspacing="0" cellpadding="5">
  <thead>
    <tr>
      <th>Variable</th>
      <th>1850</th>
      <th>1860</th>
      <th>1870</th>
      <th>1880</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Total Materials Value</td><td>★</td><td>★</td><td>★</td><td>✓</td></tr>
    <tr><td>Adult Male Workers</td><td>★</td><td>★</td><td>★</td><td>✓</td></tr>
    <tr><td>Adult Female Workers</td><td>★</td><td>★</td><td>★</td><td>✓</td></tr>
    <tr><td>Children Workers</td><td>-</td><td>-</td><td>★</td><td>✓</td></tr>
    <tr><td>Maximum Workers</td><td>★</td><td>★</td><td>★</td><td>✓</td></tr>
    <tr><td>Skilled Daily Wage</td><td>-</td><td>-</td><td>-</td><td>✓</td></tr>
    <tr><td>Unskilled Daily Wage</td><td>-</td><td>-</td><td>-</td><td>✓</td></tr>
    <tr><td>Hours May-November</td><td>-</td><td>-</td><td>-</td><td>✓</td></tr>
    <tr><td>Hours November-May</td><td>-</td><td>-</td><td>-</td><td>✓</td></tr>
    <tr><td>Months 1/2 Time</td><td>-</td><td>-</td><td>-</td><td>✓</td></tr>
    <tr><td>Months 2/3 Time</td><td>-</td><td>-</td><td>-</td><td>✓</td></tr>
    <tr><td>Months 3/4 Time</td><td>-</td><td>-</td><td>-</td><td>✓</td></tr>
    <tr><td>Months Full-Time</td><td>-</td><td>-</td><td>★</td><td>✓</td></tr>
    <tr><td>Months Idle</td><td>-</td><td>-</td><td>★</td><td>✓</td></tr>
    <tr><td>Total Production Values</td><td>★</td><td>★</td><td>★</td><td>✓</td></tr>
    <tr><td>Number of Steam Boilers</td><td>-</td><td>-</td><td>-</td><td>✓</td></tr>
    <tr><td>Number of Steam Engines</td><td>-</td><td>-</td><td>-</td><td>✓</td></tr>
    <tr><td>Horsepower from Steam</td><td>-</td><td>-</td><td>★</td><td>✓</td></tr>
    <tr><td>Height of River Fall</td><td>-</td><td>-</td><td>-</td><td>✓</td></tr>
    <tr><td>Which River Used</td><td>-</td><td>-</td><td>-</td><td>✓</td></tr>
    <tr><td>Number of Water Wheels</td><td>-</td><td>-</td><td>-</td><td>✓</td></tr>
    <tr><td>Breadth of Water Wheels</td><td>-</td><td>-</td><td>-</td><td>✓</td></tr>
    <tr><td>Horsepower of Water Wheels</td><td>-</td><td>-</td><td>-</td><td>✓</td></tr>
    <tr><td>Kind of Water Wheel</td><td>-</td><td>-</td><td>-</td><td>✓</td></tr>
    <tr><td>RPM of Water Wheels</td><td>-</td><td>-</td><td>-</td><td>✓</td></tr>
  </tbody>
</table>

#### 1880 Special Schedule Variables

There are 324 unique variables in the 1880 special schedules. The following file shows the availability for each of those across each schedule.

<div class="button-grid">
  <div class="button-item">
    <a class="button" href="https://pub-9228e653a45040598db0c86ec1d93b3c.r2.dev/website_materials/ss_variables.csv" download>Special Schedule Variables</a>
    <div class="description">Browse the Special Schedule Variables.</div>
  </div>
  </div>

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








