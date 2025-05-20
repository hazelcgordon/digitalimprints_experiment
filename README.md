## Purpose of project

Welcome! This repository includes all the details for a survey experiment designed to test how effective political campaign digital disclosures can be in informing the public. The study was developed by a research team based at the University of Sheffield, with guidance from the Electoral Commission during the research design process. 

As we are a team based in the UK, this experiment specifically tests the 'digital imprint', a form of disclosure from UK legislation of which the Electoral Commission is responsible for providing guidance and setting out the practical details of the policy. 

Overall, this study fits within a growing body of research seeking to understand how the public use such information to make judgements about who is behind campaign material, whether they are a trustworthy source, and so forth. These studies aim to inform  evidenced based policy about what role digital campaign disclosures can reasonably be expected to play in countering democratic threats faced by citizens and regulators in online environments. 

Overall, this study supports that on a population level, digital disclosures have a small effect on how informed citizens are about the source of campaign content through boosting perceptions of persuasion knowledge (advertisement recognition) and perceptions of credibility. We also showed half of the participants an 'information campaign', designed to make them aware of the purpose of disclosures and their legal significance in the UK, to see how this interacted with viewing a disclosure. An educational intervention was also shown to make disclosures more comprehensible i.e. participants better used the presence or absence of a source disclosure to assess their own knowledge of the source. We did not find the educational intervention had an effect on perceptions of credibility or the perception that electoral oversight is effective.

## Details of repository

The final analysis can be viewed under 'index.rmd', the main analysis document of the project, that includes all the code for the final version of the analysis included in the main paper *(this is not finalised yet)*

### Where are the raw and processed data files?

The raw datafile can be viewed in the /rawdata_with_wranglecode folder under 'main_data.csv'. 

Running the 'main_datawrangle.Rmd' script will reformat the data into long form with 4 rows for each participant; if the repo has been cloned, this should run smoothly. Please alter the 'read.csv' part of the code if the data and script have been downloaded separately. This script will generate 3 dataframes, 'data' (unprocessed), 'imprint_df' (4 row per participant) and 'training_df' (1 row per participant, excludes repeated measures variables). Most tests will use imprint_df.

The processed datasets can also be downloaded directly from within /processed_data. Please check variables are converted to the correct format (e.g., factor levels set) before analyses are run. 

### Where is the description of the dataset?

The full survey and variable codebook can be found in /processed_data. Corresponding variable names are in bold.

### Where can I find details about the sample?

A table summarising the main demographics of the sample can be found in /details_of_sample. Other sample attributes of interest that can be checked separately include: social media use, frequency of facebook use. 

### What data quality checks were conducted?

Please see document 'data_quality_check.rmd' in /rawdata_with_wranglecode which explains data quality checks that were made on the non-anonymised data set to form the anonymised 'main_data.csv'.

### Did the hypotheses tested match those in the preregistration?

Yes, only the pre-registered hypotheses are tested in the paper.

### Did the final analysis models match those in the preregistration?

The final models are very similar to those preregistered, however some of the final models differed due to considerations that came to light during the data analysis process, such as which models structure provided the best fit. Full justification of any changes can be viewed in the document 'supplementary materials.Rmd' which can be knitted to create an easy to navigate html document. 

*This document will be added very soon*

### How do I run the pre-registered analysis script for comparison?

The pre-registered analysis code can be run in full with the script 'preregistered_analysis_code.Rmd'. If the repo has been cloned, this script can be knitted to generate a formatted html document through which the initial version of the results can be browsed through. 

### What data was collected that might be useful for a secondary analysis?

This dataset collected many variables that would be suitable for secondary analysis:

- Political trust, mistrust and cynicism
- Political internal and external efficacy
- Key political demographics e.g., UK political party support, support for democracy

Please see the codebook under /processed_data for the full survey.

### Extra repository details

- folder: 'pilot_study': this includes all data, wrangling code and analysis code for the pilot study
  - doc: 'pilot_analysis_plan.rmd': The pre-registered analysis script that was developed using the pilot data
  - doc: 'pilot_datawrangle.rmd': data wrangling code used for the pilot data
  - doc: 'pilot_to_main_code_changes.md': text document summarising any changes between the pilot data analysis and main analysis that arose from corrections being made to the survey
- folder 'figures': this will eventually have all figures used in the final paper versions and supplementary materials; also includes histograms of all the uni-variate distributions for inspection and (eventually) assumptions of key models
- folder 'tables': this will eventually have all tables for the main and supplementary materials of the final papers

*This project is in the stage of being written into a manuscript, final scripts may be updated*

Please feel free to get in contact at hcgordon1@sheffield.ac.uk if you have any questions!
