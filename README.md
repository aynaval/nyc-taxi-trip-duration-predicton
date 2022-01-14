* Nyc taxi trip time dataset released by the NYC Taxi and Limousine Commission, which includes pickup time, geo-coordinates, number of passengers, and several other variables. Dataset has 1458644 rows and 11 columns.There were no null values in the dataset. Target was to predict trip duration time as trip duration is a continuous value; it's a supervised regression problem. Target variable has minimum value of 1 sec and max of 4days and highly positively skewed hence log transformation was applied to it, 3 std value is used to remove the outliers. Month, day no, day, hour, minute and second values were extracted from pickup datetime column. Pickup and dropoff coordinates had values which were very far from nyc and hence those outliers were dropped. There were few rows 0 passengers and extreme trip duration time those were considered as outliers and hence dropped. Month and day columns were one hot encoded while numeric columns were min max scaled. Id,dropoff datetime and pickup datetime columns were dropped. 
* Insights from EDA: Most passengers travel along and most of them travel at around 3pm also trip duration time is highest at 3pm. Trip duration time is least from midnight to early morning and passengers travel the most distance. Most passengers prefer to travel during weekdays compared to weekends,with Wednesday being the busiest day. Trips taken in January have the least trip duration time while those in June have the highest. Trip duration has an average of about 4 minutes. 
* Data was split into train and test dataset and was few into various algorithms.Linear regression similar R2 value of 0.48 for both train and test dataset. Lasso and Ridge behaved similarly after tuning hyperparameters. 
----
| Algoritmns        | MSE  | RMSE | R2   | Adjusted R2 |
|-------------------|------|------|------|-------------|
| Linear regression | 0.05 | 0.22 | 0.48 | 0.48        |
| Lasso             | 0.05 | 0.22 | 0.48 | 0.48        |
| Ridge             | 0.05 | 0.22 | 0.48 | 0.48        |
| Decision Tree     | 0.02 | 0.16 | 0.71 | 0.71        |
| XGBoost           | 0.01 | 0.13 | 0.82 | 0.82        |
