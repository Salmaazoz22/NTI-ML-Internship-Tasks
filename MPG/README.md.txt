# Auto MPG Prediction Using Linear Regression with Log Transformation

This project builds a linear regression model to predict the fuel efficiency (`mpg`) of automobiles using the Auto MPG dataset. It includes data cleaning, preprocessing, feature scaling, and model evaluation with log-transformed target values.

---

## Project Overview

- Load and clean the Auto MPG dataset:
  - Replace missing values (`'?'`) with NaN and remove rows containing missing data.
  - Drop duplicate rows.
  - Remove outliers based on Z-score filtering on the target variable (`mpg`).
  - Encode categorical variables (e.g., `origin`) using one-hot encoding.
  - Scale numerical features with large ranges using standard scaling.

- Transform the target variable (`mpg`) using a log transformation (`log1p`) to stabilize variance and improve model performance.

- Train a linear regression model to predict log-transformed `mpg`.

- Evaluate model performance by:
  - Calculating MSE, MAE, RMSE, and R² on the original scale (by inverting the log transform).
  - Plotting learning curves (train vs test MSE) to understand model learning behavior with different training set sizes.

---

## Dataset

- Source: `auto-mpg.csv`
- Features include displacement, horsepower, weight, acceleration, cylinders, model year, and origin.
- Target variable: miles per gallon (`mpg`).

---

## Preprocessing Steps

1. Missing values handled by replacing `'?'` and dropping incomplete rows.
2. Outliers removed using Z-score filtering on the `mpg` column.
3. Categorical feature `origin` encoded via one-hot encoding.
4. Numerical features with high variance scaled using `StandardScaler`.
5. Target variable `mpg` transformed using `log1p` for regression.

---

## Model Training & Evaluation

- Linear regression model trained on log-transformed target.
- Predictions converted back to original scale using `expm1`.
- Performance metrics reported:
  - Mean Squared Error (MSE)
  - Mean Absolute Error (MAE)
  - Root Mean Squared Error (RMSE)
  - R² score

---

## Learning Curves

- Learning curves plot training and testing MSE as training set size increases.
- Helps diagnose bias-variance tradeoff and model fit quality.

---

## Dependencies

Install necessary libraries with:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn scipy
