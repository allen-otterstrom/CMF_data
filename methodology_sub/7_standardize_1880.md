---
layout: default
title: Standardize 1880
prev: /methodology_sub/6_power_machine_cleaning
next: /methodology_sub/8_variable_cleaning
hide_back: true
---

# Standardize 1880

This step of the pipeline focuses on making the 1880 special schedule data consistent with earlier years by standardizing how products and materials are recorded. Unlike 1850–1870, the 1880 census includes several “special schedules” that each cover specific industries (like cheese, tanning, or sawmills), and each of these has its own unique variable names and formats. The scripts in this step clean and reformat those variables—removing inconsistent names, standardizing units (e.g., pounds, barrels, gallons), and creating clean product and material fields that align with the structure used for earlier census years.

For each of the 12 special schedules, the scripts extract relevant product or material information, reshape it into a consistent format, and assign standardized labels and units. They also group similar items (e.g., different kinds of leather or flour) into broader categories for comparability. Once cleaned, the product and material data are merged back into the main 1880 datasets. The result is a uniform dataset in which product and material information from the 1880 special schedules can be directly compared to the data from 1850, 1860, and 1870.

[code-step1](https://dl.dropboxusercontent.com/scl/fi/j14wn3s1t96vjxi76jsqz/1_1880_ss_materials.do?rlkey=g4b206c44m8kmkv4dfvb9mi06&dl=0)

[code-step2](https://dl.dropboxusercontent.com/scl/fi/853oaf9yao2rdvsqru4j9/2_1880_ss_products.do?rlkey=slqaovecja96vtxf0bva35m06&dl=0)

[code-step3](https://dl.dropboxusercontent.com/scl/fi/igdockrjqbjw0hhb1w6rf/3_merge_products_materials.do?rlkey=tlwyy56q17wc7pin29rtl57vx&dl=0)




