###View on website [Link](https://iamswati.github.io/data_analysis_gold_price/)
# Glod Price Prediction Using Machine Learning 

This Notebook deals with prediction of gold prices. The data contains features regarding the Gold Price Data.

## Objectives
* The main goal of this note book is to build the machine learning system that can predict gold prices based on several other stock prices.
* Obtain data insights using pandas.

## ABOUT THE DATA
* **Data Overview:** This data file is a Comma separated value(CSV) file format with 2290 rows and 7 columns. It contains 5 columns which are numerical in datatype and one column in Date format. Clearly the data shows value of the variables SPX, GLD, USO, SLV, EUR/USD against the dates in the date column.
* Data Sourse: [Link](https://www.kaggle.com/altruistdelhite04/gold-price-data)
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


## Data consists of various gold prices for several days in the period of 10 years [Date- MM/DD/YYYY].

* **SPX -** The Standard and Poor's 500, or simply the S&P 500, is a stock market index tracking the performance of 500 large companies listed on stock exchanges in the United States.
* **GLD -** SPDR Gold Shares is part of the SPDR family of exchange-traded funds (ETF) managed and marketed by State Street Global Advisors.
* **USO -** The United States Oil Fund ® LP (USO) is an exchange-traded security whose shares may be purchased and sold on the NYSE Arca.
* **SLV -** The iShares Silver Trust (SLV) is an exchange traded fund (ETF) that tracks the price performance of the underlying holdings in the LMBA Silver Price.
* **EUR/USD -** The Currency Pair EUR/USD is the shortened term for the euro against U.S. dollar pair, or cross for the currencies of the European Union (EU) and the United States (USD). The value of the EUR/USD pair is quoted as 1 euro per x U.S. dollars. For example, if the pair is trading at 1.50, it means it takes 1.5 U.S. dollars to buy 1 euro.


###Correlation

![HeatMap](https://user-images.githubusercontent.com/67102886/129918593-2a5de4b9-b6fb-44b1-8b11-26177e6af892.png)


* Gold (GLD) and silver (SLV) are highly corelated to each other -> 0.9
* Gold (GLD) and Standard and Poor's 500 (SPX) are zero correlation -> 0.0
* Rest features expect gold (GLD) are negative correlated with respect to gold (GLD) -> -0.0 & -0.2


###Checking the distribution of GLD price

![image](https://user-images.githubusercontent.com/67102886/129919722-eaa87a93-4d1d-43a5-bf25-363c014d8bec.png)


