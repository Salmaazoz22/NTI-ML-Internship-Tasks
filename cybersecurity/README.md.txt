# Cybersecurity Intrusion Detection System 🛡️

This project focuses on detecting potential cyber intrusions using machine learning models like Decision Trees, Logistic Regression, and Support Vector Machines (SVM). The goal is to classify whether a network session indicates an **attack** or **no attack** based on a variety of network behavior features.

## 📂 Dataset

- **Source**: `cybersecurity_intrusion_data.csv`
- Contains both **numerical** and **categorical** features representing user behavior and access patterns.
- Target column: `attack_detected`  
- Irrelevant columns dropped: `session_id`, `unusual_time_access`

---

## 🔍 Key Steps

### ✅ Data Preprocessing

- Handled **missing values**:
  - Numeric → filled with **median**
  - Categorical → filled with **mode**
- Removed **duplicate rows**
- **Outliers** capped using the **IQR method**
- Encoded categorical features using **Label Encoding**
- **StandardScaler** used for normalization

---

### 📊 Exploratory Data Analysis

- Visualized outliers with **boxplots**
- Generated **correlation heatmaps**
- Plotted **confusion matrices** and **learning curves**

---

## 🤖 Models Trained

| Model               | Highlights |
|--------------------|------------|
| **Decision Tree**  | `max_depth=5`, `min_samples_leaf=10` |
| **Logistic Regression** | `penalty='l2'`, `C=3.746`, selected using random search |
| **SVM (RBF Kernel)** | GridSearch optimized `C` and `gamma` |

---

## 📈 Evaluation Metrics

- **Accuracy Score**
- **Classification Report** (Precision, Recall, F1-Score)
- **Confusion Matrix**
- **Learning Curve**

---

## 🧠 Learning Curve (Decision Tree)

Shows how performance varies with training data size to identify overfitting or underfitting.

---

## ✅ Best Parameters (Logistic Regression)

- `C ≈ 3.746`
- `penalty = 'l2'`

---

## 📌 Results Summary

| Model               | Test Accuracy |
|--------------------|----------------|
| Decision Tree       | ~Moderate      |
| Logistic Regression | ✅ Best        |
| SVM                 | Good           |

---

## 📎 Tools & Libraries

- Python, Pandas, NumPy
- Scikit-learn (LogisticRegression, SVC, DecisionTree)
- Matplotlib, Seaborn
- LabelEncoder, StandardScaler

---



