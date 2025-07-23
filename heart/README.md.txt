# ❤️ Heart Disease Prediction - Logistic Regression Classifier

This project uses **Logistic Regression** to predict the presence of heart disease based on patient clinical features. It includes data cleaning, feature scaling, model training, and insightful visualizations.

---

## 📁 Dataset

- The dataset `heart.csv` includes health-related attributes of individuals.
- **Target** column:
  - `1` → Heart disease present
  - `0` → No heart disease

---

## 🔍 Features

- age
- sex
- cp (chest pain type)
- trestbps (resting blood pressure)
- chol (serum cholesterol)
- fbs (fasting blood sugar)
- restecg (resting ECG)
- thalach (maximum heart rate)
- exang (exercise induced angina)
- oldpeak (ST depression)
- slope (slope of peak exercise)
- ca (number of major vessels)
- thal (thalassemia)
- **target** (label)

---

## 🛠️ Workflow Overview

### 1. Data Preprocessing
- Removed duplicate entries
- Removed outliers using **Z-score**
- Displayed a correlation heatmap to assess feature relationships

### 2. Feature Scaling
- Applied `StandardScaler` to normalize features

### 3. Model Training
- Split dataset into training and test sets (80/20)
- Trained `LogisticRegression` with `max_iter=1000`

### 4. Evaluation Metrics
- Accuracy (Train/Test)
- **Classification Report** with precision, recall, and F1-score
- **Heatmap** of classification metrics
- **Confusion Matrix**
- **Learning Curve** to analyze bias/variance

### 5. Decision Boundary
- Used two most influential features: `thalach` & `oldpeak`
- Trained a separate logistic model
- Plotted decision boundary using `DecisionBoundaryDisplay`

---

## 📈 Results

- **Train Accuracy**: ~Your result here
- **Test Accuracy**: ~Your result here

> Strong predictors: `thalach`, `oldpeak`, `cp`

---

## 📦 Requirements

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
