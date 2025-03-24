# Code Folder

## Code Location:

This directory contains `.R` or `.qmd` scripts in the folders as appropriate:

- `Processing_code` cleans raw data and converts to processed data
- `Analysis_code` performs analyses on cleaned data. 


## Code Design:

The data cleaning in the `Processing_code` folder is done three ways: one R script, v1 qmd and v2 qmd files. The v1 qmd duplicates the R script but is formatted as a report. The v2 qmd sources code chunks from the .R script and includes only the text and formats the output, promoting less code maintenance. 

All of the methods load the appropriate data (e.g. raw or processed), perform actions, and save results (e.g. processed data, figures, computed values) in the appropriate folders. 

**Relative paths** are used so that each script works from the working directory set to the folder that the script is in. 

## Code Documentation:

## `processingcode.R` - cleans raw data, outputs clean data

### Inputs
	reads in the following files from `../../Data/Raw_data/`
		`penguins_raw_dirty.csv` - The raw data
		`datadictionary.csv` - The data dictionary for the raw data

### Outputs
	outputs to `../../Data/Processed_data/`
		`processeddata.rds` - clean data in rds (R) format
		`processeddata.csv` - clean data in .csv format
		`orig_names.rds` - short variable names associated with long original variable names in rds format

