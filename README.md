# Multiple Linear Regression Assignment
# Prediction of Bike Sharing Demand
> This Assignment is about finding the important features which impacts the demand of Bike and create multi Linear Regressor to predict future demand.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
#### Background
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands
Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.

#### Business Goal:
You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.

#### Steps for Model Building
1.Reading and Understanding Data
2.Visualising the Data
3.Data Preparation
4.Splitting the Data into Training and Testing Sets
5.Feature Scaling
6.Building the Model
7.Residual Analysis of the train data
8.Making predictions using final model
9.Model Evaluation

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- feature temp and atemp are highly correlated with target variable cnt
- temp and atemp are highly correalted with each other and we dropped one of them. 
- Fall have the highest booking, and spring have the lowest booking. Summer, Fall and Winder are almost closer. That means in Spring bookings are least
- There is noticable increase in bookings from 2018 to 2019
- Booking increase slowly from Jan to July and then starts decreasing (it might be related to seasons)
- There is slight decrease in bookings on holidays
- Weekday mostly not affecting bookings
- Same with Working dat, it does not have much effect
- Weather situation heavily impact the bookings, if weather is clear bookings are more and based on weather conditions it decreases
- Best fit line for regression is:
cnt = 0.244012 + (-0.084523) * holiday + 0.084523 * temp + (-0.084523) * windspeed + (-0.123336) * season_spring + 0.036464 * season_winter + 0.241186 * yr_2019 + 0.058033 * mnth_Sept + (-0.060089) * weathersit_Mist
- All the positive coefficients like temp/season_winter/yr_2019/mnth_Sept indicate that an increase in these values will lead to an increase in the value of cnt.
- At same time all negative coefficients like holiday/windspeed/season_spring/weathersit_Mist indicate that an increase in these values will lead to an decrease in the value of cnt.
- All the negative coefficients indicate that an increase in these values will lead to an decrease in the value of cnt.
- Temp is the most significant with the largest coefficient, which we expected from correlation matrix as well.
- Followed by yr_2019 and mnth_Sept.

Bike rentals is inveresely effected by windspeed and season_spring
The rentals reduce during holidays This indicates that the bike rentals is majorly affected by temperature,season and month.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- numpy- version 1.24.3
- pandas- version 1.5.3
- matplotlib- version 3.7.1
- seaborn- version 0.12.2
- statsmodels- version 0.13.5
- sklearn - 1.2.2

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->




## Contact
Created by [@pujak19a] - feel free to contact me!


