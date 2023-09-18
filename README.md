# Project4_predicting_real_estate_prices

## Overview

This project uses machine learning and deep neural networks to predict real estate prices.   It is written in Python and is run in Google Colab in order to use TensorFlow in that environment.   The project is based on a Kaggle competition, "House Prices - Advanced Regression Techniques," on advanced linear regression for first-time competitors, and uses Kaggle data.   

## Ames dataset

The primary data are from a widely-known dataset of home prices in Ames, Iowa, collected by Dean De Cook, especially for data science education.  The data can only be used for academic and educational purposes.  The Ames dataset contains 3919 records overall, with 57 features. 

Ames is a city of 66,424 (as of 2021) and the home of Iowa State University.  Almost half of the population is university students.  Ames is located about 30 miles north of Des Moines, at the intersection of two interstate highways, and lies along the Union Pacific Railway.  A third, smaller state highway runs through the city, as do two small rivers.   The terrain is open and flat.  The summers are very hot, and the winters are very cold, with an average rainfall of about 35 inches and an average snowfall of close to 3 feet.  

The genesis of this project was to study the effect of solar panels on housing prices.  Although this initial phase of the longer-term project does not involve solar panels, geographically, the city of Ames is a very good location for solar power.   Because of the temperature extremes in both winter and summer, utility bills are likely to be high year round, but transportation of solar panels to the area would be relatively easy and cheap.  The spread-out nature of the city and the flat terrain are perfect for solar panels.  While the area is not southern California with 360 days of sunshine, at least 2/3 of the days are sunny.  

A number in the dataset features are relevant to the installation of solar panels on a particular house.  Some of the relevant fields include roof type, roofing material, lot shape, lot size, basement square footage, and foundation type, as well as neighborhood.  These were noted for possible use in future predications of whic houses were likely to install solar panels.  In addition, in Ames, one neighborhood in particular is inhabited mostly by students, and is full of restaurants, bars, and shops.  Based on a number of studies, including two large prior studies at the Lawrence Berkely National Labortory (2015) and Stanford Univerity (2018, updated 2022), demographic factors play a key role in solar adoption.

# Natinal Dataset

A second data set, with over 904,966 records and ten features, was downloaded from an earler Kaggle competition, from one of the contributors, at https://www.kaggle.com/datasets/ahmedshahriarsakib/usa-real-estate-dataset.   This dataset has very basic information about each house, including the square footage of the house and the lot, and the number of bedrooms and bathrooms, but it was gathered from all over the U.S. and contains three different geographic fields - city, state, and zipcode.

## Setup Requirements to run the model code

This code requires that anyone running it either to have their device configured to access Google Colab, or to have tensorFlow, scikit Learn, Seaborn and Keras Tuner installed locally, along with Python and Pandas.

Because the Kaggle competition data is available as csv files to download once someone is logged into the ongoing competition, or is available for public download for the closed competition, and is not available by remote API, the code uses Google Drive and mounts the drive in order to upload files to Google Colab.   Every time that the user starts a new session in Google Colab, the drive has to be remounted.  The function to mount the drive will produce popup windows which provide information about what is being made accessible and requesting confirmation.  The function to load data from the mounted drive will produce a popup window requesting a user name and password.

Google Colab also has methods to attach to a GitHub repository in order to mount data, but as this project is public, the data cannot be mounted in that way.   In order to run the project as written, reviewers will have to have connected their local evnironment to access Google Colab, and then mount their own local drive.  If the code is run locally, the Ames data files are available to those with a Kaggle account at https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data.   

## Exploratory Data Analysis

## Data preprocessing

## Initial model configuration


## Model optimization

## Final Results
