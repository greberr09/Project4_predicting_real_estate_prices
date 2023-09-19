# Project4_predicting_real_estate_prices

## Overview

This project uses machine learning and deep neural networks to predict real estate prices.   It is written in Python and is run in Google Colab in order to use TensorFlow in that environment.   The project is based on a Kaggle "Getting Started" competition, "House Prices - Advanced Regression Techniques," on advanced linear regression for first-time competitors, and uses Kaggle data.   

## Ames dataset

The primary data are from a widely-known dataset of home prices in Ames, Iowa, collected by Dean De Cook, especially for data science education.  The data can only be used for academic and educational purposes.  The Ames dataset contains 3919 records overall, with 81 columns, about half of which are categorical.  The data are divided into training and testing files.   There are significant differences in the two files, discussed in the exploratory data analysis section.

Ames is a city of 66,424 (as of 2021) and the home of Iowa State University.  Almost half of the population is university students.  Ames is located about 30 miles north of Des Moines, at the intersection of two interstate highways, and lies along the Union Pacific Railway.  A third, smaller state highway runs through the city, as do two small rivers.   The terrain is open and flat.  The summers are very hot, with 85 degree average temperature in July, and the winters are very cold, with an average temperature of 11 degrees in January.  The city has an average rainfall of about 35 inches and an average snowfall of close to 3 feet.  

The genesis of this project was to study the effect of solar panels on housing prices.  Although this initial phase of the longer-term project does not involve solar panels, geographically, the city of Ames is a very good location for solar power.   Because of the temperature extremes in both winter and summer, utility bills are likely to be high year round, but transportation of solar panels to the area would be relatively easy and cheap.  The spread-out nature of the city and the flat terrain are perfect for solar panels.  While the area is not southern California with 360 days of sunshine, at least 2/3 of the days are sunny.  

A number of the dataset features are relevant to the installation of solar panels on a particular house.  Some of the relevant fields include roof type, roofing material, lot shape, lot size, basement square footage, and foundation type, as well as neighborhood.  These were noted for possible use in future predications of whic houses were likely to install solar panels.  In addition, in Ames, one neighborhood in particular is inhabited mostly by students, and is full of restaurants, bars, and shops.  Based on a number of studies, including two large prior studies at the Lawrence Berkely National Laboratory (2015) and Stanford University (2018, updated 2022), demographic factors play a key role in solar adoption.

## Setup Requirements to run the model code

This code requires that anyone running it either to have their device configured to access Google Colab, or to have tensorFlow, scikit Learn, Seaborn and Keras Tuner installed locally, along with Python and Pandas.

Because the Kaggle competition data is available as csv files to download once someone is logged into the ongoing competition, or is available for public download for the closed competition, and is not available by remote API, the code uses Google Drive and mounts the drive in order to upload files to Google Colab.   Every time that the user starts a new session in Google Colab, the drive has to be remounted.  The function to mount the drive will produce popup windows which provide information about what is being made accessible and requesting confirmation.  The function to load data from the mounted drive will produce a popup window requesting a user name and password.

The data can also be downloaded using "kaggle competitions download -c house-prices-advanced-regression-techniques," once the kaggle API packages are installed in the script and a new kaggle API key is obtained and stored in a json file in the local machine.

Google Colab also has methods to attach to a GitHub repository in order to mount data, but as this project is public, and this GitHub repository is public, the data cannot be mounted in that way.   If the code is run locally, the Ames data files also are available to those with a Kaggle account at https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data.   

## Exploratory Data Analysis

The data were examined using pandas functions describe(), info(), nunique(), and value_counts.   The data were also reviewed using Pandas head() and tail() functions.  A list of datafields with descriptions of each field and each category also was provided, in a single text file.  The data contains a very detailed set of features about each building, far beyond other datasets that are limited to square footage, number of bedrooms and bathrooms, and geographic area.  

It was immediately apparent that much of the work for analyzing this dataset would be in determining which features to use, and in cleaning and formatting the data.

While the training data set has 81 columns, the testing dataset has eighty columns.  This is because the test data set does not contain a sale price column.  The two datasets also differ in the numbers of different categories in quite a few of the categorical features, with both training and testing data having categories that are not present in the other data set for multiple features.

Despite the level of detail, manual examination of the columns, prior to any automated processing, makes clear that many of the features are likely to be duplicative or closely correlated.  For instance, there is an overall quality rating, as well as an overall condition rating, with the same ten categories, for each record, as well as separate quality or distinct quality and condition ratings for individual rooms like kitchens.   There are two fields for pool condition and pool quality, and heating and heating quality, as well as multiple fields for basement square footage, finished and unfinished areas, and basement quality.  

Similarly, for the major category of whether a house is single-family or duplex or condo, and how many floors it has, there are three different fields that appear to overlap at least in part.   There are also separate fields for fireplace quality and the number of fireplaces, and garage square footage and the number of cars a garage can hold.   

In addition, the data has fields like "level of functionality" and "low quality finished square feet," that appea to be other forms of quality rating, and multiple fields like "condition1" and condition2", "misc features",  "misc values," or whether the lot backs on an alley, that are not present for many records, and are not likely to be applicable to most of the houses in the city.   

Other features, such as separate fields for the exterior material of the first floor, the second floor, and the garage, are likely to be important to only a small subset of buyers.

On the other hand, the field for street frontage, which is very important for many zoning board decisions, is lacking for most records.

## Data preprocessing

## Initial model configuration


## Model optimization

Rirdge regression was used on the raw data.
## Final Results
