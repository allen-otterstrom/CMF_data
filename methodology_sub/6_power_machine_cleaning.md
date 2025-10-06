---
layout: default
title: Power and Machine Cleaning
prev: /methodology_sub/5_industry_assignment
next: /methodology_sub/7_standardize_1880
hide_back: true
---

# Power Machine Cleaning

This step of the data pipeline focuses on identifying the type of power used by each manufacturing establishment—such as steam, water, wind, or animal power. Because firms often described their power sources inconsistently or used different terms for the same thing, this step involves carefully cleaning and categorizing those entries. The process uses a standardized mapping file to translate raw power-related text into consistent categories. These are then used to create binary indicators (yes/no flags) for each type of power source a firm may have used.

Once the power types are cleaned and classified, the process also extracts any information related to machinery—what kind of machines were used and in what units. All of this is then merged back into the main dataset so that each firm has a clear record of its power and machinery profile. For specific industries like lumber or flour milling, additional logic is applied to flag steam or water power based on known keywords, even if power wasn't explicitly listed. The result is a standardized, easy-to-use set of variables indicating how each firm was powered, enabling analysis of industrial technology and energy use over time.

[code-step1](https://dl.dropboxusercontent.com/scl/fi/x00e5ba09jrg4nzzf5r2v/clean_1850_power_machine_vars.do?rlkey=20zhf72ogphi4fq1u4j9yi5jn&dl=0)

[code-step2](https://dl.dropboxusercontent.com/scl/fi/x429kakjn3ukwpysrm1yh/clean_1860_power_machine_vars.do?rlkey=qz8k6uleq153oo90jn5zb15rt&dl=0)

[code-step3](https://dl.dropboxusercontent.com/scl/fi/buxadot4gsqs34i40mlgw/clean_1870_power_machine_vars.do?rlkey=4l16jy7x45w5au7aab2k7kvi8&dl=0)



 




