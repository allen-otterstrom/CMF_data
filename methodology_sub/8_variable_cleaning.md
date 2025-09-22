---
layout: default
title: Numeric Variable Cleaning
prev: /methodology_sub/7_standardize_1880
hide_back: true
---

# Numeric Variable Cleaning

This step of the pipeline simply attempts to ensure that the numeric variables from the CMF for all years only contain numbers. The steps are as follows, for every numeric variable (capital, material value, production value etc.):

1. Mark if the observation contains non-numeric characters

2. Gather all observations with issues

3. Construct mappings to correct numbers, using the original images if necessary

4. Apply mappings back to the CMF data. 

[code](https://dl.dropboxusercontent.com/scl/fi/vqihjodz3vr1dbh6le1or/variable_cleaning.do?rlkey=3g2iy9hrsfw5mii00jzfw2dwe&dl=0)



