Reshape
======================

This step in the pipeline ensures that each manufacturing establishment in the historical Census of Manufactures (CMF) dataset appears as a single row in the final data files. In the raw data, a single establishment might span multiple rows—for example, if it used several types of materials or produced multiple products. This makes it difficult to analyze firms at the establishment level. The reshaping process reorganizes the data so that all information about a single firm is brought together onto one line, enabling easier and more accurate analysis.

For each census year (1850, 1860, 1870, and 1880), the process involves cleaning up duplicate entries, separating less-repeated variables to improve performance, and then restructuring the data so each firm is represented once. The 1880 data, which includes both general and special schedules with more variation in content, required custom approaches for each type of form. After reshaping, missing or empty columns are removed, and final outputs are saved in a clean, consistent format. These reshaped datasets provide a streamlined foundation for establishment-level research and statistical work.

[code-step1](https://dl.dropboxusercontent.com/scl/fi/ab9ls2qjrltr1bc4armfz/reshape1860-1870.do?rlkey=c39gr5ldnf3i1z4c6ztuvta21&dl=0)

[code-step2](https://dl.dropboxusercontent.com/scl/fi/hfxbqh8oruu4trybajm1x/reshape1880.do?rlkey=01qsyqklggn8gg1m3ujfxhx8e&dl=0)
