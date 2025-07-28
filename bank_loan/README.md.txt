# 💼 Bank Loan Prediction

This project focuses on predicting whether a customer will accept a **personal loan offer** using machine learning techniques. Two models are implemented and compared: **Decision Tree** and **Random Forest**, both with hyperparameter tuning.

---

## 📂 Dataset Overview

- **Source**: `bankloan.csv`
- **Target Variable**: `Personal.Loan` (Binary: 1 = Loan Accepted, 0 = Not Accepted)
- **Features**:
  - Age
  - Experience
  - Income
  - Family
  - CCAvg (Credit Card Average Spending)
  - Education
  - Mortgage
  - Securities Account
  - CD Account
  - Online
  - Credit Card
- **Dropped Columns**:
  - `ID`
  - `ZIP.Code`

---

## 📊 Project Objectives

- Explore and preprocess the dataset.
- Train and evaluate Decision Tree and Random Forest classifiers.
- Tune model hyperparameters using GridSearchCV.
- Compare model performance.
- Visualize evaluation metrics including confusion matrices.

---

## 🔧 Preprocessing Steps

- Dropped irrelevant columns (`ID`, `ZIP.Code`)
- Checked for null values and duplicates
- Scaled numerical features using `StandardScaler`
- Split dataset into training and testing sets (80/20)

---

## 🤖 Models Used

### ✅ Decision Tree Classifier

- **Tuned Parameters**:
  - `criterion`: `'gini'`, `'entropy'`
  - `max_depth`: `[3, 5, 10, None]`
  - `min_samples_split`: `[2, 5, 10]`

- **Selected Params**:
  - `criterion='entropy'`
  - `max_depth=5`
  - `min_samples_split=2`

---

### ✅ Random Forest Classifier

- **Tuned Parameters**:
  - `n_estimators`: `[50, 100, 200]`
  - `max_depth`: `[5, 10, None]`
  - `min_samples_split`: `[2, 5]`
  - `criterion`: `'gini'`, `'entropy'`

- **Selected Params**:
  - `n_estimators=50`
  - `max_depth=None`
  - `criterion='entropy'`

---

## 📈 Evaluation Metrics

- **Accuracy Score**
- **Classification Report** (Precision, Recall, F1-score)
- **Confusion Matrix Heatmaps**

---

## 🧪 Sample Results (Update with your actual values)

| Model           | Train Accuracy | Test Accuracy |
|----------------|----------------|---------------|
| Decision Tree  | 0.9xx          | 0.8xx         |
| Random Forest  | 0.9xx          | 0.8xx         |

---

## 📊 Visualizations

- Learning Curves
- Confusion Matrices
- Feature importances (if added later)

---

## 🚀 Run the Code

1. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
