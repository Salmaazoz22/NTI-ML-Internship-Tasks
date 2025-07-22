# Housing Price Prediction with Polynomial and Regularized Regression Models

This project demonstrates the use of linear, polynomial, and regularized regression models (Ridge, Lasso, ElasticNet) to predict housing prices using a dataset containing various features.

---

## Project Overview

The goal is to predict housing prices using selected features from the dataset, exploring different regression models and tuning hyperparameters to improve performance.

Key steps include:

- Data preprocessing: handling missing values, duplicates, encoding categorical variables, and feature scaling.
- Selecting specific features for modeling.
- Splitting the data into training and test sets with optimal random state selection.
- Training and evaluating:
  - Linear Regression
  - Polynomial Regression (with degree selection)
  - Regularized Regression techniques (Ridge, Lasso, ElasticNet)
- Visualizing learning curves for Polynomial and Ridge regression models.
- Hyperparameter tuning for regularization strength (`alpha`).

---

## Dataset

- The dataset `housing.csv` is loaded and preprocessed.
- Column names are renamed generically as `feature 1`, `feature 2`, ..., for simplicity.
- Missing values and duplicates are removed.
- Categorical variables are encoded using `LabelEncoder`.
- Features are standardized using `StandardScaler`.

---

## Features and Target

- Features used for modeling are columns indexed 5, 10, and 12.
- Target variable is column indexed 13.

---

## Model Details

### 1. Linear Regression

- Baseline model trained on the selected features.
- Best random state for train-test split is searched by maximizing R² score.

### 2. Polynomial Regression

- Polynomial degrees from 1 to 10 are evaluated.
- The best polynomial degree is selected based on test R² score.
- Train and test R² scores for the best polynomial degree are displayed.
- Learning curve is plotted to visualize how model performance scales with training size.

### 3. Regularized Regression

- Models evaluated: Ridge, Lasso, and ElasticNet.
- Alpha (regularization strength) values tested: `[0.0001, 0.001, 0.01, 0.1, 1, 10, 100]`.
- Best alpha is selected based on highest test R².
- Train and test R² and MSE are printed for the best models.
- Learning curve is plotted for Ridge Regression.

---

## Dependencies

Make sure to install the following Python libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
