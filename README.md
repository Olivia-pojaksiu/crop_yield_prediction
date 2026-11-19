# Crop Yield Prediction

Predicts crop yield (hg/ha) from country, crop, year, rainfall, pesticides and temperature using Support Vector Regression (SVR).

## Data
Crop Yield Prediction Dataset from Kaggle (yield_df.csv), 28,242 rows. After removing 2,310 duplicate rows, 25,932 rows remained. There were no missing values.

## What I did
- Cleaned the data and one-hot encoded Area (101 countries) and Item (10 crops)
- Split into 80% training and 20% test data
- Scaled the number columns, fitting the scaler on training data only
- Trained an SVR model

## Result
- Default SVR: R² = -0.21
- After also scaling the target (yield) and converting predictions back: R² = 0.963

## Tools
Python, pandas, scikit-learn, Google Colab
