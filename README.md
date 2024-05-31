# BrainStation Data Science Capstone Template

This is a template repository for setting up your capstone project: it includes a simple folder structure and placeholder files for the most important assets you will be creating.

## Usage

1. Start a new GitHub repo using this template.
2. Update your `LICENSE` file with date and owner.
3. Update your `README.md` file to reflect the project - see a sample structure below and please refer to Synapse on what needs to be included here. 
4. Set up and activate your conda environment:
    - Create a new `conda` environment for your capstone project.
    - Activate the environment and export:
        ```bash
        conda env export > conda.yml
        ```
    - Make sure re-export every time after you update the environment.
    - You can reset your conda environment by running:
        ```bash
        conda env create -f conda.yml
        conda activate <your-env-name>
        ```
5. Add your own notebooks in `./notebooks/` and remove placeholders.
6. Add your own data in `./data/` and remove placeholder. Note: `.gitignore` will ignore the data folder when you push to github, save a copy of your raw and processed data, pickled models in a Google Drive folder and add the link in the `data_links.md` file.
7. Add your project documents, figures, reports, presentation pdf's in the `./docs` and remove placeholders.
8. Add your references (tutorials, papers, books etc.) in `./references`. 
9. Add your own scripts in `./src/` and remove unnecessary folders.

Feel free to rename the folder and customize the project structure to best fit your work - this template is just the starting point.

------------------------------------------------------------------------------

## Predicting Regular Season NBA Games Outcome + Scores with Machine Learning
=========================

### Overview
The objective is to predict the outcome and scores of any regular season NBA game of any given team by training a model that take parameters/features such as 
 - team performance
 - player stats
 - related stats/variations of the above

Ideally, the model will be able to predict with 65%+ from feeding it with a small sample size of significant game training data.

... Data Collection: Gather historical NBA game data, including team statistics, player performance metrics, and game outcomes, from reliable sources such as official NBA APIs or datasets.

... Data Preprocessing: Clean the data by handling missing values, removing duplicates, and addressing inconsistencies. Perform feature engineering and find/create meaningful predictors such as team win percentage, player efficiency ratings etc.

... Model Selection: Choose appropriate machine learning algorithms such as logistic regression or classification for outcome prediction and regression for score prediction. Experiment with different models to find the one that best fits the data and the problem.

... Model Training: Split the data into training and testing sets. Train the selected models on the training data, and tune it using test data.

... Model Evaluation: Evaluate the trained models on the testing data using accuracy and scores.

... Iterative Improvement: Iterate on the model development process, refining features, experimenting with different algorithms, and incorporating new data to improve prediction accuracy and scores.

... Use it in real worl scenaries: Use the trained model for real-time predictions. Continuously monitor model performance and update the model as needed to adapt to current NBA seasons.

### Executive Summary

... Define the problem
... What is the data science opportunity
... Key takeaways

### Demo

... Show your work:
...     Data visualizations
...     Interactive demo (e.g., `streamlit` app)
...     Short video of users trying out the solution


### Methodology

... High-level diagrams of entire process:
...     various data processing steps
...     various modelling directions
...     various prototyping directions


### Organization

#### Repository 

* `data` 
    - contains link to copy of the dataset (stored in a publicly accessible cloud storage)
    - saved copy of aggregated / processed data as long as those are not too large (> 10 MB)

* `model`
    - `joblib` dump of final model(s)

* `notebooks`
    - contains all final notebooks involved in the project

* `docs`
    - contains final report, presentations which summarize the project

* `references`
    - contains papers / tutorials used in the project

* `src`
    - Contains the project source code (refactored from the notebooks)

* `.gitignore`
    - Part of Git, includes files and folders to be ignored by Git version control

* `conda.yml`
    - Conda environment specification

* `README.md`
    - Project landing page (this page)

* `LICENSE`
    - Project license

#### Dataset

... Google Drive links to datasets and pickled models

### Credits & References

... Include any personal learning
