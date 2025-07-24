# 🍷 Wine Quality Classification

This project classifies red wine samples as "Good" or "Bad" based on physicochemical properties using **Logistic Regression** and **Support Vector Machines (SVM)**.

## 📁 Dataset

- Source: UCI Wine Quality Dataset
- File: `winequality-red.csv`
- Features include:
  - Fixed acidity, volatile acidity, citric acid, residual sugar, etc.
  - Target: `quality` (score from 0–10)

## 🎯 Goal

Convert the multiclass quality score into a binary classification:
- **Good** (quality ≥ 6)
- **Bad** (quality < 6)

## 🔄 Data Preprocessing

- Removed duplicates
- Handled outliers using **IQR capping** (1.5 × IQR)
- Scaled all features with **StandardScaler**
- Converted target to binary labels ("Good", "Bad")
- Visualized:
  - Boxplots before/after capping
  - Correlation heatmap
  - Class balance using `countplot`

## 🔍 Models Used

### 🔹 Logistic Regression

- Applied with `L2` penalty and tuned `C` value
- Evaluated with:
  - Accuracy (Train & Test)
  - Learning Curve
  - Classification Report
  - Confusion Matrix
  - PCA + Decision Boundary

### 🔹 Support Vector Machine (SVM)

- Kernel: `rbf`
- Hyperparameter tuning via **GridSearchCV**
- Visualized:
  - Confusion matrix
  - PCA-based decision boundary (2D)

## 📊 Evaluation Metrics

| Metric       | Logistic Regression | SVM          |
|--------------|---------------------|--------------|
| Train Accuracy | ✅ High           | ✅ High       |
| Test Accuracy  | ✅ Good           | ✅ Good       |
| Grid Search    | Used              | Used         |
| Visualization  | Heatmaps, PCA     | Heatmaps, PCA|

## 📈 Visualizations

- 🧃 Boxplots (Outlier Inspection)
- 🔥 Correlation Heatmap
- 📚 Learning Curve
- 🎯 Classification Report (Heatmap)
- 🎯 Confusion Matrix
- 🧭 PCA Decision Boundaries (2D)

---

> ✅ Task completed as part of NTI Machine Learning Internship  
> 📁 Folder: `wine`
