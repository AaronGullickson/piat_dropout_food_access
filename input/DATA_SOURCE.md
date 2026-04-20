---
editor: visual
---

# Data Source Description

The data for this project come from two sources. Food availability measures come from the [USDA Food Access Research Atlas](https://www.ers.usda.gov/data-products/food-access-research-atlas), which provides measures of food availability in 2019 at the [US Census tract level](https://en.wikipedia.org/wiki/Census_tract). The remaining tract level data comes from pooled [American Community Survey](https://www.census.gov/programs-surveys/acs.html) (ACS) data from 2017-2021. The ACS is a large 1-in-100 survey of the US population conducted annually by the US Census Bureau. Estimates for small areas are typically pooled across multiple years to limit issues of sampling error.

From the full data, I have extracted and recoded the following variables for our use as an analytical dataset. To load this dataset in R, you just need to run the setup code chunk in the full_report.qmd quarto document. The name of the dataset in R is `tracts_food`.

-   **food_access_pct**: We will use the primary measure of limited access which is measured as not having a supermarket within a half-mile in urban areas and within 10 miles in rural areas. The USDA Food Access Research Atlas estimates the share (percent) of the population within each census tract that lacks this access. This is the key independent variable.
-   **urban**: The urbanicity of the census tract. Either urban or rural. This is the key contextual variable.
-   **rate_dropout**: The percent of 16-19 year old individuals in the census tract who had not completed high school and were not currently attending high school.
-   **pop_density**: The number of 1000 people per squared mile in the census tract.
-   **rate_poverty**: The percent of families in the census tract that had a household income below the federal poverty line.
-   **pct_nonwhite**: The percent of the population in the census tract that identified as non-white.
-   **pct_college**: The percent of the population over 25 years that had earned at least a four-year college degree.
-   **rate_unemploy**: The percent of the labor force that is currently unemployed.
-   **pct_renter**: The percent of residences that are renter-occupied rather than homeowner-occupied.
