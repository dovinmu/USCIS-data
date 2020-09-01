# USCIS-data

This repository collects together data on US citizen naturalizations by field office from the USCIS [Immigrant and Citizenship Data](https://www.uscis.gov/tools/reports-studies/immigration-forms-data) portal. Note that there are only 2 fiscal quarters from 2020, making it look like there's a downward trend. 

![alt text](https://github.com/dovinmu/USCIS-data/blob/master/plots/all_US.png "US Naturalization")

Made using various tools from the Anaconda stack.

## Files

**USCIS scrape and concat.ipynb**: scrapes quarterly reports on naturalizations by field office and puts them together. Puts the results into a CSV called first_pass.csv (not committed to the repo).

**concat_excel_quarters.ipynb**: opens an xlsx file with the remaining quarters of data, which weren't available as CSV and so had to be pasted into an excel file. Saves everything to master_df.csv.

**sum.ipynb**: sums the quarterly data into (fiscal) yearly data, putting the data into three CSVs (in order to exclude non-US and non-US state data) in the data folder.
