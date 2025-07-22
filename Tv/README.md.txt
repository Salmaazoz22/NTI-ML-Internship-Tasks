# TV Marketing Sales Prediction Using Linear Regression

This project uses a simple linear regression model to predict product sales based on TV advertising budgets. It also visualizes model performance through learning curves.

---

## Project Overview

- Load and explore the TV marketing dataset.
- Perform exploratory data analysis with pairplots and correlation heatmaps.
- Build a linear regression model using `TV` advertising budget as the predictor.
- Evaluate model performance using metrics: MAE, MSE, RMSE, and R² score.
- Plot learning curves showing training and test RMSE for varying training set sizes to assess model learning behavior.

---

## Dataset

- Dataset file: `tvmarketing.csv`
- Features: 
  - `TV` (Advertising budget spent on TV)
  - `Sales` (Product sales)
  
---

## Data Exploration

- Displays basic info and statistics about the dataset.
- Checks for null and duplicate values.
- Visualizes pairwise relationships between features.
- Shows correlation heatmap between variables.

---

## Model Details

- Feature: `TV` advertising budget.
- Target: `Sales`.
- Splits data into train (80%) and test (20%) sets.
- Trains a linear regression model.
- Prints coefficient (weight) and intercept (bias).
- Evaluates model on test data using:
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - R² Score (coefficient of determination)

---

## Learning Curve

- Trains the model on increasing subsets of the training data.
- Calculates RMSE for training and test sets.
- Plots training and test RMSE vs. training set size.
- Helps diagnose underfitting or overfitting.

---

## Dependencies

Install required libraries with:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
