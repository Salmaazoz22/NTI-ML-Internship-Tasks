# 🩺 Diabetes Prediction - Logistic Regression Classifier

This project uses **Logistic Regression** on a diabetes dataset to predict whether a patient has diabetes based on health-related attributes. The pipeline includes data cleaning, feature scaling, model training, evaluation, and visualizations.

---

## 📁 Dataset

The dataset used is `diabetes2.csv`, which contains medical predictor variables and one target variable (`Outcome`) indicating diabetes presence (1) or absence (0).

---

## 🔍 Features

- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age
- **Outcome** (target)

---

## 🛠️ Workflow Steps

### 1. Data Preprocessing
- Removed duplicate entries
- Detected and removed outliers using the IQR method
- Visualized correlations using a **heatmap**

### 2. Feature Scaling
- Standardized numerical features using `StandardScaler`

### 3. Model Training
- Split data into training and testing sets (80/20)
- Trained `LogisticRegression` with `max_iter=1000`

### 4. Evaluation Metrics
- Accuracy Score (Train & Test)
- Classification Report (printed + heatmap)
- Confusion Matrix
- Learning Curve to detect overfitting/underfitting

### 5. Decision Boundary
- Selected top features based on correlation: `Glucose` and `BMI`
- Trained a separate logistic regression model on these 2 features
- Visualized the **decision boundary** using `DecisionBoundaryDisplay`

---

## 📈 Results

- **Train Accuracy**: ~Your result here
- **Test Accuracy**: ~Your result here

> Key influential features: **Glucose**, **BMI**

---

## 📂 File Structure

```plaintext
├── diabetes2.csv
├── diabetes_logistic_regression.ipynb
└── README.md
