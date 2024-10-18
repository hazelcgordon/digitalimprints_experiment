## Purpose of project

Welcome! This repository includes all the details for a survey experiment designed to test how effective political campaign digital disclosures can be in informing the public. The study was developed by a research team based at the University of Sheffield, with guidance from the Electoral Commission during the research design process. 

As we are a team based in the UK, this experiment specifically tests the 'digital imprint', a form of disclosure from UK legislation of which the Electoral Commission is responsible for providing guidance and setting out the practical details of the policy. 

Overall, this study fits within a growing body of research seeking to understand how the public use such information to make judgements about who is behind campaign material, whether they are a trustworthy source, and so forth. These studies aim to inform  evidenced based policy about what role digital campaign disclosures can reasonably be expected to play in countering democratic threats faced by citizens and regulators in online environments. 

Overall, this study supports that on a population level, digital disclosures have a small effect on how informed citizens are about the source of campaign content, but this does not further impact evaluations of trustworthiness. Future research testing mediating mechanisms and individual differences in reactions may help illuminate the association between disclosures and perceptions of trust.

## Details of repository

- doc: 'index.rmd': this is the main analysis document of the project, that includes all the code for the final version of the analysis included in the main paper (this is not finalised yet)

### Where are the raw and processed data files?

### Where is the description of the dataset?

### Where can I find details about the sample?

### Did the hypotheses tested match those in the preregistration?

### Did the final analysis models match those in the preregistration?

### How do I run the pre-registered analysis script for comparison?

### What data was collected that might be useful for a secondary analysis?


### Extra repository details

- folder: 'pilot_study': this includes all data, wrangling code and analysis code for the pilot study
  - doc: 'pilot_analysis_plan.rmd': The pre-registered analysis script that was developed using the pilot data
  - doc: 'pilot_datawrangle.rmd': data wrangling code used for the pilot data
  - doc: 'pilot_to_main_code_changes.md': text document summarising any changes between the pilot data analysis and main analysis that arose from corrections being made to the survey
- folder: 'rawdata_with_wranglecode': this includes raw anonymised data and all corresponding wrangling code
  - doc: 'data_quality_check.rmd': explains data quality checks that were made on the non-anonymised data set to form the anonymised 'main_data.csv'
  - doc: 'main_datawrangle.rmd': includes data quality exclusions at the beginning, if data 'main_data.csv' is downloaded this script should run smoothly to create the 'processed_data.csv' (which can also be accessed from folder 'processed_data')
  - doc: 'sample_details.rmd': code underlying the sample breakdown in folder 'details_of_sample'
- folder 'figures': this will eventually have all figures used in the final paper versions and supplementary materials; also includes histograms of all the uni-variate distributions for inspection and (eventually) assumptions of key models
- folder 'tables': this will eventually have all tables for the main and supplementary materials of the final papers

*This project is in the stage of being written into a manuscript, final scripts may be updated*

Please feel free to get in contact at hcgordon1@sheffield.ac.uk if you have any questions!