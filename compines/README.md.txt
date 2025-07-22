# Company Profit Prediction with Linear Regression

This project uses a linear regression model to predict company profits based on various expenses and location data.

## About

Using the **1000 Companies** dataset, this model predicts profits by analyzing:
- Research and Development Spend
- Administration Costs
- Marketing Spend
- State (categorical feature)

The project includes data preprocessing (One-Hot Encoding for the state) and model evaluation using test data.

## Features

- Cleans dataset by removing duplicates
- Encodes categorical data with One-Hot Encoding
- Splits data into training and testing sets (80/20)
- Builds a linear regression pipeline for prediction
- Outputs model coefficients and intercept
- Calculates and displays MSE, RMSE, and R² scores
- Visualizes actual vs predicted profits using a scatter plot

## How to Use

1. Upload `1000_Companies.csv` to your working directory.
2. Run the Python script in your preferred environment (Google Colab recommended).
3. View the model’s performance metrics and plot.

## Dependencies

- pandas
- numpy
- matplotlib
- scikit-learn

Install required libraries with:

```bash
pip install pandas numpy matplotlib scikit-learn
