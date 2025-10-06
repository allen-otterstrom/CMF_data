---
layout: default
title: Numeric Variable Cleaning
prev: /methodology_sub/7_standardize_1880
next: /methodology_sub/important_notes
hide_back: true
---

# Numeric Variable Cleaning

Numeric variables in the Census of Manufactures data (such as capital, materials, labor, and product values) required extensive cleaning to address both non-numeric entries and transcription errors. Many census marshals entered text or notes into numeric fields—for example, writing “6000 Real” for capital or “10 boys” for male workers—necessitating the identification and removal of non-numeric content. Additional issues stemmed from transcription errors in the DDD digitization process, where text from other columns (e.g., “raw turpentine”) was mistakenly placed in numeric fields or numeric values were mis-entered due to unclear handwriting or misplaced decimals (e.g., 8,400 recorded as 84,000). Unlike string variables, numeric variables were corrected directly, and no unaltered raw versions are retained in the final dataset.

Cleaning proceeded in two stages. First, all entries containing non-numeric characters were extracted and reviewed manually, with research assistants creating crosswalks to correct legible cases. Unreadable entries, often marked with a “?”, were addressed when possible, though some remain unresolved for users to handle. The second stage targeted extreme or improbable numeric values, which were harder to detect because they appeared valid at first glance. We flagged potential errors by reviewing the top ten establishments by key numeric variables in each year and correcting anomalies found in the manuscripts. We also used Mahalanobis distance measures—calculated within each industry using both raw variables and their ratios—to identify outliers inconsistent with typical industry patterns. By examining which variables contributed most to each establishment’s distance from the industry mean, we were able to pinpoint and verify likely transcription errors systematically.
[code](https://dl.dropboxusercontent.com/scl/fi/fmdrsixua0l49meyly80x/variable_cleaning.do?rlkey=jcgu8uivtz2qnnia3g607v764&dl=0)






