---
layout: default
title: Coverage
prev: /data-structure
next: /faqs
hide_back: true
---

# Establishment Level Data Coverage

The Census of Manufacturers data from 1850 to 1880 is rich and detailed, but it does not cover all manufacturing establishments in the United States. There are two main reasons for this:

- **500 dollar minimum threshold**: Only establishments producing at least $500 worth of goods were included, leaving out smaller manufacturers. These smaller businesses were included in the Agriculture Census as home manufacturing, so in principle we know the number of businesses, but they are not included in these Data.

- **Missing manuscripts**: Many original records have been lost over the past 140+ years. This is especially significant for 1880:
  
  - Part of the **general schedule** is missing.
  
  - All **special agent schedules** are entirely lost.

The second reason is much more important than the first, but together these factors mean the datasets are not fully comprehensive, but they still capture a large and likely representative share of significant manufacturers during the period.

## Comparison to County and County-Industry Data

At the time each census was completed, all manuscripts were gathered by the Census Bureau and tabulated at both the county level and the county-industry level. Comparing the data to the tabulations allows us to get a bit of an idea of the broad coverage of the data:
<table border="1" cellspacing="0" cellpadding="5">
  <thead>
    <tr>
      <th>State</th>
      <th>1850</th>
      <th>1860</th>
      <th>1870</th>
      <th>1880</th>
      <th></th>
      <th>State</th>
      <th>1850</th>
      <th>1860</th>
      <th>1870</th>
      <th>1880</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>AL</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
      <td></td>
      <td>MO</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
    </tr>
    <tr>
      <td>AZ</td><td>-</td><td>-</td><td>0%</td><td>0%</td>
      <td></td>
      <td>MT</td><td>-</td><td>-</td><td>✓</td><td>✓</td>
    </tr>
    <tr>
      <td>AR</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
      <td></td>
      <td>NE</td><td>-</td><td>✓</td><td>✓</td><td>✓</td>
    </tr>
    <tr>
      <td>CA</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
      <td></td>
      <td>NV</td><td>-</td><td>-</td><td>✓</td><td>✓</td>
    </tr>
    <tr>
      <td>CO</td><td>-</td><td>-</td><td>✓</td><td>✓</td>
      <td></td>
      <td>NH</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
    </tr>
    <tr>
      <td>CT</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
      <td></td>
      <td>NJ</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
    </tr>
    <tr>
      <td>DE</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
      <td></td>
      <td>NM</td><td>-</td><td>0%</td><td>0%</td><td>✓</td>
    </tr>
    <tr>
      <td>DC</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
      <td></td>
      <td>NY</td><td>✓</td><td>✓</td><td>82%</td><td>99%</td>
    </tr>
    <tr>
      <td>FL</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
      <td></td>
      <td>NC</td><td>✓</td><td>84%</td><td>✓</td><td>✓</td>
    </tr>
    <tr>
      <td>GA</td><td>0%</td><td>0%</td><td>0%</td><td>✓</td>
      <td></td>
      <td>ND & SD</td><td>-</td><td>-</td><td>0%</td><td>18%</td>
    </tr>
    <tr>
      <td>ID</td><td>-</td><td>-</td><td>✓</td><td>✓</td>
      <td></td>
      <td>OH</td><td>✓</td><td>26%</td><td>74%</td><td>68%</td>
    </tr>
    <tr>
      <td>IL</td><td>✓</td><td>✓</td><td>46%</td><td>✓</td>
      <td></td>
      <td>OR</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
    </tr>
    <tr>
      <td>IN</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
      <td></td>
      <td>PA</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
    </tr>
    <tr>
      <td>IA</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
      <td></td>
      <td>RI</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
    </tr>
    <tr>
      <td>KS</td><td>-</td><td>✓</td><td>✓</td><td>✓</td>
      <td></td>
      <td>SC</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
    </tr>
    <tr>
      <td>KY</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
      <td></td>
      <td>TN</td><td>✓</td><td>30%</td><td>35%</td><td>✓</td>
    </tr>
    <tr>
      <td>LA</td><td>0%</td><td>0%</td><td>0%</td><td>✓</td>
      <td></td>
      <td>TX</td><td>✓</td><td>✓</td><td>85%</td><td>✓</td>
    </tr>
    <tr>
      <td>ME</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
      <td></td>
      <td>UT</td><td>-</td><td>✓</td><td>✓</td><td>✓</td>
    </tr>
    <tr>
      <td>MD</td><td>✓</td><td>✓</td><td>0%</td><td>✓</td>
      <td></td>
      <td>VT</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
    </tr>
    <tr>
      <td>MA</td><td>✓</td><td>✓</td><td>32%</td><td>✓</td>
      <td></td>
      <td>VA</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
    </tr>
    <tr>
      <td>MI</td><td>✓</td><td>✓</td><td>49%</td><td>✓</td>
      <td></td>
      <td>WA</td><td>-</td><td>✓</td><td>✓</td><td>✓</td>
    </tr>
    <tr>
      <td>MN</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
      <td></td>
      <td>WV</td><td>-</td><td>-</td><td>✓</td><td>✓</td>
    </tr>
    <tr>
      <td>MS</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
      <td></td>
      <td>WI</td><td>✓</td><td>✓</td><td>✓</td><td>✓</td>
    </tr>
  </tbody>
</table>

This table shows our coverage of counties. Percents indicate estimates of the share of establishments that we digitized, given the published county-level tabulations. In 1850, the Census records for three counties in California (Contra Costa, San Francisco, and Santa Clara) were lost and never tabulated, we have complete coverage of the remaining counties in California. Dashes indicate that no survey was conducted, checkmarks indicate that we have complete coverage.






