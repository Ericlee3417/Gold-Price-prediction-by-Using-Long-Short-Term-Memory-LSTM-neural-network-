# Gold Price Prediction Project

## Overview

This repository contains the final project for CFRM 521, completed by Eric Lee and Ian Lee. The project aims to predict gold prices using various machine learning models, including regression techniques and deep learning approaches. The goal is to analyze historical data and economic indicators to build models that forecast future gold prices effectively.

## Project Components

### Regression Models (Contributed by Ian Lee)
- **Random Forest Regressor**: Used to predict gold prices based on highly correlated variables such as the USD index (DX-Y.NYB) and platinum prices (PL=F).
- **Linear Regression**: Applied to determine if a simpler, linear model could outperform more complex models in predicting gold prices.

### Neural Networks (Contributed by Eric Lee)
- **Long Short-Term Memory (LSTM) Model**: Eric Lee developed and implemented an LSTM-based deep neural network specifically designed for time series prediction. The LSTM model takes advantage of its ability to remember long-term dependencies, making it well-suited for predicting gold prices. This part of the project involved:
  - Data preprocessing and feature selection.
  - Creating and tuning the LSTM model architecture, including layers and dropout regularization.
  - Evaluating model performance with different sets of input features (all variables, without gold price, and only gold price).

## Data Source

The data used in this project was sourced from Yahoo Finance. It includes various economic indicators and asset prices that potentially influence gold prices. The primary variables considered are:
- **DX-Y.NYB (USD Index)**: Represents the value of the US dollar, which typically has an inverse relationship with gold prices.
- **^GSPC, ^DJI, ^VIX**: Major stock indices and the volatility index, which provide insights into market sentiment and risk appetite.
- **^FTSE, 000001.SS, ^N225**: Stock market indices from Europe, China, and Japan, offering a global perspective.
- **SI=F, PL=F**: Prices of silver and platinum, commodities often correlated with gold.
- **CL=F, ^TNX**: Crude oil prices and the 10-year treasury yield, indicating broader economic conditions.

## Implementation and Results

- **Regression Analysis**: Multiple regression models were tested, including random forest and linear regression. The linear regression model demonstrated the best performance among the regressors, achieving a lower RMSE than simple predictions.
- **LSTM Model**: The LSTM model showed significant promise in predicting gold prices, with the model achieving high accuracy on the test data. Different configurations of the input data were evaluated to determine the optimal feature set for the model.

## Acknowledgments

This project was inspired by various academic and industry resources. The LSTM model and parts of the data preparation were implemented by Eric Lee, with a focus on replicating and optimizing existing techniques rather than claiming originality over the overall methodology. The goal was to explore the application of machine learning in financial forecasting, particularly in predicting the price of gold.
