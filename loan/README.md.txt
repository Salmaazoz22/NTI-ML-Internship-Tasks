# 💰 Loan Approval Prediction

This project is part of my NTI Machine Learning Internship and focuses on predicting whether a loan will be approved using classification models such as **Logistic Regression** and **Support Vector Machine (SVM)**.

## 📁 Dataset

- Dataset: `loan.csv`
- Includes customer financial & demographic features like:
  - Gender, Married, Education
  - ApplicantIncome, LoanAmount
  - Credit_History, Property_Area
  - Target: `Loan_Status` (Y/N)

## 🔄 Preprocessing

- Removed unnecessary ID column (`Loan_ID`)
- Handled missing values:
  - Numeric → median
  - Categorical → mode
- Applied **one-hot encoding** for categorical features
- **Outlier capping** using 1st and 99th percentiles
- Encoded target:  
  - `Y → 1`, `N → 0`
- **StandardScaler** used for scaling features
- Visualized correlation and distributions using heatmaps & boxplots

## 📈 Models Used

### 🔹 Logistic Regression

- Used **GridSearchCV** to find best `C` (regularization parameter)
- Evaluated using:
  - Accuracy
  - Learning curves
  - Classification report heatmap
  - Confusion matrix
- Decision boundary visualized using **PCA** (2D)

### 🔹 Support Vector Machine (SVM)

- RBF kernel used
- Hyperparameters (`C`, `gamma`) tuned with **GridSearchCV**
- Compared with manually selected parameters
- Visualized decision boundary using PCA-reduced data

## ✅ Evaluation Metrics

| Metric       | Logistic Regression | SVM (Manual) |
|--------------|---------------------|--------------|
| Train Accuracy | High              | High         |
| Test Accuracy  | Good              | Strong       |
| GridSearchCV   | Used              | Used         |

- Learning curves for performance insights
- Classification report + confusion matrix
- Decision boundaries (PCA-based visualization)

## 📊 Visualization Highlights

- 📦 Boxplots before & after capping
- 🔥 Correlation heatmap
- 🧠 Learning curve for model training behavior
- 🎯 Confusion matrix and classification report
- 🌐 PCA-based decision boundary plots

---

> Developed as part of the NTI ML Internship  
> 📂 Folder: `loan`
