# 🏡 Boston Housing Price Prediction – Log Transformation (bostonT1)

This task uses the classic **Boston Housing dataset** to predict median housing prices (`MEDV`) using **Linear Regression**. A log transformation is applied to the target variable to improve model performance and normalize skewed data.

---

## 📁 Dataset Overview

- File: `Boston-house-price-data.csv`
- Target: `MEDV` – Median value of owner-occupied homes
- Features: Various numeric attributes including crime rate, room count, etc.
- Note: `CHAS` was dropped due to low correlation

---

## 📌 Objectives

- Apply preprocessing and feature scaling
- Use **log-transformed regression** to better fit skewed target
- Evaluate the model using appropriate metrics
- Visualize learning curve to detect underfitting/overfitting

---

## 🧠 ML Workflow Summary

### ✅ Preprocessing
- Removed nulls and duplicates
- Dropped the `CHAS` column (binary, low correlation)
- Scaled features with `StandardScaler`
- Log-transformed target using `np.log1p(MEDV)` to handle skewness

### ✅ Model Training
- Model: **Linear Regression**
- Train/Test Split: 80/20
- Converted predictions back to original scale using `np.expm1()`

### ✅ Evaluation Metrics
- **MSE**: Measures average squared error  
- **MAE**: Measures average absolute error  
- **RMSE**: Interpretable average error  
- **R² Score**: Indicates goodness of fit

| Metric | Value (approx) |
|--------|----------------|
| MSE    | Moderate       |
| MAE    | Low            |
| RMSE   | Low            |
| R²     | ~0.79          |

---

## 📈 Learning Curve

A custom learning curve was plotted:
- Training MSE vs. Test MSE
- Shows model stability and generalization as training size increases

---

## 📉 Correlation Insights

The features with **strongest correlation** with `MEDV`:
- `LSTAT` (negative)
- `RM` (positive)
- `PTRATIO` (negative)

These insights can be used for feature selection or model refinement.

---

## 🛠️ Libraries Used

- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn` (preprocessing, regression, metrics)

---

## 📎 Author

**Salma Azoz**  
🔗 [GitHub Portfolio](https://github.com/Salmaazoz22)

---

## 📝 Notes

- This task is part of my **NTI Machine Learning Internship – July 2025**
- It demonstrates how **log transformation** of the target can stabilize variance and improve regression performance
