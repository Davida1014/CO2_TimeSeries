# Predicting US Carbon Dioxide Emissions Using a Time Series Model
![Stock%20photo](https://github.com/Davida1014/CO2_TimeSeries/blob/main/Images/Stock%20photo.jpg?raw=true)

Cierra Andaur, Davida Rosenstrauch

# Business Problem
Carbon dioxide (CO2) makes up the majority of greenhouse gas emissions worldwide, which are largely responsible for climate change. As the scientific community continues to work toward diminishing future emissions and preventing further damage, understanding past emission patterns is vital to understanding their relationships to climate change. Furthermore, being able to predict future carbon emission levels helps assess risk, garner awareness and funds to aid in preventative measures, and measure success of these measures. As the United States is the top contributor to CO2 emissions worldwide, we have focused our time series analysis on US CO2 emissions per capita.

# The Data
CO2 emission data was downloaded from the Our World in Data CO2 Database (https://ourworldindata.org/co2-emissions). The entire dataset is comprised of 24,017 rows and 38 columns, including data from all countries and continents until 2018. Our univariate time series model is based on 218 observations, namely US emission data from 1800 through 2018.

# Exploratory Data Analysis
The below graph plots total CO2 emissions since 1850 for the entire world as well as United States specfically. Key events are highlighted that may have impacted local increases or decreases in emissions. For example, the end of World War II is preceded by a stark worldwide dip and followed by a steep increase, which is further steepened upon the commonization of commercial air travel. Further, the US curve flattens following the popularization of the term "Global Warming".

(insert image)

The below graph plots the top 50 CO2-emitting countries, as defined by mean emissions since 1950.
(insert image)

Of countries with a mean emission rate of 150 tonnes or more, the threshold indicated above, below are the countries with the top 10 mean emissions per capita.
(insert image)

The data upon which we will be building our model, CO2 emissions per capita in the United States, is presented below.

# Results
The most predictive model on this data was an AR model on logged data. Train and test sets were purposefully split in 2009 os as to account for the 2008 dip in emissions, which may have been due to the stock market crash in that year, in predictions. Our final model had an RMSE of 0.84 and AIC score of -442.84. Below is a graphic representation of predicted versus actual values for our test set.
(insert image)

# Recommendations and Next Steps
It is important to continue to spread awareness of the dangers of climate change and CO2 emissions' impact, as well as to cognizant of financial and sociopolitical events' impacts on CO2 emissions. We would recommend the following steps for further work on this project:
-Apply predictions to the future.
-Analyze and predict CO2 emissions for other high-emitting countries and the world overall.
-Include exogenous variables in a multivariate model, such as population and GDP.
-Utilize neural networks to improve model.
