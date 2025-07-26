# Drug Classification using Machine Learning 💊

This project aims to classify patients into the correct **Drug type** based on medical attributes using various machine learning models including **Decision Tree**, **Logistic Regression**, and **Support Vector Machine (SVM)**.

## 📊 Dataset

- **Source**: `drug200.csv`
- Contains information like Age, Sex, Blood Pressure, Cholesterol, and Na-to-K ratio.
- **Target column**: `Drug` (DrugA, DrugB, DrugC, DrugX, etc.)

---

## ⚙️ Preprocessing Steps

- Checked for **null values** and **duplicates**
- Capped **outliers** using the **IQR** method
- Encoded **categorical features** using `LabelEncoder`
- Normalized numeric features using `StandardScaler`
- Split into **Train/Test** sets (80%/20%)

---

## 📈 Models Trained

| Model                | Description |
|---------------------|-------------|
| **Decision Tree**    | `max_depth=5`, `min_samples_leaf=5` |
| **Logistic Regression** | `C=0.1`, `penalty='l2'`, `max_iter=2000` |
| **Support Vector Machine (SVM)** | Tuned with GridSearch (`linear` kernel, `C=10`) |

---

## 🔍 Model Evaluation

Each model was evaluated using:

- **Training & Testing Accuracy**
- **Classification Report** (Precision, Recall, F1-Score)
- **Confusion Matrix**
- **Learning Curve** (for Decision Tree)
- **Decision Tree Visualization** using `plot_tree`

---

## 🧪 Results Summary

| Model                | Training Accuracy | Testing Accuracy |
|---------------------|-------------------|------------------|
| Decision Tree        | ~High             | ~Good            |
| Logistic Regression  | ~High             | ~Good            |
| SVM (Linear Kernel)  | ✅ Best Overall    | ✅ Best Overall   |

> 🎯 SVM with linear kernel performed best after tuning hyperparameters via GridSearchCV.

---


