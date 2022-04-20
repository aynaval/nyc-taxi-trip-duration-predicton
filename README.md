

# Project Name : NYC Taxi Trip Duration Prediction

#### -- Project Status: Completed

## Project Intro/Objective
The purpose of this project is to predict the trip duration of NYC Taxi Trip> It can benifit both taxi association and customer to plan their trips accordingly.


### Methods Used
* Inferential Statistics
* Machine Learning
* Data Visualization
* Predictive Modeling
* Model explination

### Technologies
 
* Python
* Machine learning algorthmn

## Project Description
* The dataset is based on the 2016 NYC Yellow Cab trip record data made available in Big Query on Google Cloud Platform.The data was originally published by the NYC Taxi and Limousine Commission (TLC). The data was sampled and cleaned for the purposes of this project.
* Dataset has 1458644 rows and 11 columns.
* Data has no null values and no duplicate values.
* EDA is performed on the data to find patterns and insights from the data.
* Following steps are performed in feature engineering : Column creation, Column delection and Transformation.
* Following models have been train on the dataset : Linear regression, Lasso, Ridge, Decision tree and XGboost.
* Winner model is XGboost with R2 value of: 0.80 and RMSE of: 0.13.h
* Shap values have been calculated for XGboost model and most important features are : Pickup_dropoff_diatance, hour, Geo-coridantes and Day.



## Needs of this project

- data exploration/descriptive statistics
- data processing/cleaning
- statistical modeling
- model explainability


## Getting Started

1. Clone this repo 
2. Raw Data is being kept [here](https://drive.google.com/file/d/1XNFAKhJu76q6e3RI54gd3hmP1gjNrigF/view?usp=sharing).
3. Data processing/transformation, EDA, model training and model eplainability scripts are being kept [here](https://github.com/aynaval/nyc-taxi-trip-duration-predicton/blob/main/NYC_Taxi_Trip_Time_Prediction_Capstone_Project.ipynb) with in this repo.



