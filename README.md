# Glod Price Prediction Using Machine Learning

This Notebook deals with prediction of gold prices. The data contains features regarding the Gold Price Data.

## Objectives
* The main goal of this note book is to build the machine learning system that can predict gold prices based on several other stock prices.
* Obtain data insights using pandas.

## ABOUT THE DATA
* Data Overview: This data file is a Comma separated value(CSV) file format with 2290 rows and 7 columns. It contains 5 columns which are numerical in datatype and one column in Date format. Clearly the data shows value of the variables SPX, GLD, USO, SLV, EUR/USD against the dates in the date column.
* Data Sourse: Link
* Data type available: .csv

```
# Import required libraries
import pandas as pd                                          #Load data & perform basic operations
import numpy as np                                           #Numpy Arrays
import matplotlib.pyplot as plt                              #Matplotlib is a low level graph plotting library in python that serves as a visualization utility.
import seaborn as sns                                        #Seaborn is a library that uses Matplotlib underneath to plot graphs. It will be used to visualize random distributions.
from sklearn.model_selection import train_test_split         #Use to split the original data into training data & test data
from sklearn.ensemble import RandomForestRegressor           #Import Random Forest Regression Model
from sklearn import metrics                                  #Useful for finding performance of model

```
