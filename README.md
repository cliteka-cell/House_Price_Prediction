# House Price Prediction

Regression project predicting house sale prices using the Ames Housing Dataset
(2,930 houses, 80 features). Compares four models: Linear Regression, Ridge,
Random Forest, and XGBoost.

## Results
| Model | RMSE | R² |
|-------|------|-----|
| XGBoost | $21,224 | 0.944 |
| Random Forest | $25,594 | 0.918 |
| Ridge Regression | $34,124 | 0.855 |
| Linear Regression | $39,463 | 0.806 |

## What I did
- Handled 27 columns of missing data with context-aware strategies
- Engineered 6 new features (TotalSF, TotalBaths, HouseAge, RemodAge, IsNew, WasRemodeled)
- TotalSF became the 2nd most important feature (12.0% importance)
- Log-transformed target reduced skewness from 1.744 to -0.015
- Evaluated with cross-validation to ensure results aren't from lucky splits

## Tools
Python · Pandas · Scikit-learn · XGBoost · Matplotlib · Seaborn · Google Colab

## Dataset
[Ames Housing Dataset](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)
