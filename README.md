# US Crime Data Analysis and Prediction

## Overview

This project focuses on the Crime Data Cleaning process and explores the relationship between various demographic and economic factors with different types of crimes over the past four decades. The analysis includes an in-depth exploratory data analysis (EDA) and predictive modeling using both traditional statistical methods and a neural network.

## Exploratory Data Analysis

### Correlation Heatmap

- Plotted a correlation heatmap to identify relationships between types of crime and demographic factors like per capita income, unemployment rate, population, and the Gini index.

### Research Questions

1. What is the influence of demographic factors like population and unemployment on different types of crime over the past four decades?
2. How have economic metrics like per capita income and the Gini index impacted crime trends over the last four decades?
3. Can we predict crime accurately in upcoming years using demographic and economic factors?

## Causal Inference Analysis

- Conducted causal inference analysis on the US crime dataset.
- Examined the impact of population, unemployment, and per capita income on various crimes.
- Used Treatment Control Split based on the median.
- Null Hypothesis: No effect of unemployment, population, and income on crimes.
- Alternate Hypothesis: Significant effects of these factors on crimes.

### Analysis Results

- Unemployment has a positive Average Treatment Effect (ATE) on crime rate.
- Gini Index has a negligible effect on crime rate, contrary to general assumptions.

## Predictive Modeling

### Feature Standardization

- Applied standardization using z-score normalization to features.

### Regression Model

- Trained a regression model on the standardized features.
- Predictions made on the test set, and performance metrics such as Mean Squared Error (MSE) and R-squared are calculated.
- Rescaled true and predicted values for better interpretation.
- Scatter plots generated to visually compare true and predicted values for each target variable.

### Neural Network Model

- Implemented a two-layer neural network using the Keras Sequential model.
- Used Linear and Relu activation functions between layers.
- Model compiled using the Adam optimizer with a learning rate of 0.001.
- Mean Squared Error (MSE) used as the loss function.
- Trained for 100 epochs with a batch size of 32.
- Achieved a good RMSE of 0.219.

## Time Series Analysis

### SARIMAX Model

- Split data into test and train, keeping the time series intact.
- Scaled data accordingly.
- Trained SARIMAX Model on 35 years of data.
- Model predicted 5 years of data.

### Results

- Berries per capita is best predicted when the exogenous variable income per capita is used.
- Achieved a low RMSE of 0.05631, showing a similar trend to the observed data.
- Time series regression showed even better results than the neural network.

## Conclusion

This project emphasizes thorough data preprocessing, a comprehensive approach to analysis, and a focus on interpretability and evaluation. The results provide insights into the complex relationships between demographic and economic factors and crime rates, offering a foundation for further research and policy considerations.

Feel free to explore the Jupyter notebook for a detailed walkthrough of the analysis and implementation. Your feedback and contributions are welcome!
