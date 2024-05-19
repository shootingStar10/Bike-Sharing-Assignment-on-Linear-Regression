# Assignment on Advanced Regression

## Table of Contents
* [Problem Statement](#problem-statement)
* [Conclusions](#conclusions)
* [Contributer](#contributer)
* [Notes](#notes)

## Problem Statement
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know:

Which variables are significant in predicting the price of a house, and

How well those variables describe the price of a house.

Also, determine the optimal value of lambda for ridge and lasso regression.

## Conclusions

**Que) Which variables are significant in predicting the price of a house?**

**Ans)** 

As per `Lasso` model the top 5 significant variables are as follows
- GrLivArea
- OverallQual_10
- OverallQual_9
- GarageCars
- Neighborhood_NoRidge
        
As per `Ridge` model the top 5 significant variables are as follows
- OverallQual_9
- GrLivArea
- OverallQual_10
- GarageCars
- 2ndFlrSF

**Que) How well those variables describe the price of a house?**

**Ans)** Below table displays the impact of top significant variables on sales price of house

| Feature                   | Ridge Val    | Lasso Val    |
|:-------------------------:|:------------:|:------------:|
|**GrLivArea**              |  0.048032	   |  0.315847    |
|**OverallQual_10**         |  0.047356    |  0.125369    |
|**OverallQual_9**          |  0.053592	   |  0.115666    |
|**GarageCars**             |  0.046469    |  0.069368    |
|**Neighborhood_NoRidge**   |  0.042958    |  0.046216    |
|**2ndFlrSF**               |  0.045832    |  0.008288    |

**Data dictionary of above features**

- `GrLivArea` is Above grade (ground) living area square feet
- `OverallQual` is Rates the overall material and finish of the house (10 is very excellent and 9 is excellent)
- `GarageCars` is Size of garage in car capacity
- `Neighborhood` is Physical locations within Ames city limits (NoRidge is Northridge)
- `2ndFlrSF` is Second floor square feet

**Best alpha value for `Ridge` and `Lasso` model**

- Best alpha for ridge model is 10.0
- Best alpha for lasso model is 0.0002

**Model accuracy**

| Model                     | Train Accuracy    | Test Accuracy    |
|:-------------------------:|:-----------------:|:----------------:|
|**Ridge**                  |  90.04%	        |  85.05%          |
|**Lasso**                  |  90.11%           |  85.77%          |

## Contributer
- Vishrut Mishra

## Notes
If code file is not open then you can view it on nbviewer with following link

https://nbviewer.org/github/shootingStar10/Assignment-on-Advanced-Regression/blob/main/Coding%20Solution.ipynb