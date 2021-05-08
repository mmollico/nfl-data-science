# NFL Data Science

#### Project Status: [Early Stages]

## Introduction
Using data science to predict outcomes in nfl games, player statistics for sports betting and/or fantasy football.

### Methods:
* Web Scraping
* Logistic Regression

### Technologies:
* Python
* BeautifulSoup, selenium
* scikit-learn

## Project Description

The goal of this project is to get familiar with some web scraping libraries, scrape some football statistics from profootballreference.com, do some basic feature engineering and develop a predictive model.

I initially wrote a function to web scrape from a specific type of pfr page for simple win/loss stats for the 2020 season using selenium and a headless chrome browser. This was used to generate the input file scores2020.csv. I accidentaly deleted my selenium function and am in the process of trying to rebuild it using beeautiful soup as I have realized it is unecessary to use selenium for the basic html that is being used by pfr.

So far, I used win/loss and pts for/against to generate a few basic features with with to predict a game outcome. I attempted to train a logistic regression model on the w/l data prior to week 11 of the nfl season where I then attempted to predict outcomes for week 12. The results were quite poor however, the goal was just to use scikit-learn logistic regression for the first time. Next steps are to scrape more data, engineer some bette features and a better data model for the training data, then I will try and optiomize my logistic regression and test out some other models.

### Inputs:
* [Scrape pfr](https://github.com/mmollico/nfl-data-science/blob/main/scrape_pfr.ipynb)
  * currently rebuilding
* scores_2020.csv

### Notebooks
* [Predict Outcomes](https://github.com/mmollico/nfl-data-science/blob/main/predict_outcomes.ipynb)

