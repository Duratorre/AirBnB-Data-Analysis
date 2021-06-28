# AirBnB Data Analysis

## Table of Contents
1. [ Installation. ](#inst)
2. [ Motivation. ](#motiv)
3. [ Data. ](#data)
4. [ Methodology. ](#method)
5. [ Results. ](#res)
6. [ Licensing, Authors, Acknowledgement. ](#lic)

<a name="inst"></a>
## 1. Installation
In addition to the xgboost library, which needs to be installed, there are no requirements needed to run the code in this repository apart from the Anaconda distribution of Python. The code runs with no issues using the Python versions 3 and later ones.

<a name="motiv"></a>
## 2. Motivation
This project aims at analysing AirBnB data in the cities of Seattle and Boston.
In particular, I will try to answer answering the following questions:

  1. Are there any months during the year when the price of a house increases or decreases? Are there any differences between the two cities?
  2. Are there any differences in average price between different neighbourhoods and home-types in the two cities?
  3. How are house prices and ratings correlated?
  4. How accurately can we predict house prices using machine learning?

<a name="data"></a>
## 3. Data and File Descriptions
Data regarding rent properties in both cities have been provided by AirBnB:
- [Seattle](https://www.kaggle.com/airbnb/seattle/data)
- [Boston](https://www.kaggle.com/airbnb/boston)

The repository is organized as follows:
- the folders Boston and Seattle contain respectively AirBnB data for the
cities of Boston and Seattle;
- inside each folder, the file _calendar.csv_ contains AirBnB data related to
house prices in time, _listings.csv_ contains data regarding all the listings'
characteristics, whereas _reviews.csv_ contains all the reviews for the said houses;
- the file _Analysis.ipynb_ contains all the calculations and analysis done.

<a name="method"></a>
## 4. Methodology

<a name="res"></a>
## 5. Results
Regarding the first question, the data show that for Boston, the least and most expensive months are, respectively, October and December, while for Seattle April is the month with the highest average price per night and January is the one with the lowest average price per night. Although for Boston the situation is not so clear, as September and October appear to be the most expensive months, but there are a lot of listings where the price is at their minimum.

For the second question, in both cities prices of entire homes/apartments are on average higher than prices of private or shared rooms. One thing to notice is that for the neighbourhoods with the most expensive apartments, the same cannot be said for private and shared rooms and vice versa.

About the grade of correlation between prices and ratings, the data show that they are generally not correlated, with ratings and prices that do not show a linear relationship. However, it can be said that for higher prices, ratings tend to be higher, meaning that higher prices are an indication of good ratings.

For the prediction of house prices, three methods are used: Linear Regression, Random Forest Regression and Extreme Gradient Boost. The first method performs worse than the other two, with the two metrics used to measure the goodness of the prediction being the Root-Mean-Square-Error (**RMSE**) and the coefficient of determination (**R^<sup>2/<sup>}**). Between Random Forest and Extreme Gradient Boost, the first performs better on the train set, while the second performs better on the test set.

<a name="lic"></a>
## 6. Licensing, Authors, Acknowledgement
Credit to AirBnB for providing the data. You can find the Licensing for the data and other descriptive information at the Kaggle links available [here](https://www.kaggle.com/airbnb/seattle/data) for the city of Seattle and [here](https://www.kaggle.com/airbnb/boston) for Boston. Code contained in this repository can be used freely.
