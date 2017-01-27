#Helper Datasets
This helper_datasets repo contains look-up tables related to complex datasets that can help simplify steps in your analysis.

##uniquebblbin.csv

28% of the BBLs in NYC have more than one BIN on them. Further complicating things, many building footprints have been assigned dummy BIN numbers (100000, 200000, 300000, 400000, and 500000) when a real BIN number has not been assigned. These issues both make it difficult to easily assign a missing BIN value based on the BBL and visa versa. To help alleviate this issue for the majority of cases, we have created a look-up table of all the distinct 1 BBL-1 BIN relationships, excluding all dummy BINs. As long as your BBL or BIN of interest is in the table, you can use it to safely assign its corresponding missing value. The table was derived from the [Building Footprints](https://data.cityofnewyork.us/Housing-Development/Building-Footprints/nqwf-w8eh/data) data provided by DoITT. More documentation on the source data is [available here](https://github.com/CityOfNewYork/nyc-planimetrics/blob/master/Capture_Rules.md). 

##agencylookup.csv

This table provides the standard agency names and abbrevations used by DCP's Capital Planning division.

##bblcentroids.csv

Coming soon! This table will provide an easy look-up of the centroid coordinates for each BBL in NYC, saving you the step of calculating them.
