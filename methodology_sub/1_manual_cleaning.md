---
layout: default
title: Manual Checking
---

# Manual Checking

The CMF data are very rich, but the irregularites present in original source are such that many things had to be manually checked and fixed. Manually made crosswalks and similar tools were used in the later pipeline, but these four steps were overwhelmingly accomplished by undergraduate research assisntants and associates at DDD, and thus are considered to be manual steps.

1. ## Error Checking:
   
   - Purpose: To find cases of mis-transcription in numeric variables and fix them.
   
   - Process:
     
     - Within the census sheets themselves, totals were added up by Census Marshals.
     
     - After transcription, totals were computed based on entered data and compared to the totals written on the census sheets.
     
     - Cases where they were not equivalent were then checked by research assistants. Transcription errors were then corrected, or the Research Assistant determined that the Marshal made an error.

2. ## Firm line and Firm Number Cleaning:
   
   - Purpose: To make minor corrections to firm line and firm number. In some cases these were missing, and in other cases had incorrect characters or were wrong in other ways.
   
   - Process:
     
     - Many cases fixed in this step were known problems, and thus were manually fixed with the aid of an algorithm.
     
     - Non-numeric firm numbers in 1880 were systematically fixed with simple Stata code:
     
     - ```Stata
       local filelist SS1 SS2 SS3 SS4 SS5 SS6 SS7 SS8 SS9 SS12
       foreach s of local filelist{
         use "${input}/4_apply/output/aug2020/CMF_1880_`s'.dta", clear
         replace firm_number = "" if firm_number == "."
         replace firm_line = "" if firm_line == "."
         gen non_numerical = 1 if !regexm(firm_number, "[0-9]")
         replace non_numerical = 1 if !regexm(firm_line, "[0-9]")
         save "${output}/interm/5a_SS_to_clean/5a_CMF_1880_`s'_to_clean.dta", replace
       }
       ```

3. ## Establishment Fixing:
   
   - Purpose: For variables like capital, wage, hands employed, and industry, each establishment should only have one value in each of these variables. Sometimes this isn't the case, and this step fixes the cases where this happens.
   
   - Process:
     
     - Simple code was used to flag such firms:
     
     - ```Stata
       gen tag = 1 if firm_name != "" & firm_line != 1 
       foreach var of varlist capital avg_wage_male avg_wage_female industry_raw hands_male hands_female {
       replace `var' = "" if `var' == "."
       replace tag = 1 if `var' != "" & firm_line != 1 
       }
       egen image_to_check = sum(tag), by(file_name)
       ```
     
     - Once a firm was flagged, a research assistent then went in and checked the transcribed data against what was recorded on the census sheet.
     
     - When there was a mistake in transcription, this was note and corrected. If there really were multiple values for the numeric variables outlined above, this meant that the same owner owned two establishments. When that was the case, the establishments were then split to reflect that.
     
     - Corrections were then compiled and applied to the data.

4. ## Duplicate Establishment ID checking.
   
   - Purpose: Find and eliminate duplicate establishments. At this point, file name, firm number and firm line should have been unique. This phase of duplicate elimination focused on establishments that were, for one reason or another, entered into the data twice. This was due to both mistakes from the Census Marshals themselves and DDD associates.
   
   - Process:
     
     - Use simple code to identify duplicates in file name, firm number and firm line:
     
     - ```Stata
       duplicates tag file_name firm_number firm_line, gen(dup)
       gen obs_order = _n
       bysort file_name firm_number firm_line (obs_order): gen dup_group = _n if dup!=0
       drop obs_order
       order dup dup_group
       ```
     
     - RA's then went through and determined which of these duplicates to drop.

