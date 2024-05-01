# REAL ESTATE SALES PREDICTION MODEL

## Project Overview

In the fast-paced world of real estate, it's crucial for agencies to provide clients with precise information. Clients, whether they're looking to become homeowners or investors, rely on real estate companies for guidance on important decisions such as pricing, market trends, and property evaluations. To meet this need, real estate agencies can benefit from a sophisticated regression-based tool. This tool uses various property variables like the number of bedrooms, year built, floor count, living area, condition, location, and amenities to accurately predict property prices. By employing regression analysis, agencies can offer clients more precise pricing estimates, leading to better-informed decisions. Ultimately, this tool aims to improve client satisfaction, streamline decision-making processes, and drive success for real estate agencies.


### Business Problem

Real estate experts in King County need help understanding what factors influence property values and market trends. This study aims to analyze property features, locations, buyer preferences, and market changes over time. By gaining insights from this analysis, real estate professionals can make informed decisions about buying, selling, and positioning themselves in the dynamic King County market. The goal is to provide practical advice to help them succeed in this ever-changing real estate landscape.
### The Data Understanding

King County, Washington, situated in the northwest of the United States, is known for its vibrant housing market centered around Seattle. The county has experienced significant growth due to its strong economy and cultural importance, attracting a large number of residents and creating high demand for housing in both urban and suburban areas. Seattle, with its impressive skyline, is especially sought after by tech professionals and city lovers. King County's real estate market is competitive, offering a range of neighborhoods to suit different preferences, from historic areas to modern suburban developments
**Target Variable**

price: Sale price of the house .

**Unique identifier**

id - Unique identifier for a house

**Property Characteristics:**



bathrooms: Number of bathrooms.

sqft_living: Square footage of living space in the home.

sqft_lot: Square footage of the lot.

floors: Number of floors (levels) in the house.

waterfront: Indicates whether the house is on a waterfront (categorical: YES/NO).

view: Quality of view from the house, categorized into various types.

condition: Overall condition of the house, categorized based on maintenance.

grade: Overall grade of the house, reflecting construction and design quality.

Additional Features:
sqft_above: Square footage of house apart from the basement.

sqft_basement: Square footage of the basement.

yr_built: Year when the house was built.

yr_renovated: Year when the house was renovated.

zipcode: ZIP Code of the property.

lat: Latitude coordinate of the property.

long: Longitude coordinate of the property.

sqft_living15: Square footage of interior housing living space for the nearest 15 neighbors.

sqft_lot15: Square footage of the land lots of the nearest 15 neighbors.bedrooms: Number of bedrooms.

bathrooms: Number of bathrooms.

sqft_living: Square footage of living space in the home.

sqft_lot: Square footage of the lot.

floors: Number of floors (levels) in the house.

waterfront: Indicates whether the house is on a waterfront (categorical: YES/NO).

view: Quality of view from the house, categorized into various types.

condition: Overall condition of the house, categorized based on maintenance.

grade: Overall grade of the house, reflecting construction and design quality.

**Additional Features:**

sqft_above: Square footage of house apart from the basement.

sqft_basement: Square footage of the basement.

yr_built: Year when the house was built.

yr_renovated: Year when the house was renovated.

zipcode: ZIP Code of the property.

lat: Latitude coordinate of the property.

long: Longitude coordinate of the property.

sqft_living15: Square footage of interior housing living space for the nearest 15 neighbors.

sqft_lot15: Square footage of the land lots of the nearest 15 neighbors.
### Key Points

# **OBJECTIVES**


**Main Objective:**

The primary aim of this project is to develop a predictive regression model to support real estate agencies in advising clients on house prices. This model is intended to anticipate potential changes in property value based on property characteristics, furnishing clients with valuable insights to facilitate informed investment decisions.

Specific Goals:

i). Identification of Key Influencing Factors on House Prices:

Analyze various property features, including bedrooms, bathrooms, and square footage, to determine their impact on sale price. Investigate location-related attributes such as zip codes and geographic coordinates to further comprehend their effect on property prices.

ii). Assessment of Model Performance:

Employ metrics such as mean squared error, R-squared values, and residual analysis to evaluate the model's accuracy in predicting house prices effectively.

iii). Provision of Actionable Recommendations:

Offer practical recommendations to real estate agencies aimed at enhancing profitability and market presence. Utilize insights gleaned from the model to optimize marketing strategies and enhance overall decision-making processes.

# **TABLE OF CONTENT**
1.   Data Preparation
2.   Data cleaning
1.   Exploratory data analysis
2.   Statistical Analysis
1.   Modelling
2.   Regression Results
1.   Conclusion
2.   Recomendations


#**Statistical Analysis**
Statistical analysis plays a crucial role in understanding relationships within datasets, identifying patterns, and gaining insights. In this regression modeling project aimed at predicting property values, several key steps in statistical analysis are essential:

Descriptive Statistics
Correlation matrix
Distribution Analysis
Inferential Statistics using Hypothesis Testing and Analysis of Variance
MultiColinierity
# *Modelling**
Baseline model - simple linear model.
2. log transformation. 
3. Multiple Linear Regression
4. Residual modelling.

# **REGRESSION RESULTS**

**SIMPLE LINEAR REGRESSION** 
Intercept: This is like the starting point or baseline of our predictions. For example, if all other factors were zero, we'd expect the value to be around -44593.95. It's where our line would intersect the y-axis on a graph.

Coefficient: This tells us how much the predicted value changes for each unit increase in the independent variable. In this case, for every one-unit increase in the independent variable, we'd expect the dependent variable to increase by about 281.41.

R-squared: This is a measure of how well our model explains the variation in the data. An R-squared value of 0.49 means that about 49% of the variability in the dependent variable is explained by our model. So, it's doing a decent job, but there's still room for improvement.

Mean Squared Error (MSE): This tells us, on average, how much our predictions differ from the actual values in the training data. Here, the average squared difference is around 68601152192.94, which is quite large but it's relative to the scale of the dependent variable.

Root Mean Squared Error (RMSE): This is just the square root of the MSE. It gives us an idea of the average amount our predictions are off by. Here, it's around 261918.22, which is the typical difference between our predicted values and the actual values in the training data.

Test Set:

R-squared: Similar to the training set, this tells us how well our model explains the variation in the test data. An R-squared value of 0.48 means that about 48% of the variability in the dependent variable is explained by our model when evaluated on the test data.

Mean Squared Error (MSE): This is the average squared difference between our predictions and the actual values in the test data. It's around 68845100756.11, similar to the MSE in the training set.

Root Mean Squared Error (RMSE): Again, this is just the square root of the MSE for the test data. It's around 262383.50, which is the typical difference between our predicted values and the actual values in the test data
Overall
, the model suggests that there is a positive relationship between the independent and dependent variables. However, given the moderate R-squared value and the relatively high MSE and RMSE, it's clear that there may be other factors influencing the dependent variable that are not captured by the model. Further investigation or refinement of the model may be needed to improve its predictive performance.
# ** Multiple Linear Regresion 
![alt text](image-1.png)
# **RESIDUALS**
![alt text](image-3.png)
A p-value of 3.975373048166964e-258, which is extremely close to zero, indicates strong evidence against the null hypothesis of homoscedasticity. In other words, there is a significant presence of heteroscedasticity in your data.

Heteroscedasticity refers to the situation where the variability of a variable is unequal across the range of values of a second variable that predicts it. In the context of regression analysis, it means that the variance of the errors is not constant across observations.
The model identifies the main factors that affect house prices, giving useful advice to real estate companies when they help customers. It's not perfect, but it does an okay job with a 63.1% score. We still need to check if it can predict prices well. However, the model does its job by helping with decisions and making marketing better by using details about houses and the market.

We can see the positive correlation between the house prices and all other features except the year built which indicates a negative correlation.
#**Log transformation**.
Transforming the dependent variable or one or more independent variables can sometimes stabilize the variance. Common transformations include taking the natural logarithm, square root, or reciprocal of the variables.

Log transformation of the multiple linear regression.
![alt text](image-4.png)

![alt text](image-5.png)
The model's residuals are randomly distributed, indicating no systematic bias. The log transformation visualizes residuals and patterns. A horizontal red line suggests linearity and normality are satisfied, but does not provide a definitive answer on model goodness fit and additional technique's could be used to assess the model.
visualization of the positive and negative coefficient variables.
R-squared: The R-squared value indicates that approximately 71.61% of the variance in the target variable (price) is explained by the model.

MSE (Mean Squared Error): The MSE of approximately 37,774,083,176.84 represents the average squared difference between the predicted and actual house prices.

Coefficients: The coefficients represent the estimated effect of each predictor variable on the target variable. For example: The coefficient for const (intercept) is 4987.94. The coefficient for x1 (bathrooms) is 3457.38. The coefficient for x2 (sqft_living) is -16.53. The coefficient for x3 (floors) is -16.98. The coefficient for x4 (waterfront) is -59.75. The coefficient for x5 (condition) is -66.70. The coefficient for x6 (grade) is 21.71. The coefficient for x7 (sqft_basement) is 56.12. The coefficient for x8 (yr_built) and other coefficients follow.

P-values: P-values indicate the statistical significance of the coefficients. A small p-value (typically < 0.05) suggests that the corresponding predictor variable is statistically significant in predicting the target variable. In this summary, some coefficients have p-values less than 0.05, indicating statistical significance, while others do not.

F-statistic: The F-statistic tests the overall significance of the model. A low p-value (typically < 0.05) suggests that at least one of the predictors has a non-zero coefficient, indicating that the model as a whole is statistically significant.

Overall, the summary provides valuable insights into the relationships between the predictor variables and the target variable, as well as the overall goodness-of-fit of the model.

![alt text](image-6.png)
#**REGRESSION Results**

From all the models observed,We can see the positive correlation between the house prices and all other features except the year built which indicates a negative correlation.

Polynomial Regression is the preferred model beacuse from the evaluation it has the highest R-squared value of 0.73

The features below impact price such that an increase will cause an increase in the price of the property. 'bedrooms','bathrooms', 'sqft_living','floors', 'waterfront','view''condition', 'grade', 'sqft_above','sqft_basement', 'yr_renovated', 'sqft_living15','renovated', 'basement'
# **Assumptions**
Linearity: The relationship between the independent variables (predictors) and the dependent variable (response) is linear. This means that a change in the independent variable corresponds to a proportional change in the dependent variable.

Independence of errors: The errors (residuals) from the regression model should be independent of each other. In other words, the residual for one observation should not predict the residual for another observation.

Normality of errors: The errors are normally distributed. This implies that the residuals should follow a normal distribution with a mean of zero.

No perfect multicollinearity: There should be no perfect linear relationship between the independent variables. In other words, no independent variable should be a perfect linear combination of other independent variables.
#**Limitations**
Despite its effectiveness in predicting property prices, the model has several limitations that need to be addressed:

Limited Property Characteristics: The dataset may lack comprehensive property-based characteristics, potentially limiting the model's ability to capture the full range of factors influencing housing prices.

Multicollinearity Concerns: The presence of correlated predictors, such as square footage and number of bedrooms, can introduce multicollinearity issues. This makes it difficult to discern the individual impact of each feature accurately, potentially affecting the model's reliability.

Assumption Violations: Polynomial regression relies on the assumption of linearity between predictors and the target variable. However, in reality, this assumption may not always hold true, leading to biased estimates and less dependable predictions.Also heteroscedasticity was present.

Overfitting Risk: Polynomial regression models, especially those with high degrees, are prone to overfitting. This occurs when the model fits the training data too closely, capturing noise rather than underlying patterns. As a result, the model may struggle to generalize well to unseen data, impacting its predictive performance.

**Limitations**
1.   The dataset could have more property based characteristics
2.   Multicollinearity:The presence of correlated predictors (e.g., square footage and number of bedrooms) can lead to multicollinearity issues, making it challenging to interpret the individual effects of each feature accurately

1. Assumption Violations:Polynomial regression assumes linearity between predictors and the target variable, which may not hold true in all cases. Violations of this assumption can lead to biased estimates and unreliable predictions.
1. Overfitting: Polynomial regression models, particularly those with high degrees, are susceptible to overfitting, where the model fits the training data too closely and may not generalize well to unseen data.
Overall the model was the best fit model for this predictions

# **RECOMENDATIONS**

1.Invest in Larger Properties: Investors seeking maximum returns should focus on larger houses, as there's a positive correlation between total square footage and price. Such properties have the potential for higher profits upon resale or rental.


2.Upgrade Existing Properties: Homeowners can increase their property's value by investing in upgrades that increase square footage, such as adding extra rooms or expanding living spaces.


3.Optimize Bedroom and Bathroom Ratios: It's essential to find the right balance between bedrooms and bathrooms to maximize property value. Consulting with real estate professionals can help determine the optimal ratio based on market trends and buyer preferences.


4.Focus on Quality Over Quantity: Prioritize quality improvements that enhance functionality and aesthetics, such as renovating bathrooms with modern fixtures or upgrading kitchen appliances, to add perceived value to the property.


5.Highlight Features in Listings: Emphasize the number of bedrooms and bathrooms in property listings to attract buyers who prioritize space and convenience. Highlight unique features that add versatility to the property.


6.Differentiate Marketing Strategies: Tailor marketing strategies based on property condition and grade ratings. Highlight the benefits of higher-grade properties to attract premium buyers, while emphasizing renovation potential for properties with lower condition ratings.
# ** Conclusion**

Property Size Matters: There is a clear positive correlation between the size of a property, indicated by total square footage, and its price. Investing in larger properties can potentially yield higher returns for investors and increase market value for homeowners.


Strategic Upgrades Add Value: Upgrading existing properties with strategic renovations and expansions, particularly those that increase square footage, can enhance their market value. Quality improvements that improve functionality and aesthetics are key to maximizing property value.


Balance is Key: While adding extra bedrooms and bathrooms can increase a property's price, there's a point of diminishing returns. It's important to strike a balance between quantity and quality, optimizing the bedroom-to-bathroom ratio to align with market trends and buyer preferences.


Marketing Differentiation is Essential: Tailoring marketing strategies based on property condition and grade ratings is crucial. Highlighting the unique features and benefits of higher-grade properties can attract premium buyers, while emphasizing renovation potential for properties with lower ratings can appeal to savvy investors.
