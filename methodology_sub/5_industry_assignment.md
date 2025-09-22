---
layout: default
title: Industry Classification
prev: /methodology_sub/4_county_assignment
next: /methodology_sub/6_power_machine_cleaning
hide_back: true
---
# Industry Classification

This step in the pipeline standardizes the industry classifications for all establishments across the Census of Manufactures from 1850 to 1880. Originally, industry information was recorded in inconsistent and often ambiguous text entries (e.g., “mill,” “cabinet,” or “bootmaker”), which made analysis across years and locations difficult. This step addresses that by cleaning the original text strings, matching them to standardized industry categories using crosswalks, and assigning each firm a set of consistent industry labels. These include both detailed and broader classifications that allow users to group establishments according to the level of industry specificity needed for their analysis.

The process begins by cleaning raw industry labels and matching them to cleaned values previously compiled by research assistants. From there, entries are either automatically classified using keyword-based logic (especially for common industries like flour and lumber mills) or matched against manually reviewed crosswalks. For the 1880 special schedules, industry assignments are often hardcoded based on the known content of each form (e.g., all firms in SS2 are boot and shoe manufacturers). In the final step, each firm is assigned hierarchical industry codes ranging from specific (“flour and grist mills”) to broad (“food manufacturing”), making the data ready for consistent, high-quality historical analysis.



[code-step1](https://dl.dropboxusercontent.com/scl/fi/uird86x1wyzwitkiswbu9/1_industry_assignment.do?rlkey=xjvg9f5zkapj7p0vblk98b96q&dl=0)

[code-step2](https://dl.dropboxusercontent.com/scl/fi/6or4m4rwzdhfp6u7iei3e/2_add_hand_crosswalk.do?rlkey=124u5v3mkuzniq64p65oyfz2s&dl=0)

[code-support1](https://dl.dropboxusercontent.com/scl/fi/roaacaisowhgxg6xmp5ig/industry_raw_clean.do?rlkey=u4g8kwezsitvv428c57ftwupl&dl=0)

[code-support2](https://dl.dropboxusercontent.com/scl/fi/opjct87bnralezpn19r9n/infer_industry_classification.do?rlkey=z4tjtkj1dvpxql65venrblv0c&dl=0)



