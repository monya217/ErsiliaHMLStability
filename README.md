# Ersilia Model EOS30GR Analysis
## Overview
This repositery contains code and analysis of model EOS30GR provided by Ersilia for Outreach 2024 Summer Internship Contribution Period. The model can be used to predict the probability that a molecule is a hERG blocker. 
The first step in the analysis was to check for model bias. I used dataset of 1000 compounds from the ChEMBL database and predicted the outcomes by fetching and runing the model using Ersilia. Then I used data visualizations to look for probability distribution and other trends.


## Repository organisation
The repository is organised in folders:

'/notebooks' contains the jupyter notebooks where most of the work is being developed
'/data' contains all the .csv files. Model predictions are obtained outside this repository and saved in this folder. Subfolders might be created if needed
'/src' contains important functions I will re-use throughout the repository, to avoid typing them each time
'/figures' contains the plots I have produced during the model validation process
'requirements.txt' lists all the required packages to run the notebooks in this repository. If possible I also specify the version of the package I am using.

## Steps to Reproduce the repository

1. Download ersilia by following these [instructions](https://ersilia.gitbook.io/ersilia-book/ersilia-model-hub/installation).
2. Run the model on your system using these [instructions](https://ersilia.gitbook.io/ersilia-book/ersilia-model-hub/antibiotic-activity-prediction) or simply use these commands:
  ersilia -v fetch eos30gr
  ersilia serve eos30gr
  ersilia -v api run -i data/input.csv -o data/output.json
3. Compare and explore with results in the repository.
