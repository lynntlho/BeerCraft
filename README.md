**BrainStation Capstone Project**

**Author: Lynn Ho**

# **Crafting the Perfect Beer:** Predicting Beer Ratings with Sentiment Analysis and Clustering

---

## Introduction

There are thousands of beers and breweries in the market with different product and branding styles. In fact, there are over 100 documented styles of beer from all regions of the world, there is a wide variety of characteristics that can be used to describe and rate a beer, such as alcohol percentage, clarity, colour, and aroma, just to name a few. This project aimed to answer the following business questions:

- How can we use machine learning to predict a beer rating?
- What are the characteristics of a beer that make it more appealing, i.e. get a higher review rating?

By addressing these questions, beer brewers can use the information gathered to understand market trends and craft beers that suit the palates and tastes of consumers, which will ultimately help to increase sales and profit.


## Data Overview

The data used for this project was obtained from BeerAdvocate.com, one of the original beer review websites that started in 1996. The dataset contains 9.07 million beer reviews from 1996 to 2018 and consists of three csv files, one main dataset for the actual beer reviews and two metadata files providing information about the beers: 

- `reviews.csv`
- `beers.csv`
- `breweries.csv`

Due to the large size of the files, they are not loaded in a folder here. However, they can be accessed from links provided in the notebooks.


## Methodology

The machine learning algorithms used for predicting beer ratings were Logistic Regression, Decision Tree, and XGBoost. K-Means Clustering was also used on the vectorized text data to find groups with common features. 

The files in this project are as follows. It is recommended to start with the EDA notebook before moving on to the Classification and Clustering notebooks.

- `1 - beer_cleaning_EDA.ipynb` (background and exploratory data analysis)
- `2 - beer_classification.ipynb` (Logistic Regression, Decision Tree, and XGBoost models)**
- `3 - beer_clustering.ipynb` (K-Means Clustering model)

** this notebook requires a boosting environment that can be set up by running the following commands in the terminal:

1. `conda create -n boosting python=3.8 numpy pandas matplotlib seaborn statsmodels scikit-learn=0.24.1 jupyter jupyterlab`

2. `conda activate boosting`

3. `conda install -c conda-forge xgboost=1.1.1`
