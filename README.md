# Iconicity ratings for 14,000+ English words

This repository contains all the main scripts and data that are needed to reproduce the analysis that we report for the iconicity ratings in the following paper:

Winter, Bodo, Gary Lupyan, Lynn K. Perry, Mark Dingemanse, and Marcus Perlman. “Iconicity Ratings for 14,000+ English Words.” Behavior Research Methods, April 20, 2023. https://doi.org/10.3758/s13428-023-02112-6.

For all analyses using our iconicity ratings, we recommend using the `iconicity_ratings_cleaned.csv` file in the `ratings` folder. This contains the files that are processed.

The main script folder contains the following files:

- `processing_raw_ratings.Rmd` : takes the `combined_byWord_and_subject_anonymized.csv` file, applies exclusion criteria and aggregates the data to yield the cleaned file, which is the main iconicity ratings file that will be used for all analyses `iconicity_ratings.csv`

- `bayesian_models.Rmd` : takes `iconicity_ratings.csv` and performs a series of analysis, specifically correlations with other lexical measures from published studies that are in the `additional_data` folder

- `bayesian_models.Rmd` : posterior predictive checks for all models that will be saved in the folder `pp_checks`

- `substantive_analysis.Rmd` : the main analysis script that reproduces all the main results reported and creates plots (this script loads in the models created by `bayesian_models.Rmd`)

- `calculate_ICCs.Rmd` : inter-rater reliability measures added after review

