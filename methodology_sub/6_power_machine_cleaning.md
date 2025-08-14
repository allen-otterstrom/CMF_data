# Power Machine Cleaning

This step of the data pipeline focuses on identifying the type of power used by each manufacturing establishment—such as steam, water, wind, or animal power. Because firms often described their power sources inconsistently or used different terms for the same thing, this step involves carefully cleaning and categorizing those entries. The process uses a standardized mapping file to translate raw power-related text into consistent categories. These are then used to create binary indicators (yes/no flags) for each type of power source a firm may have used.

Once the power types are cleaned and classified, the process also extracts any information related to machinery—what kind of machines were used and in what units. All of this is then merged back into the main dataset so that each firm has a clear record of its power and machinery profile. For specific industries like lumber or flour milling, additional logic is applied to flag steam or water power based on known keywords, even if power wasn't explicitly listed. The result is a standardized, easy-to-use set of variables indicating how each firm was powered, enabling analysis of industrial technology and energy use over time.

[code-step1](https://dl.dropboxusercontent.com/scl/fi/rasleottca9mvvwbe1v02/clean_1850_power_machine_vars.do?rlkey=hbe17lvh2dexabgipyqe7lfv5&dl=0)

[code-step2](https://dl.dropboxusercontent.com/scl/fi/osrwzz9faflkj99pdmork/clean_1860_power_machine_vars.do?rlkey=7bhgficulmu8tizdplhf71cnf&dl=0)

[code-step3](https://dl.dropboxusercontent.com/scl/fi/m17tpr7qzh19cvo9f5hnb/clean_1870_power_machine_vars.do?rlkey=53brvl70a4qjl105l767sfmpa&dl=0)



 
