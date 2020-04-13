# EDA of sars_cov_2 (covid 19) data
This repository is inspired by kaggle covid 19 week 2 challange (https://www.kaggle.com/c/covid19-global-forecasting-week-2).

# data enrichment
The orignal data set only contains number of cases, fatalities and a time stamp. Features like mean humidity, mean wind speed, sun time, latutude, longitude, mean temperature were added based on the time stamps and location through bigquery api. Population density was enriched via the world bank dataset.

# EDA
![correlation_2](https://user-images.githubusercontent.com/20724609/78664923-9aa2ca00-78f2-11ea-95d7-17a7524148ae.png)

This heatmap shows pairwise correlation of all the features. 
very weak negative correlation (~ -0.1) between humidity and number of cases which is in agreement with majority of research taking place (https://www.researchgate.net/publication/339873481_High_Temperature_and_High_Humidity_Reduce_the_Transmission_of_COVID-19).

# future plans
1) Enriching the dataset with additional important features like number of critical patients, ICU beds, ventilators, time stamp of lockdown etc.
2) Forecasting cases and fatalities using RNN's.


# considerations and problems
1) It should be noted that this data is till 21 march, 2020 only.
2) Due to the lack of data about provinces, the location and nature dependent features can be a bit skewed; presently working on a method to normalize these features. 
