# House Price Prediction Analysis Report

[View the Jupyter Notebook](https://github.com/Illias-b/House-Price-Prediction-Notebook.git) 

## Objective

The primary goal was to develop a predictive model to accurately forecast the house price per unit area based on features such as the property's age, proximity to key amenities like MRT stations, the number of convenience stores, and its geographical location.

## Data Analysis and Preprocessing

We began by examining our dataset to identify missing values, understand the distribution of each variable, and explore the relationships between features and the target variable.

### Key Findings

- **Negative Correlation:** The 'Distance to the nearest MRT station' showed a strong negative correlation with the house price per unit area.
- **Positive Correlation:** The 'Number of convenience stores' displayed a moderate positive correlation with house prices.

![image](https://github.com/Illias-b/House-Price-Prediction/assets/33836566/d33a13b6-9825-4e16-84c5-324406393159)

## Feature Selection and Engineering

### Feature Selection

Features with strong correlations were prioritized for the model. Specifically, 'Distance to the nearest MRT station' was identified as a key predictive feature.

![image](https://github.com/Illias-b/House-Price-Prediction/assets/33836566/7f8d3661-e7ef-4953-84a5-2d19665bfdb2)

### Feature Engineering

Attempted to capture more complex relationships through polynomial features up to the 2nd degree. However, this did not significantly impact the model's performance.

## Model Development and Evaluation

Two models were selected for comparison: Linear Regression and Random Forest Regressor. Both models were trained and evaluated using Mean Squared Error (MSE) and R-squared (R²) metrics.

![image](https://github.com/Illias-b/House-Price-Prediction/assets/33836566/54f2e44a-6a23-4dc3-ba38-bb0a491a3e86)


### Model Performance

- **Linear Regression** showed better performance compared to the Random Forest Regressor, with a lower MSE and higher R², indicating its effectiveness in capturing the relationship between the selected features and house prices.
- **Random Forest Regressor** did not show significant improvement even after the addition of polynomial features.

### Interpretation of Results

- The coefficient for 'Distance to the nearest MRT station' in the Linear Regression model suggests a decrease in house prices with increasing distance from MRT stations.

## Conclusions and Recommendations

Linear Regression emerged as the more suitable model for this dataset. The addition of polynomial features did not significantly enhance the Random Forest model's performance.

### Recommendations for Future Work

- Further explore feature engineering, including higher-degree polynomials.
- Optimize the Random Forest model's hyperparameters.
- Evaluate other regression models or ensemble methods.
- Investigate additional features or external data sources to improve model predictions.

This analysis highlights the importance of feature selection, the impact of amenities' proximity on house prices, and the effectiveness of different modeling techniques for this prediction task.
