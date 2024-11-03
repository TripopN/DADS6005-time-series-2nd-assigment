# DADS6005-time-series-2nd-assignment
2nd Assignment - Moving Average &amp; Simple Expo Smoothing.Try to answer what is the best model (lower forecast error).
Here is a config of model fitting.
    1. {'trend': 'add', 'seasonal': 'add'}
    2. {'trend': 'add', 'seasonal': 'mul'}
    3. {'trend': 'mul', 'seasonal': 'add'}
    4. {'trend': 'mul', 'seasonal': 'mul'}
# Interpretaion and Conclusion 
**1. Model (trend=add, seasonal=add): MAE = 200.17, MSE = 61690.11**
This model uses an additive trend and additive seasonality. While it provides a reasonable forecast, its MAE and MSE are higher than some of the other models, indicating that it may not capture the data patterns as well.

**2.Model (trend=add, seasonal=mul): MAE = 222.19, MSE = 73579.47**
This model uses an additive trend and multiplicative seasonality. It performs slightly worse than the first model, with higher MAE and MSE values, indicating that this configuration may not be ideal for your data.

**3.Model (trend=mul, seasonal=add): MAE = 123.92, MSE = 24785.76**
This model uses a multiplicative trend and additive seasonality. It performs significantly better than the additive trend models, with much lower MAE and MSE values. This suggests that using a multiplicative trend helps in capturing the data's underlying pattern more accurately.

**Model (trend=mul, seasonal=mul): MAE = 102.32, MSE = 15637.04**
This model, which uses both multiplicative trend and multiplicative seasonality, has the lowest MAE and MSE among all models, indicating that it provides the most accurate forecast.

**Conclusion**
The model with multiplicative trend and multiplicative seasonality (trend=mul, seasonal=mul) provides the best forecast for your data, as it has the lowest MAE (102.32) and MSE (15637.04). This suggests that both the trend and seasonal components of your data are better represented by a multiplicative approach, which may capture variations in both trend and seasonality more effectively. This model would be the best choice based on your forecast accuracy criteria.
