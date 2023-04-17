# Appliance-Energy-Prediction

### Introduction
--------------------------------------
Today's word usage of energy is increasing rapidly. Due to more usage of energy in some parts of the world, we are facing a lack of energy and it leads to environmental pollution. In some of the places, we are facing outrageous energy consumption in home appliances, so our main goal in this project is to analyse what the factors are affecting the increasing energy consumption of home appliances, how we can reduce the energy consumption of home appliances and predict energy consumption of appliances by using regression models.

This project will use Python libraries,sklearn, matplotlib, and Seaborn and Eli5 to examine the Telecom dataset through visualizations and graphs.

### Abstract:
----------------------------------------
Prediction of the energy consumed by household appliances is a challenging research topic owing to a transition toward the Internet of Everything. In this study, the energy consumptions of appliances were predicted using a ML model based method, wherein the linear, lasso, ridge, decision tree, random forest, gradient boosting, xgb, adaboost and lgbm regression algorithms were employed. The two objectives of the present study were the maximization of the prediction performance of the algorithms and minimization of the number of selected features. The proposed method was tested on the appliances energy prediction dataset which was downloaded from a public dataset from Reliable Prognosis.

### Dataset information:
----------------------------------------
Below are the info that is available in given dataset- • lights - Energy use of light fixtures in the house • T1 - Temperature in kitchen area • RH_1 - Humidity in kitchen area. • T2- Temperature in living room area. • RH_2 - Humidity in living room area • T3 - Temperature in laundry room area • RH_3 - Humidity in laundry room area • T4 - Temperature in office room • RH_4 - Humidity in office room • T5 - Temperature in bathroom • RH_5 - Humidity in bathroom • T6 - Temperature outside the building • RH_6 - Humidity outside the building • T7 - Temperature in ironing room • RH_7 - Humidity in ironing room • T8 - Temperature in teenager room 2 • RH_8 - Humidity in teenager room 2 • T9 - Temperature in parents room • RH_9 - Humidity in parents room • T_out - Temperature outside (from Chievres weather station ) • Press_mm_hg - Pressure (from Chievres weather station) • RH_out - Humidity outside (from Chievres weather station) • Windspeed - Wind speed (from Chievres weather station) • Visibility - Visibility (from Chievres weather station) • Tdewpoint - Tdewpoint (from Chievres weather station) • rv1 - Random variable 1 • rv2 - Random variable 2 • Date - Date and time format • Appliances - Energy used by appliances (Target Feature)

### Problem Statement:
------------------------------------------
The data set is at 10 min for about 4.5 months. The house temperature and humidity conditions were monitored with a ZigBee wireless sensor network. Each wireless node transmitted the temperature and humidity conditions around 3.3 min. Then, the wireless data was averaged for 10 minutes periods. The energy data was logged every 10 minutes with m-bus energy meters. Weather from the nearest airport weather station (Chievres Airport, Belgium) was downloaded from a public data set from Reliable Prognosis (rp5.ru) and merged together with the experimental data sets using the date and time column. Two random variables have been included in the data set for testing the regression models and to filter out non-predictive attributes (parameters).

### Approaches:
-------------------------------------------
This project aims to predict the energy consumption of home appliances. With the advent of smart homes and the rising need for energy management, existing smart home systems can benefit from accurate prediction. If the energy usage can be predicted for every possible state of appliances, then device control can be optimized for energy savings as well. This is a case of Regression analysis which is part of the Supervised Learning problem. Appliance energy usage is the target variable while sensor data and weather data are the features.

we will draw some insights from data visualization after fetching the information from date column and analysis so that we could get the factors which will affect the output i.e. Energy consumption by appliances which is a major problem and one of the most important concerns for Green Economy.

We will divide this project into five steps for reproductive analysis.

As the first step we will be analyzing, cleaning the dataset which was provided and dropping some unnecessary column.

In the next step we will draw some insights after fetching the other details from date column like hourly, daily and monthly energy consumption. After that we will do Feature selection and Engineering. In FE we will be using VIF and correlation both method for Removing Multicollinearity and drop Some unnecessary column.

Then we will split our data into train and test set after that we used some scaling techniques on train set and after that we prepare our data for feeding to our models for training and analyze the results of all models by comparing with each other. We will select best model among these and proceed with them further.

In the last step we will do hyper-parameter tuning for our topmost model and will see how our model behaves with different parameters. After getting best parameter for our top models we will go for feature importance method and draw the weightage of all features for our top model by using ELi5.

### Tabel of content
----------------------------------------------
Step 1: Importing the Relevant Libraries

Step 2: Data Inspection

Step 3: Exploratory Data Analysis

Step 4: Feature selection

Step 5: Feature engineering

Step 6: Train and Test split

Step 7: Model training

Step 8: Cross validation

Step 9: Model explainability

Step 10: Conclusion

### Conclusion:
--------------------------------------------------------
Tree based models are by far the best performing models while dealing with our dataset because of its ability to stay insulated from the efect of worst performing features.

Based on to our main objective to predict the energy usage by the appliances. Random Forest Regressor is the best performing model when cross validation and hyperparameter tuning is applied we got the best results.

The Model Explainabilty using Eli5 determines which attributes are crucial for predicting the outputs.
