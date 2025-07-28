# 📱 SMS Spam Detection using KNN and SMOTE

This project aims to classify SMS messages as **spam** or **ham** using **TF-IDF vectorization** and the **K-Nearest Neighbors (KNN)** algorithm. To handle class imbalance, the **SMOTE** technique is applied.

---

## 📂 Dataset Information

- **Source**: `SPAM text message 20170820 - Data.csv`
- **Columns**:
  - `label`: 'spam' or 'ham'
  - `message`: The text of the SMS
- **Target**: `label_encoded` (0 = ham, 1 = spam)

---

## 🔍 Objectives

- Text preprocessing and vectorization using **TF-IDF**
- Apply **Label Encoding** to convert labels into binary format
- Use **SMOTE** for handling class imbalance
- Implement and tune **KNN classifier**
- Evaluate model performance using accuracy, learning curves, and confusion matrix

---

## ⚙️ Preprocessing Steps

- Renamed columns for clarity
- Removed duplicate rows
- Label-encoded the `label` column
- Vectorized the `message` column using **TfidfVectorizer**
- Applied **SMOTE** to oversample the minority class
- Split data into training and testing sets (80/20 split)

---

## 🤖 Model: K-Nearest Neighbors

- **Optimal K** selected using the **Elbow Method**
- **Best K**: `k=3`
- Model trained on **SMOTE-balanced** data

---

## 📈 Evaluation Metrics

| Metric     | Score (Approx) |
|------------|----------------|
| Train Accuracy | 0.98+        |
| Test Accuracy  | 0.95+        |

### ✅ Other Metrics:
- Precision
- Recall
- F1-score
- Confusion Matrix
- Learning Curve

---

## 📊 Visualizations

- 📉 **Elbow Curve** (to select the optimal `k`)
- 📚 **Learning Curve** (train vs validation performance)
- 🔲 **Confusion Matrix** (visual overview of prediction performance)

---

## 🧪 Run the Code

1. Install requirements:
   ```bash
   pip install pandas numpy scikit-learn imbalanced-learn matplotlib seaborn
