---
layout: default
title: FAQs
---

# FAQs

- Where did the data come from?
The United States collected a census of manufacturers in the years 1850-1880. Similar to the Census of Population and the Census of agriculture, this process involved sending numerous enumerators (U.S. Marshals and their assistants) to interview manufacturing establishments across the United States. Unlike the Census of Population, there were a few stipulations for what would be included. For example, the Census of Manufactures included only firms that produced goods worth at least $500. Some industries, like “butter, cheese, etc.” were included as home manufacturers on the agriculture census before being included in the manufacturing census more often until presumably complete coverage in 1880.
- Why are there multiple 1880 datasets?
Establishments in 1850-1870 were all canvassed using the same questionaire, although the exact questions varied by decade. In 1880, the Census of Manufactueres was split into three parts, a general schedule, a "special agent" schedule, and a "special" schedule. Many types of firms were included in the general schedule and were given a questionaire similar to those of decades past. Certain firms in industries deemed as important were included in the "special agent" schedule, were someone knowledgeable about the particular industry performed the enumeration with a specially tailored set of questions. A third set of establishments appeared on the "special" schedule. These establishments also belonged to industries considered as important and were canvassed with specific questions, but normal Marshals were used instead of experts. There are twelve industries that fall into this category, and thus 12 slightly different sets of questions.

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

