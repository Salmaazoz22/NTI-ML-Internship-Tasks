# 🏘️ Boston Housing Dataset – Regression Analysis (boston2)

This project explores housing price prediction using the **Boston Housing** dataset. It applies regression techniques to predict the **median house value** based on various features such as crime rate, number of rooms, and others.

---

## 📁 Dataset Overview

- Dataset: `boston housing.csv`
- Features: 13 numerical and/or categorical predictors (renamed as `feature 1`, `feature 2`, ..., `feature 14`)
- Target: Last column (likely `MEDV`, the median value of owner-occupied homes)

---

## 📌 Objectives

- Apply feature scaling and encoding to prepare the dataset
- Use regression models to predict housing prices
- Compare linear, polynomial, and regularized regression models
- Visualize model performance with learning curves

---

## 🧠 ML Workflow Summary

### ✅ Data Preprocessing
- Dropped null values and duplicates
- Encoded categorical features using Label Encoding
- Standardized numeric features using `StandardScaler`

### ✅ Modeling Techniques Used

| Model                    | Degree | Description                              |
|--------------------------|--------|------------------------------------------|
| Linear Regression        | 1      | Baseline model with all features         |
| Polynomial Regression    | 1      | Tested with `degree=1` (same as linear)  |
| Ridge Regression         | 1      | Regularized linear regression            |
| Lasso Regression         | 1      | Feature selection via L1 regularization  |
| ElasticNet Regression    | 1      | Hybrid of Ridge & Lasso                  |

### ✅ Evaluation Metrics
- **R² Score**
- **Mean Squared Error (MSE)**
- **Mean Absolute Error (MAE)**
- **Root Mean Squared Error (RMSE)**

---

## 📈 Results (Sample)

| Model              | Test R² Score | Test MSE |
|-------------------|---------------|----------|
| Linear Regression | ~0.73         | Low      |
| Ridge             | ~0.74         | Low      |
| Lasso             | ~0.72         | Low      |
| ElasticNet        | ~0.73         | Low      |

> *Ridge Regression gave slightly better generalization on the test set.*

---

## 📉 Learning Curves

Learning curves were plotted for:
- Polynomial Regression (`degree=1`)
- Ridge Regression (to observe overfitting vs. underfitting)

---

## 🛠️ Libraries Used

- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn` (linear models, metrics, preprocessing, learning_curve)

---

## 📎 Author

**Salma Azoz**  
🔗 [GitHub Portfolio](https://github.com/Salmaazoz22)

---

## 📝 Notes

- This task is part of my **NTI Machine Learning Internship – July 2025**
- It reinforces the use of **regularized regression models** to improve prediction robustness on real-world data

