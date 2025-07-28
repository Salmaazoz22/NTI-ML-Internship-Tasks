# 🏦 Bank Customer Churn Prediction (Naive Bayes)

This machine learning project predicts customer churn using the **Naive Bayes algorithm** on a banking dataset. It involves preprocessing, encoding, feature scaling, training a classifier, and evaluating the results through metrics and visualizations.

---

## 📄 Dataset Overview

- **Dataset**: `BankChurners.csv`
- **Target Variable**: `Attrition_Flag` (1 = Attrited Customer, 0 = Existing Customer)
- **Features**: Demographic and transactional data
- **Source**: [Bank Churn Prediction Dataset](https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers)

---

## 🎯 Objectives

- Clean and preprocess data
- Encode categorical and target variables
- Standardize numerical features
- Train a **Gaussian Naive Bayes** model
- Visualize model performance with a **confusion matrix** and **learning curve**

---

## 🛠️ Preprocessing

- Removed ID and irrelevant prediction columns
- Converted `Attrition_Flag` to binary labels (0 or 1)
- Applied **Label Encoding** to categorical features
- Used **StandardScaler** for feature normalization
- Split data into train and test (80/20)

---

## 🤖 Model Used

- **Algorithm**: Gaussian Naive Bayes (`sklearn.naive_bayes.GaussianNB`)
- Simple and efficient probabilistic model based on Bayes’ theorem

---

## 📈 Evaluation Metrics

| Metric          | Score (approx.) |
|-----------------|-----------------|
| Training Accuracy | ~0.87          |
| Testing Accuracy  | ~0.85          |

### ✅ Additional Metrics
- **Classification Report**: Precision, Recall, F1-score
- **Confusion Matrix**
- **Learning Curve**: Shows model generalization over increasing data sizes

---

## 📊 Visualizations

- 📚 **Learning Curve**: Displays how accuracy evolves as training data increases
- 🔵 **Confusion Matrix**: Highlights correct vs incorrect classifications

---

## ▶️ How to Run

1. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
