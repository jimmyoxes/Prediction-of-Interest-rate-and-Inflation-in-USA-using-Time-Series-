# Project: Predicting U.S. Inflation Using Interest Rates (VAR Model)

## Authors: Artur Bruev, Onur Berke Yesil, Othniel Jimmy Adu Mensah

## Overview:
This project applies Vector Autoregression (VAR) modeling to analyze and forecast the relationship between inflation and interest rates in the United States. The model helps uncover dynamic interactions and causality between these key macroeconomic indicators.

## Key Steps & Methods

### Data Preparation:

Filtered and cleaned data to include only U.S. variables.

Removed null values and renamed categories for consistency.

Split dataset into stationary and non-stationary series.

Performed 90/10 train-test split after differencing and stationarity testing.

## Stationarity Testing:

Used the Augmented Dickey-Fuller (ADF) test to ensure all time series were stationary.

Null hypothesis (unit root) rejected when p-value < 0.05.

## Modeling with VAR:

Applied VAR model from statsmodels to capture relationships between inflation and interest rates.

Conducted Impulse Response Function (IRF) analysis to study the effect of shocks across variables.

## Results & Interpretation:

Inflation and interest rate shocks influence each other dynamically over time.

FEVD (Forecast Error Variance Decomposition) showed both series are initially driven by their own shocks, but cross-variable effects grow stronger over time.

Granger Causality Test: Interest rates did not provide strong predictive power for inflation during this period, though both remain interdependent in the broader economic context.

## Tools & Libraries

Python

statsmodels, pandas, numpy, matplotlib

Time series techniques: ADF Test, VAR, IRF, FEVD, Granger Causality

## Key Insights

Inflation and interest rates are mutually influential, with inflation showing greater long-term sensitivity to rate changes.

VAR modeling provides valuable insights for macroeconomic forecasting and policy analysis.
