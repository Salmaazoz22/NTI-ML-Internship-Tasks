# 📊 Naive Bayes Classification Project

This project demonstrates a supervised machine learning pipeline using the **Gaussian Naive Bayes** classifier on a structured dataset. It includes data preprocessing, model training, evaluation, and visualization.

---

## 🗂️ Dataset Info

- **Filename**: `Naive-Bayes-Classification-Data.csv`
- **Type**: Tabular (CSV)
- **Target Variable**: Last column in the dataset
- **Features**: Numerical

---

## 🎯 Objectives

- Preprocess data (scaling, cleaning)
- Train a **Gaussian Naive Bayes** classifier
- Evaluate model performance using accuracy and classification metrics
- Visualize the **learning curve** and **confusion matrix**

---

## 🛠️ Steps & Techniques

### ✅ Preprocessing
- Checked for **missing** and **duplicate** values
- Separated features and target
- Scaled features using **StandardScaler**
- Split into **train/test** sets (80/20)

### ✅ Modeling
- Used **GaussianNB** from `sklearn.naive_bayes`
- Trained model on the training set
- Evaluated accuracy on both training and test data

### ✅ Evaluation
- **Accuracy Score**
- **Classification Report** (Precision, Recall, F1)
- **Confusion Matrix**
- **Learning Curve** to analyze bias-variance tradeoff

---

## 📊 Results

| Metric        | Score (Approx.) |
|---------------|-----------------|
| Train Accuracy | ~0.XX (varies by dataset) |
| Test Accuracy  | ~0.XX (varies by dataset) |

> Exact values depend on your specific dataset content.

---

## 📈 Visualizations

- 📉 **Learning Curve**: Plots training and validation accuracy vs. training size  
- 🔷 **Confusion Matrix**: Visual representation of correct and incorrect predictions

---

## ▶️ How to Run

1. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
