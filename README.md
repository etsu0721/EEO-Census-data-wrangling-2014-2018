# EEO-Census-data-wrangling-2014-2018
The American Community Survey Office (ACSO) released the 2014-2018 5-Year EEO tables via FTP on: [https://www2.census.gov/EEO_2014_2018/](https://www2.census.gov/EEO_2014_2018/). However, the format of the data files needed by the KY EEO Team changed from the format used in [2006-2010](https://www2.census.gov/EEO_2006_2010/), so the steps used to wrangle the 2006-2010 data cannot be reused to wrangle the 2014-2018 data. Thus, new code has been written to wrangle the new data such that the schema and the Power BI dashboard developed for the 2006-2010 data can be reused.

## enumerate_all_categorical_var_combos.ipynb
Enumerates all combinations of report type, gender, race and ethnicity, and value format to produce a unique ID for each.

## process_data_files.ipynb
Wrangles the data file for each geography level needed by the KY EEO Team such that the resulting tables can be related to the table produced by *enumerate_all_categorical_var_combos.ipynb*.
