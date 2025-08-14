---
layout: default
title: Methodology
---

# Collection

The original census manuscripts (the paper sheets filled out by enumerators) ended up scattered in archives and libraries nationwide. To work with them, the project first had to create a complete set of digital images.

**Key steps**

- **Locate the records**
  
  - Manuscripts were found in state archives, the National Archives, university libraries, and on Ancestry.com.

- **Acquire images or microfilm**
  
  - Where digital scans already existed, copies were obtained.
  
  - Where only microfilm was available, reels were borrowed or purchased.

- **Digitize microfilm**
  
  - The University of Chicago Library scanned the microfilm into high‑resolution images.

- **Standardize the images**
  
  - Most scans captured two manuscript pages per image; many were blank or contained only enumerators’ notes.
  
  - Every image was reviewed to identify pages with usable data.

- **Publish the image set**
  
  - All vetted images are now hosted on the project’s data website for public access.

These steps produced a unified, quality‑controlled image archive that serves as the foundation for further data extraction and analysis.

# Image Processing and Metadata Collection

Once the initial images were obtained, they were processed into individual pages using code and organized into packages by state and year. Undergraduate research assistants (RAs) then reviewed each image to determine whether it included a manufacturing schedule, recorded establishment counts and county names, flagged legibility or quality issues, and made notes about duplicates or nullified entries. This metadata was recorded in standardized CSV files.

To assess coverage, the team compared the total number of establishments in the images with published historical census aggregates. Gaps were identified and additional images were sought when needed. Clean metadata files were used to generate renaming CSVs, which encoded all relevant metadata into standardized filenames.

## Data Transcription

Once images were split, organized, renamed, and metadata gathered, the transcription process began. Images and Excel batches with column names reflecting the original column names on the manuscripts were given to a data team to be transcribed. Each item was double transcribed by two different associates, with a third resolving any differences. In total, there were 65,211 manuscript images with manufacturing establishments, including 28,506 pages from 1880. The average page had 7 establishments. When we have records for a state and decade, the records are normally complete for the entire state. For some states and decades, there are some entire counties missing or parts of counties from comparing our establishment totals to the published county-level tabulations (see the explanation of [coverage](coverage.html)).

## Raw Data Processing and Cleaning

To help clean the data, we received assistance from many UChicago undergraduates, graduate students, and full-time research professionals. The team randomly checked many entries, finding a low error rate. We also used a useful feature of the manuscripts to verify numeric entries on many sheets: many 19th-century enumerators entered *totals*, such as writing the total production value for the entire page or for a given firm. We also digitized these row totals and page totals, and compared the entered total with the sum of the relevant responses. Consistent with our general verification of the data, the most common sources for discrepancies were that the total was calculated incorrectly by the enumerator or the total reflected a sum of values that were later crossed out and replaced with other values. In these cases, we made no changes. We also manually checked entries when a ratio seemed highly unusual, such as the output to employment ratio, which was inspired by the data cleaning processes at the current U.S. Census.

We manually processed the entered strings for product names, material inputs, and self-reported industry, along with categorizing the entered power strings based on relevant information such as "water" and "steam". The overall goal was to standardize misspellings and British spellings, expand abbreviations, and assign strings to broader categories. To clean industries, we also used the product strings.

Some values for string variables were entered in the "wrong place", when the surveyor had run out of room, which we manually corrected. Similarly, we corrected when numeric variables were entered in a string column. Some entries were marked with a question mark, when the data processing team could not read part or all of a cell. We looked at those entries, and were rarely able read them either.

In addition to these manual steps, many algorithmic and other cleaning steps performed through code were required to get the data into a usable state. The entire set of cleaning and preparation steps that take the data from its raw entered form to its current state are outlined below.

1. [Manual Steps](methodology_sub/1_manual_cleaning.html)
2. [String Cleaning](methodology_sub/2_string_cleaning.html)
3. [Reshape](methodology_sub/3_reshape.html)
4. [County Assignment](methodology_sub/4_county_assignment.html)
5. [Industry Classification](methodology_sub/5_industry_assignment.html)
6. [Power and Machine Cleaning](methodology_sub/6_power_machine_cleaning.html)
7. [Standardize 1880](methodology_sub/7_standardize_1880.html)
8. [Numeric Variable Cleaning](methodology_sub/8_variable_cleaning.html)


