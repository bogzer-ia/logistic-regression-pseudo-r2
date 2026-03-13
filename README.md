# Pseudo-R² Measures in Logistic Regression

This project investigates several pseudo-R² measures used to evaluate logistic regression models.

Because logistic regression uses maximum likelihood estimation, the classical OLS R² cannot be directly applied. Several alternative measures have been proposed, including McFadden, Cox–Snell, and Nagelkerke R².

## Objective

The goal of this project is to reproduce and evaluate the conclusions of Menard (2000) using simulation.

## Methods

Three datasets (n = 5000) were simulated with different base rates:

- 1%
- 10%
- 50%

A logistic regression model was fitted in each scenario, and several pseudo-R² measures were computed:

- OLS analog R²
- McFadden R²
- Cox–Snell R²
- Nagelkerke R²
- Contingency coefficient
- Predictive efficiency indexes

## Results

The simulations confirm Menard's findings:

- McFadden R² is the most stable measure across different base rates.
- Nagelkerke R² is highly sensitive to prevalence.
- Classification-based indexes are unstable when outcomes are rare.

## Tools

- R
- tidyverse
- ggplot2
- broom

## Reference

Menard, S. (2000). Coefficients of determination for multiple logistic regression analysis. The American Statistician.
