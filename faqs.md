---
layout: default
title: FAQs
---

# FAQs

- 

# Important Notes

#### 1. Non-Numeric Characters in Numeric Fields

Some numeric variables still contain non-numeric characters. These usually reflect unclear or inconsistent entries by Census Marshals. For instance, values like `1.5` for `hands_male` do not make sense in context, but reflect what was written in the original manuscript. These cases are rare but should be handled with care during analysis.

#### 2. Unclassified Industries

While most establishments have been assigned to an industry category, a small number remain unclassified. This typically happens when the transcribed description or listed products are too vague to determine the industry with confidence.

#### 3. Non-Manufacturing Establishments

Not all establishments included in the dataset are manufacturers. For example, fisheries and other non-manufacturing operations were sometimes recorded in the Census and appear in the data. These have been flagged in the industry categorization. Users focusing solely on manufacturing should filter these out.

#### 4. Ambiguity in Labor Reporting

It’s unclear whether owners are included in labor counts (e.g., `hands_male`, `hands_female`). Smaller establishments may be more likely to include owners as workers, but there's no consistent rule. Users should interpret labor variables cautiously.

#### 5. Use of `file_name` Variable

The `file_name` variable often contains useful information about the image source for each observation, based on metadata from the transcription process. However, due to inconsistencies, its structure is not reliable for identifying state or county. Instead, rely on variables like `state`, `county`, and `fips` for geographic information. Use `file_name` primarily to locate the original image.

