# EDA of sars_cov_2 (covid 19) data
This repository is inspored by kaggle covid 19 week 2 challange (https://www.kaggle.com/c/covid19-global-forecasting-week-2).

# data enrichment
The orignal data set only contains number of cases, fatalities and a time stamp. Features like mean humidity, mean wind speed, sun time, latutude, longitude, mean temperature were added based on the time stamps and location through bigquery api. Population density was enriched via the world bank dataset.

![correlation_2](https://user-images.githubusercontent.com/20724609/78664923-9aa2ca00-78f2-11ea-95d7-17a7524148ae.png)
