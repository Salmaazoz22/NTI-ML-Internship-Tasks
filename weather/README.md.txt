# 🌦️ Weather Rain Prediction Using Machine Learning

This machine learning project predicts **whether it will rain** or not based on weather conditions. It utilizes models like **Decision Tree**, **Logistic Regression**, and **Support Vector Machine (SVM)** and explores **Optuna hyperparameter tuning** for optimization.

---

## 📁 Dataset Overview

- **File**: `weather_forecast_data.csv`
- **Target column**: `Rain` (`rain` or `no rain`)
- Contains numerical and categorical features like temperature, humidity, wind, etc.

---

## 🧹 Data Preprocessing

✔️ Checked for:
- Missing values  
- Duplicates  
- Outliers using **IQR capping**

✔️ Label encoding for categorical features  
✔️ Feature scaling using `StandardScaler`  

---

## ⚙️ Modeling

### Models Used:
| Model                | Description |
|---------------------|-------------|
| **Decision Tree**    | `max_depth=5`, `min_samples_leaf=10` (also tuned via Optuna) |
| **Logistic Regression** | `C=0.01`, `penalty='l2'` |
| **Support Vector Machine (SVM)** | `kernel='rbf'`, `C=100000`, `gamma=0.0001` |

---

## 🎯 Evaluation Metrics

- **Training and Testing Accuracy**
- **Classification Report** (Precision, Recall, F1-Score)
- **Confusion Matrix**
- **Learning Curve**
- **Decision Tree Plot**

---

## 🔧 Hyperparameter Tuning

Used **Optuna** to optimize Decision Tree parameters:

```python
# Example best params
{
  'max_depth': 5,
  'min_samples_split': 17,
  'min_samples_leaf': 9,
  'criterion': 'entropy'
}
