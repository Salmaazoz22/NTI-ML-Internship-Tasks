# 🧠 Sonar Rock vs Mine Classification

This project is part of my NTI Machine Learning Internship and focuses on classifying sonar signals as either rocks or mines using **Logistic Regression** and **Support Vector Machine (SVM)**.

## 📁 Dataset

- Dataset: `sonar.csv`
- 60 continuous features representing sonar signal attributes.
- Binary target:  
  - `R` = Rock  
  - `M` = Mine

## 🔄 Preprocessing Steps

- Renamed columns as `F1` to `F60` + `Label`.
- Checked for missing/duplicate values.
- Outliers were **capped** at 1st and 99th percentiles (no rows removed).
- Label encoded:
  - `R → 1` (Rock)
  - `M → 0` (Mine)
- Applied **StandardScaler** for feature scaling.
- Visualized feature correlations with heatmaps.

## 📈 Models Used

### 🔹 Logistic Regression

- Used `GridSearchCV` to tune hyperparameters (C, penalty).
- Plotted:
  - Learning curve
  - Classification heatmap
  - Confusion matrix
- Visualized decision boundaries using **PCA (2D)**.

### 🔹 Support Vector Machine (SVM)

- RBF kernel used with `GridSearchCV`.
- Trained with best hyperparameters and visualized results.
- Also trained a manual SVM model for comparison.
- Visualized decision boundary in 2D (PCA).

## ✅ Evaluation Metrics

- **Accuracy**
- **Classification Report**
- **Confusion Matrix**
- **Learning Curves**
- Visual insights through **boxplots**, **heatmaps**, and **PCA plots**

## 📊 Results Summary

| Model                 | Train Accuracy | Test Accuracy |
|----------------------|----------------|----------------|
| Logistic Regression  | High           | Good generalization |
| SVM (best parameters)| High           | Strong performance |

## 📌 Highlights

- Performed robust preprocessing (outlier capping + scaling).
- Compared Logistic Regression and SVM.
- Visualized decision boundaries using PCA-reduced features.
- Evaluated with detailed metrics and plots.

---

> Developed as part of the NTI ML Internship  
> 📂 Folder: `sonar`
