# Advanced Analytics and AI Modeling

## Introduction

This section presents the advanced analytics and machine learning modeling part of the project. After completing data collection, cleaning, preparation, and visualization, statistical and machine learning techniques were applied to understand unemployment patterns in Jordan.

The project used a complete analytical pipeline that includes regression modeling, validation, multicollinearity testing, residual diagnostics, dimensionality reduction, and clustering.

## Methods Used

The main methods used were:

- Pooled OLS Regression
- Fixed Effects Regression
- Leave-One-Year-Out Validation
- Variance Inflation Factor
- Residual Diagnostics
- Principal Component Analysis
- K-Means Clustering
- Hierarchical Clustering

## Pooled OLS Regression

Pooled Ordinary Least Squares was used as the baseline regression model. It combines all observations into one dataset and estimates one general relationship between unemployment and the selected explanatory variables.

### Pooled OLS Results

| Metric | Value |
|---|---:|
| R² | 0.281 |
| RMSE | 3.586 |
| MAE | 2.955 |

The Pooled OLS model captured some general unemployment patterns, but its explanatory power was limited because it does not control for governorate-specific characteristics.

## Fixed Effects Regression

The Fixed Effects model was used as the main regression model because the dataset is panel data. This model controls for governorate-specific characteristics that may affect unemployment but are not directly measured in the dataset.

### Fixed Effects Results

| Metric | Value |
|---|---:|
| R² | 0.847 |
| RMSE | 1.657 |
| MAE | 1.306 |

The Fixed Effects model performed better than Pooled OLS because it controlled for differences between governorates.

## Leave-One-Year-Out Validation

Leave-One-Year-Out validation was used to test the model’s ability to generalize across unseen years.

In this method, one year was excluded from training, the model was trained on the remaining years, and then the excluded year was predicted.

### LOYO Result

| Metric | Value |
|---|---:|
| R² | 0.692 |
| RMSE | Add from output |
| MAE | Add from output |

The LOYO results showed acceptable temporal generalization, meaning that the model was not only fitting the training data but also had the ability to predict unseen years reasonably well.

## Variance Inflation Factor

VIF was used to check multicollinearity between independent variables.

The VIF equation is:

```text
VIFᵢ = 1 / (1 − Rᵢ²)