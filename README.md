# Linear Regression Assignment
> In order to predict the demand for shared bikes, we had to create a multivariate linear regression model for this programming project. 


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information

- A bike-sharing system is a service that makes bikes available to people for short-term, shared use that can be paid for or provided for free. Many bike share programmes enable users to pick up a bike from a "dock," which is typically computer-controlled and where they enter their payment details to have the bike unlocked. Then, you can return this bike to a different system-affiliated dock.

### Problem Statement

- The ongoing Corona pandemic has recently caused a US bike-sharing company, BoomBikes, to experience significant drops in income. In the current market environment, it is extremely difficult for the organisation to remain viable. It has therefore made the conscious decision to develop a business plan that will enable it to increase revenue as soon as the ongoing lockdown ends and the economy returns to a healthy state.

BoomBikes hopes to understand how people will feel about shared bikes when the current Covid-19-related nationwide quarantine situation ends in this effort. They have planned this in order to differentiate themselves from other service providers and be ready to meet people's requirements when everything improves.

### Business Goals
- With the available independent variables, we must model the demand for shared bikes. The management will use it to determine precisely how the needs change with changing features. They can adjust their business approach in accordance with demand levels and client expectations. The model will also help management better grasp the dynamics of demand in a new market.

### About the Data
- The data set used is the day.csv data set. It have 730 rows and 16 columns. Explaining the columns which has been most used for the analysis andmodeling purposes.

1. instant: record index
2. dteday : date
3. season : season (1:spring, 2:summer, 3:fall, 4:winter)
4. yr : year (0: 2018, 1:2019)
5. mnth : month ( 1 to 12)
6. holiday : weather day is a holiday or not
7. weekday : day of the week
8. workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
9. weathersit : 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
10. temp : temperature in Celsius
11. atemp: feeling temperature in Celsius
12. hum: humidity
13. windspeed: wind speed
14. casual: count of casual users
15. registered: count of registered users
16. cnt: count of total rental bikes including both casual and registered
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
1. EDA
- People are most likely to rent bike on holidays.
- People are most likely to rent bike when the weather is weathersit 1 that is when the weather is mostly clear or with few clouds or partly cloudy.
- Around 60% bike rent capacity has been increased from year 2018 to 2019.
- The bike rent capacity increases every fall that is the third season (season 3).
- Derived a variable quarter from the date column and got to know that the bike rent capacity reaches to its peak in every 3rd quarter.
2. ‘Registered’ numerical variable has the highest correlation with the target variable ‘cnt’ having a correlation value of +0.94.
3. I have finalized over Model 4 getting R-squared: 0.842 & Adj. R-squared: 0.837 on training data and R-squared: 0.827 on testing data.
4. I have also create an alternate model using pipeline and column transfer which has achived Test Score of Linear Regression Model: 0.824
 

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- numpy version - 1.22.3
- pandas version - 1.4.2
- matplotlib version - 3.3.2
- seaborn version - 0.11.2
- missingno version - 0.4.2
- plotly version - 5.1.0
- scikit-learn - 0.24.1
- category-encoders - 2.2.2
- statsmodels - 0.14.0
<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
- We have taken the references of data computation methods from some of the python libraries.
1. Numpy: https://numpy.org
2. Pandas: https://pandas.pydata.org
- We have taken the references of data visualization from some of the python libraries.
1. Plotly: https://plotly.com
2. Seaborn: https://seaborn.pydata.org
3. Matplotlib: https://matplotlib.org
- We have taken the references of data modeling from some of the python libraries.
1. scikit-learn: https://scikit-learn.org/stable/
2. category-encoders: https://contrib.scikit-learn.org/category_encoders/
3. statsmodels: https://www.statsmodels.org/stable/index.html 


## Contact
Created by [@ayush10mehta] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
