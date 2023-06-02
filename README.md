# -Seoul-Bike-Sharing-Demand-Prediction
![image](https://github.com/shubham-bhadouria/-Seoul-Bike-Sharing-Demand-Prediction/assets/103518257/1fe7ec74-bdd0-4cb0-93d1-d4f09eb759d9)
# Problem Statement

Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.

# Data Description:
The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.

# Attribute Information:

• Date : year-month-day

• Rented Bike count - Count of bikes rented at each hour

• Hour - Hour of the day

• Temperature-Temperature in Celsius

• Humidity - %

• Windspeed - m/s

• Visibility - 10m

• Dew point temperature - Celsius

• Solar radiation - MJ/m2

• Rainfall - mm

• Snowfall - cm

• Seasons - Winter, Spring, Summer, Autumn

• Holiday - Holiday/No holiday

• Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)

Data Pipeline:

● Exploratory Data Analysis (EDA): In this part we have done some EDA on the features to see the trend.

● Data Processing: In this part we went through each attributes and encoded the categorical features.

● Model Creation: Finally in this part we created the various models. These various models are being analysed and we tried to study various models so as to get the best performing model for our project.

# Algorithms Used :

Linear Regression

Regularized linear regression:

• Lasso regression

• Ridge regression

Ensemble techniques:

• Decision tree regression

• Random-forest regression

• XG–Boost regression 

# Conclusions:
• No overfitting is seen.

• On comparing all the models, the XG- boost  model has  Adjusted R-squared of 89.4% in test data which is highest among all the models. So, finally, this model is best for predicting the bike rental count on daily basis.

• Functioning days and Seasons were ranked as the most influential variable to predict the rental bike demand at each hour.
