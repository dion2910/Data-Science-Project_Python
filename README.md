# SC1015-DSAI_Python
NTU SC1015 Project

## About
This is a mini-project for SC1015 (Introduction to Data Science and Artificial Intelligence), we will be focussing on the World Happiness Report 2023.

Singapore was crowned the happiest country in Asia and ranked 25th in the UN's World Happiness Report 2023. Our group decided to dive deeper to find out how Singapore achieved its ranking, through analysing which factors were the most important in deciding happiness and to build a model to predict future happiness scores.

## Contributors

School of Computer Science and Engineering

1. Dion Lim ([@dion2910](https://github.com/dion2910))
2. Marvin ([@Brloom](https://github.com/Brloom))
3. Merwyn Masagca ([@t4bles](https://github.com/t4bles))

## Table of Contents
1. Problem Formulation
2. Models Used
3. Data-driven insights and Recommendations
4. Key learning points
5. References

## Problem Formulation
- To find out which factors are the most important in predicting happiness in a country
- To find and build a model that best predicts happiness in a country

## Models Used
1. Multi-Variate Linear Regression
2. K-fold Multi-Variate Linear Regression
3. Random Forest Regression
4. Ridge Regression

## Data-driven insights and Recommendations
- Random tree regression has the best model amongst the four used, having the best explained varience(R^2) of 0.8692 and the lowest mean squared error(MSE) of 0.1641

|         | Explained Variance   | MSE  |
| ------- | ------- | ------- |
| **Multi Variate Linear Regression** | 0.7132 | 0.3504 |
| **K-fold Multi Variate Linear Regression** | 0.7606 | 0.3029 |
| **Random Forest Regression** | 0.8692 | 0.1641 |
| **Ridge Regression** | 0.7761 | 0.2870 |

- From our analysis of the dataset, we have found that there are 3 variables that best predict the happiness of a country, which are: 
- GDP per capita 
- Social Support  
- Healthy life expectancy at birth

- Hence for our recommendation, Singapore should focus on these 3 variables in order to maximise the happiness of the country and if the Singapore governemnt would want to compare our performance against other countries, Random Forest regression should be used.

## Key learning points
- Applied relavent EDA that helped us in finding useful variables
- Learnt and applied k-fold cross validation for our models, to get better accuracy
- Learnt new regression models (Random Forest Regression and Ridge Regression) to determine which models would give us the best results



## References
1. https://happiness-report.s3.amazonaws.com/2023/WHR+23_Statistical_Appendix.pdf
2. https://scikit-learn.org/stable/modules/cross_validation.html
3. https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html
4. https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.Ridge.html
