# ❤️ Heart Disease Prediction using Random Forest

This project uses the **Random Forest Classifier** to predict the presence of heart disease based on clinical features. It includes preprocessing, model training, evaluation with accuracy metrics, learning curves, and a visualization of a decision tree from the forest.

---

## 📁 Dataset

- **Filename**: `heart_disease_data1.csv`
- **Target Column**: `target` (0 = No Heart Disease, 1 = Heart Disease)
- **Features**: Multiple numerical clinical features such as age, cholesterol, blood pressure, etc.

---

## 📊 Project Workflow

1. **Data Cleaning**
   - Removed duplicate records
   - Checked for missing values

2. **Feature Scaling**
   - Standardized the features using `StandardScaler`

3. **Train-Test Split**
   - 80% Training, 20% Testing using `train_test_split`

4. **Model Training**
   - Used `RandomForestClassifier` with:
     - `n_estimators=100`
     - `max_depth=4`
     - `min_samples_split=10`
     - `min_samples_leaf=5`
     - `max_features='sqrt'`

5. **Evaluation**
   - Calculated **accuracy on train and test sets**
   - Visualized **learning curves**
   - Displayed **confusion matrix**
   - Generated **classification report**

6. **Tree Visualization**
   - Visualized one decision tree from the forest (`estimators_[0]`) with `max_depth=3`

---

## 📈 Evaluation Results

- Accuracy metrics: Training and Testing
- Classification report includes precision, recall, F1-score
- Confusion matrix for visual assessment
- Learning curve to diagnose underfitting or overfitting

---

## 📉 Learning Curve

Shows how model performance changes as the size of training data increases:

- Blue: Training Accuracy
- Green: Validation Accuracy
- Shaded area = Standard deviation

---

## 🌲 Decision Tree Visualization

One tree from the Random Forest is plotted to understand how it makes decisions based on features.

---

## ▶️ How to Run

1. Install required packages:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
