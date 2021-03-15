# Iconicity mega ratings

This repository contains all the main scripts and data that are needed to reproduce the analysis that we report for the iconicity ratings.

The main script folder contains the following files:

- `processing_raw_ratings.Rmd` : takes the `combined_byWord_and_subject_anonymized.csv` file, applies exclusion criteria and aggregates the data to yield the cleaned file, which is the main iconicity ratings file that will be used for all analyses `iconicity_ratings.csv`

- `bayesian_models.Rmd` : takes `iconicity_ratings.csv` and performs a series of analysis, specifically correlations with other lexical measures from published studies that are in the `additional_data` folder

- `bayesian_models.Rmd` : posterior predictive checks for all models that will be saved in the folder `pp_checks`

- `substantive_analysis.Rmd` : the main analysis script that reproduces all the main results reported and creates plots (this script loads in the models created by `bayesian_models.Rmd`)
