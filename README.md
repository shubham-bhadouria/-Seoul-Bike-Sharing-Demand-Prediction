# Seoul Bike Sharing Demand Prediction
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

# Project Overview

Bike-sharing, as a new green public transportation mode, has gained popularity in several western cities. Many developing countries are following the western model of Bike Sharing Systems. In this project, we deeply analyze the data of the Seoul bike sharing system and predict the required bike count for each hour to ensure a stable supply of rental bikes.

## Data Preparation and Exploratory Data Analysis (EDA)

To begin, we load the dataset and check for any null values or duplicate rows. Fortunately, our dataset is clean, with no duplicate or null values present.

Next, we conduct Exploratory Data Analysis (EDA) on the dataset. First, we convert the 'Date' column, which is of type 'string', into a datetime format and extract valuable information from it. Then, we explore the relationship between the 'rented bike count' (dependent variable) and all the independent variables. We also examine the distribution of the dependent variable and find that it is not normally distributed. To address this, we apply a square root transformation to achieve a normal distribution.

We further analyze the correlation between variables using a heatmap and observe a high correlation between temperature, dew point temperature, and humidity. To mitigate the issue of multicollinearity, we calculate the Variance Inflation Factor (VIF) score for the independent variables. By removing the dew point temperature column, we successfully reduce the VIF scores of all variables below 10. Additionally, we remove unnecessary columns such as date, year, and weekday.

## Data Encoding and Model Fitting

After extracting the useful data from the dataset, we proceed with data encoding. Categorical variables such as 'Season', 'Holiday', and 'Functional day' are converted into numeric variables, making the dataset ready for fitting into various machine learning models.

We fit the data into five different models: Linear Regression, Lasso Regression, Ridge Regression, Decision Tree Regression, and XGBoost Regression. Among these models, XGBoost Regression performs the best, yielding an adjusted r-square value of 0.894637.

## Conclusion

Based on our analysis, we conclude that XGBoost Regression outperforms all other models in predicting the rental bike demand, with an adjusted r-square value of 0.894637. The most influential variables for predicting the demand at each hour are functioning days and seasons.

This project demonstrates the power of machine learning in accurately predicting the bike count required for a bike sharing system. By leveraging these predictions, operators can ensure a stable supply of rental bikes, thereby promoting eco-friendly transportation and enhancing the overall user experience.

