---
layout: default
title: Standardize 1880
---

# Standardize 1880

This step of the pipeline focuses on making the 1880 special schedule data consistent with earlier years by standardizing how products and materials are recorded. Unlike 1850–1870, the 1880 census includes several “special schedules” that each cover specific industries (like cheese, tanning, or sawmills), and each of these has its own unique variable names and formats. The scripts in this step clean and reformat those variables—removing inconsistent names, standardizing units (e.g., pounds, barrels, gallons), and creating clean product and material fields that align with the structure used for earlier census years.

For each of the 12 special schedules, the scripts extract relevant product or material information, reshape it into a consistent format, and assign standardized labels and units. They also group similar items (e.g., different kinds of leather or flour) into broader categories for comparability. Once cleaned, the product and material data are merged back into the main 1880 datasets. The result is a uniform dataset in which product and material information from the 1880 special schedules can be directly compared to the data from 1850, 1860, and 1870.

[code-step1](https://dl.dropboxusercontent.com/scl/fi/6dumktk27vtfaql1640uq/1_1880_ss_materials.do?rlkey=bhx8gmwfh37no0qe4dx4icyik&dl=0)

[code-step2](https://dl.dropboxusercontent.com/scl/fi/kr4seuvnv5d0w4vg6re5d/2_1880_ss_products.do?rlkey=h5o6935fd45mpb549r9us3ekh&dl=0)

[code-step3](https://dl.dropboxusercontent.com/scl/fi/0f3rr7kpa1j6fywo2pwjg/3_merge_products_materials.do?rlkey=rnybxiwv6gccardus85ymowag&dl=0)

