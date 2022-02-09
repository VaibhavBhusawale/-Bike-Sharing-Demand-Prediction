Problem Statement:-	


Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.


The Solution:-


As the first step, perform Data wrangling over the raw data of  Seoul Bikes Sharing (2017 to 2018) further I divided my solution  into Three main parts i.e. Exploratory data analysis, Feature Selection and Engineering and the last work on Various Regression models.
The goal of this project was to build a machine learning model that could make an accurate prediction of how many bikes would be rented based on factors such as day of the week, time of day, temperature, humidity, precipitation, wind, and solar radiation. The dataset had 8,760 observations, with each observation representing one hour of one day. The target variable is ‘Rented Bike Count’ and there were 13 attributes to work with.
In the EDA I focused on the firstly importing required Libraries and cleaning the data set then working on some basic analysis to check stable supply of rental bikes becomes a major concern
1. The number of bikes rented during rainfall/snowfall reduces.
2. The number of bikes rented increases during peak hours.
3. The number of bikes rented during weekends is less compared to weekdays.
4. The number of bikes rented on holidays is less compared to that of working days.
5. The number of bikes rented reduces if there is high humidity.
6. The number of bikes rented on days with high solar radiations is low.
7. The number of bikes rented on average in summer is higher compared to other seasons.

Next step is Feature Selection and Engineering First of all, to avoid any data leakage, I examined the dataset to see if there was any information we wouldn’t necessarily have before making a prediction on bike rental count. Various steps we follow in FSE like Handle Outliers, min_max_scaling, standard scaling, One Hot Encoding, Correlation checking with the help of heat map and VIF we dropping highly correlated features.
The last part of my solution is Regression models. I identified six different regression models I wanted to compare using R-squared as the evaluation metric. For this dataset statistical models were trained with optimized hyper parameters using a repeated cross validation approach and testing set is used for evaluation: (a) Linear Regression (b) Lasso Regression (c) Ridge Regression(d) Decision Tree Regression (e) Light Gradient Boost Regression (f) Random forest. Multiple evaluation indices such as R2, Root Mean Squared Error, Mean Absolute Error and Coefficient of Variation were used to measure the prediction performance of the regression models.Our experiment can help understand what could be the reason for the Regression of such labels by feature selection, data analysis and prediction with machine learning algorithms taking into account previous trends to determine the correct Regression.

