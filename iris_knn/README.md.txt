# 🌸 Iris Flower Classification using K-Nearest Neighbors (KNN)

This project applies the **K-Nearest Neighbors (KNN)** algorithm to classify iris flower species based on their physical measurements. It demonstrates preprocessing, model training, evaluation, and visualization with the classic Iris dataset.

---

## 📁 Dataset

- **Filename**: `iris.csv`
- **Target Column**: `Species`
- **Features**: `SepalLengthCm`, `SepalWidthCm`, `PetalLengthCm`, `PetalWidthCm`

---

## ⚙️ Project Workflow

1. **Data Preprocessing**
   - Dropped the `Id` column
   - Checked for missing and duplicate values

2. **Feature Scaling**
   - Applied `StandardScaler` to normalize the features

3. **Train-Test Split**
   - 80% training, 20% testing with stratification on the `Species` column

4. **Model Selection**
   - Used the **Elbow Method** to determine the best `k` value
   - Chose `k = 2` for KNN classifier

5. **Model Training and Evaluation**
   - Evaluated the model on training and test data
   - Visualized:
     - Learning Curve
     - Confusion Matrix

---

## 📈 Evaluation

- **Accuracy**:
  - Training Accuracy: ✅
  - Test Accuracy: ✅
- **Metrics**: Precision, Recall, F1-score via `classification_report`
- **Visuals**:
  - Elbow plot for optimal `k`
  - Learning curve
  - Confusion matrix heatmap

---

## 📉 Learning Curve

Shows model performance vs dataset size:
- Helps detect underfitting or overfitting
- Plots training vs validation accuracy

---

## 🔍 Confusion Matrix

Displays predicted vs actual class distribution:
- Useful to assess per-class performance
- Labels: Setosa, Versicolor, Virginica

---

## ▶️ How to Run

1. Install required libraries:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
