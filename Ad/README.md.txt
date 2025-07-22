# 📊 Ad Sales Prediction using Regression Models

This task focuses on predicting product **sales** based on advertising budgets spent on **TV**, **Radio**, and **Newspaper** using different regression techniques. The dataset used is `advertising.csv`.

---

## 📁 Dataset Overview

- **Features**:
  - `TV`: Advertising budget on TV
  - `Radio`: Advertising budget on Radio
  - `Newspaper`: Advertising budget on Newspaper

- **Target**:
  - `Sales`: Units sold

---

## 📌 Objectives

- Explore the relationship between ad budgets and sales
- Apply multiple regression techniques:
  - Linear Regression
  - Ridge Regression
  - Lasso Regression
  - ElasticNet Regression
  - Polynomial Regression (Degree 4)
- Compare model performance using R² and MSE
- Visualize learning curves to understand overfitting/underfitting behavior

---

## 🧠 ML Workflow Summary

### ✅ Data Preprocessing
- Handled null values and duplicates
- Standardized features before model training
- Visualized feature correlation using heatmap

### ✅ Model Training & Evaluation
- Trained **Linear Regression** and evaluated performance on training and test sets
- Compared against **Ridge**, **Lasso**, and **ElasticNet** using:
  - R² Score
  - Mean Squared Error (MSE)
  - Learning Curves

### ✅ Polynomial Regression
- Applied 4th-degree polynomial features
- Trained with regularized regression models for better generalization
- Evaluated and visualized performance across training sizes

---

## 📈 Results (Sample)

| Model              | R² (Test) | MSE (Test) |
|-------------------|-----------|------------|
| Linear Regression | ~0.89     | Low        |
| Ridge             | ~0.89     | Low        |
| Lasso             | ~0.89     | Low        |
| ElasticNet        | ~0.89     | Low        |
| Polynomial Ridge  | ~0.95     | Lower      |

> *Polynomial Ridge Regression gave the best generalization performance.*

---

## 📚 Libraries Used

- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn` (regression models, metrics, pipelines)

---

## 📎 Author

**Salma Azoz**  
🔗 [GitHub Portfolio](https://github.com/Salmaazoz22)

---

## 🔍 Notes

- This task is part of my NTI Machine Learning Internship (July 2025).
- The project demonstrates the power of regularization and polynomial feature expansion in improving prediction accuracy.

