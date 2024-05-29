# ohio Election Shapefile

This shapefile was processed by Professor Ellen Veomett and her student Ananya Agarwal.

# **Sources**
@author: eveomett AI for Redistricting, USF All data retrieved 05/29/24:

Obtain the following data from Restricting Data Hub

[Population data](https://redistrictingdatahub.org/dataset/ohio-block-pl-94171-2020-by-table/): based on the decennial census at the Census Block level on 2020 Census Redistricting Data

[Congressional District data](https://redistrictingdatahub.org/dataset/2022-ohio-congressional-districts-approved-plan/): 2022 ohio Congressional Districts plan enacted on 2/27/23

[State House District data](https://redistrictingdatahub.org/dataset/2024-ohio-state-house-districts-approved-plan/): 2022 State House Approved Plan

[State Senate District data](https://redistrictingdatahub.org/dataset/2024-ohio-senate-districts-approved-plan/): 2022 State Senate Approved Plan

[2020 election data](https://redistrictingdatahub.org/dataset/vest-2020-ohio-precinct-and-election-results/)**:**  VEST 2020 ohio precinct and election results

[2018 election data](https://redistrictingdatahub.org/dataset/vest-2018-ohio-precinct-and-election-results/)**:**  VEST 2018 ohio precinct and election results

[2016 election data](https://redistrictingdatahub.org/dataset/vest-2016-ohio-precinct-and-election-results/)**:**  VEST 2016 ohio precinct and election results

## Preprocessing
Demographic data were aggregated from the block level using MGGG’s proration software [maup](https://github.com/mggg/maup). Congressional, house, and senate district IDs were assigned to precincts also using this package.

## Metadata
* `CNTYFIPS`: County FIPS code
* `COUNTY`: County name
* `CODE`: County-level precinct code
* `PRECODE`: County FIPS and precinct code (precinct unique identifier)
* `PRECINCT`: Precinct name
* `PRENAME`: Precinct name from tabular results
* `TOTREG16`: Total registered voters on November 8, 2016
* `TOTVOTE16`: Total votes cast on November 8, 2016
* `TURNOUT16`: Turnout proportion on November 8, 2016
* `PRES16R`: Number of votes for 2016 Republican presidential candidate
* `PRES16D`: Number of votes for 2016 Democratic presidential candidate
* `PRES16L`: Number of votes for 2016 Libertarian presidential candidate
* `PRES16G`: Number of votes for 2016 Green Party presidential candidate
* `SEN16R`: Number of votes for 2016 Republican senate candidate
* `SEN16D`: Number of votes for 2016 Democratic senate candidate
* `USH16R`: Number of votes for 2016 Republican US congressional candidates
* `USH16D`: Number of votes for 2016 Democratic US congressional candidates
* `SSEN16R`:  Number of votes for 2016 Republican state senate candidates
* `SSEN16D`:  Number of votes for 2016 Democratic state senate candidates
* `STH16D`:  Number of votes for 2016 Republican state house candidates
* `STH16R`:  Number of votes for 2016 Democratic state house candidates
* `TOTPOP`: Total population 
* `NH_WHITE`: White, non-hispanic, population
* `NH_BLACK`: Black, non-hispanic, population
* `NH_AMIN`: American Indian and Alaska Native, non-hispanic, population
* `NH_ASIAN`: Asian, non-hispanic, population
* `NH_NHPI`: Native Hawaiian and Pacific Islander, non-hispanic, population
* `NH_OTHER`: Other race, non-hispanic, population
* `NH_2MORE`: Two or more races, non-hispanic, population
* `HISP`: Hispanic population
* `H_WHITE`: White, hispanic, population
* `H_BLACK`: Black, hispanic, population
* `H_AMIN`: American Indian and Alaska Native, hispanic, population
* `H_ASIAN`: Asian, hispanic, population
* `H_NHPI`: Native Hawaiian and Pacific Islander, hispanic, population
* `H_OTHER`: Other race, hispanic, population
* `H_2MORE`: Two or more races, hispanic, population
* `VAP`: Total voting age population
* `HVAP`: Hispanic voting age population
* `WVAP`: White, non-hispanic, voting age population
* `BVAP`: Black, non-hispanic, voting age population
* `AMINVAP`: American Indian and Alaska Native, non-hispanic, voting age population
* `ASIANVAP`: Asian, non-hispanic, voting age population
* `NHPIVAP`: Native Hawaiian and Pacific Islander, non-hispanic, voting age population
* `OTHERVAP`: Other race, non-hispanic, voting age population
* `2MOREVAP`: Two or more races, non-hispanic, voting age population
* `CD`: US congressional district ID
* `SEND`: State Senate district ID
* `HDIST`: State House district ID

## Projection
This shapefile uses a NAD83(Harn)/UTM zone 17 North projection (EPSG:3747).