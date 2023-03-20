# Appliance-Energy-Prediction
Using Machine Learning Algorithms, Predicting the Energy Used by the Appliance.

Appliances energy prediction involves developing models to predict the energy consumption of household appliances based on various factors such as time of day, usage patterns, weather conditions, and appliance features.

The goal of appliances energy prediction is to help homeowners and utility companies optimize energy usage and reduce costs. By accurately predicting appliance energy consumption, homeowners can adjust their usage patterns and schedule tasks during off-peak hours to take advantage of lower energy rates. Utility companies can also use this data to optimize energy distribution and reduce peak demand, which can lead to more efficient use of resources and a more stable energy grid.

The data set is at 10min for about 4.5 months. The house temperature and humidity conditioned are monitored with a Zigbee Wireless sensor network. Each wireless node transmitted the temperature and humidity conditions around 3.3min. Then the wireless data was averaged for 10 minutes. The energy data was logged every 10 minutes with m-bus energy meters. Weather from the nearest airport weather station(Cheieves Airport Belgium) was downloaded from a public data set from Reliable Prognosis(rp5.ru) and merged together with the experimental data set using the date and time column. Two random variables have been included in the dataset for testing the regression models and to filter out non-predictive attributes. You need to predict the energy use of appliances.
