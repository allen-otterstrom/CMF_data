String Cleaning
============================

This step of the pipeline focuses on standardizing and organizing key text fields—like industry names, materials, and products—across multiple years of the Census of Manufactures (CMF). Using data that had already undergone manual cleaning, do-files were used to ensure that terms were made consistent (e.g., correcting spelling, formatting, and variations in naming). This allowed data from different years and census schedules to be comparable.

For the main census years (1850, 1860, 1870), the cleaning process involved matching original strings to standardized versions using predefined string crosswalks, then consolidating those cleaned values into final fields for industry, materials, and products. The 1880 data required a slightly different approach depending on the schedule type: some required only minimal cleaning, while others like the cheese factory and stone quarry schedules needed targeted processing of specific fields. In the end, all cleaned files were saved in a consistent format, with intermediate steps removed to reduce file size and simplify downstream use. This step ensured a uniform structure across the CMF dataset, enabling reliable cross-year comparisons.

[code](https://dl.dropboxusercontent.com/scl/fi/0o6grsnufpub5qej37miw/round1_apply_all_string_cleaning.do?rlkey=thy8au6l142qyamlfz8ony9il&dl=0)
