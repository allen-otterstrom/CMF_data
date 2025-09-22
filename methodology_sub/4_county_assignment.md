---
layout: default
title: County Assignment
hide_back: true
---

# County Assignment

This step of the data pipeline focuses on assigning standardized county information to each manufacturing establishment in the dataset. On the original census manuscripts, county names were handwritten, and those names were initially recorded during the metadata collection phase.  However, to make the data useful for analysis—especially across time and geographic units—those county names had to be cleaned and linked to consistent identifiers. This process involves cleaning the county names, merging them with standardized county lists, and finally assigning historical FIPS codes (standard geographic codes) from the ICPSR for each county.

The process is divided into two major parts. First, the county names are extracted from the file names or manually collected metadata, cleaned, and cross-checked with curated correction files. Where needed, unmatched or ambiguous entries are flagged for manual review. Once a clean set of county assignments is established, the second part of the process links those counties to their corresponding historical FIPS codes using a specially created crosswalk. This ensures consistent county identifiers across all years of the Census of Manufactures. The final output is a set of county-assigned datasets, one for each year and schedule (where applicable).

[code-step1](https://dl.dropboxusercontent.com/scl/fi/a24wclvba9nkcc74o1ngu/1_county_assignment.do?rlkey=dyj7e43yzxmbjcu24mgmfooe0&dl=0)

[code-step2](https://dl.dropboxusercontent.com/scl/fi/859h42q04cjimpbdvak9k/2_merge_fips.do?rlkey=t2iux4pxvjdm8ah5zg9h1p2rg&dl=0)



