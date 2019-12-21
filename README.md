# House-Prices-Advanced-Regression

![House banner](https://github.com/williamhuybui/Iowa-Ames-House-Prices-Prediction/blob/master/Picture/housesbanner.png)

**-- Project Status** Completed

## Project description
If you want to buy a house in Ames, Iowa, give me as much details of your dream house as you can. I will give you the price estimation of the house with a high accuracy

The data consists of 1461 houses with 79 explanatory variables describing (almost) every aspect of residential homes in Ames, Iowa. The feature ranging from the number of bed rooms, living area, or house condition , to lot configuration, neighborhood, or roof style.

## Technology

Python: `pandas`, `numpy`, `sklearn`
Model: blending model of `ElasticNetCV`, `LassoCV`, `RidgeCV`, `XGBRegressor`, `LGBMRegressor`
Visualization: `Tableau`

## Some EDA
1) There are **5 different type of houses: Single-family Detached (1Fam), Two-family Conversion (2FmCo), Duplex (Duplx), Townhouse End Unit (TwnhsE), Townhouse Inside Unit (TwnhsI). The graph shows that Single-family Detached type is the most expensive one 

![House type](https://github.com/williamhuybui/Iowa-Ames-House-Prices-Prediction/blob/master/Picture/house_type_price.PNG)

2) Feature importantce model shows that **`ground living area and overall quality** are two most important feature. Overall quality ranging from 1 to 10 and ground living area is is square feet. The graph shows that there is a linear relationship between these two feature and the average sale price. It also exposes some outliners which were removed later. 

![House type](https://github.com/williamhuybui/Iowa-Ames-House-Prices-Prediction/blob/master/Picture/ground_overall_quality.PNG)

3) After investigaing the **characteristics of the most expensive houses and cheapest houses**, I concluded that the most expensive houses were built in the last 15 years, with living area above 15,000 square feet. The cheapest houses are those that built 60 years ago, with living are less than 9000 square feet.

Expensive houses
![Expensive](https://github.com/williamhuybui/Iowa-Ames-House-Prices-Prediction/blob/master/Picture/SalePriceLivingAreaYear.PNG)

Cheapest houses
![Cheap](https://github.com/williamhuybui/Iowa-Ames-House-Prices-Prediction/blob/master/Picture/poor.PNG)

4) **The garage area and sale price** has partial linear relationship, it has a direct relationship from 0 to 800 square feet of grage area and become volatile for more than 800. This can be explained by the zoning area. A city houses can be more expensive than the rural houses! Also, it is straight forward that the **number of cars that fit in the garage increase** as garage area increase.

![Garage](https://github.com/williamhuybui/Iowa-Ames-House-Prices-Prediction/blob/master/Picture/Garage.PNG))

5) There are only 5 residents that own a pool. The graph shows that having a pool has no relationship with sale price for this area.

![Pool](https://github.com/williamhuybui/Iowa-Ames-House-Prices-Prediction/blob/master/Picture/pool.PNG))

For the interactive EDA version please visit [Tableau Public](https://public.tableau.com/profile/huy.bui#!/vizhome/HousePricesRegression/Story1?publish=yes)

# Challenges
The hardest part of this project is feature engineer. Especially, there are many features that have nan values and categorical data. Filling in the data requires domain knowledge which I had to consult with the community on kaggle discussion.

# Future work
* The model can be reused for a more updated version of the data

* It would be interesting to see how listing prices change over time

# Sources
You can find about everything [here](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/)

# Contact
Email: williamhuybui@gmail.com
