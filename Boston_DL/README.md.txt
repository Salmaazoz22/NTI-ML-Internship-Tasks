# Boston Housing Price Prediction

This project focuses on predicting housing prices using the **Boston Housing** dataset with various regression techniques and neural networks.

---

## 📊 Dataset

- The dataset contains features related to housing attributes in Boston.
- Features were scaled and preprocessed before training.
- Categorical features were encoded as needed.
- Target variable: Housing prices.

---

## 🔬 Models and Techniques Used

1. **Linear Regression**  
   Basic linear model predicting housing prices.

2. **Polynomial Regression**  
   Used polynomial features (degree = 1 here, which is linear) to capture non-linear relationships.

3. **Regularized Regression**  
   - Ridge Regression (L2 regularization)  
   - Lasso Regression (L1 regularization)  
   - ElasticNet Regression (combined L1 and L2)  

4. **Neural Network Regression**  
   A fully connected deep neural network built with TensorFlow/Keras, using:
   - Dense layers with ReLU activation  
   - Dropout for regularization  
   - L2 kernel regularization option  
   - Early stopping based on validation loss  
   - Custom callback to monitor R² score during training

---

## ⚙️ Preprocessing

- Null and duplicate rows removed.
- Label encoding for categorical variables.
- Feature scaling using `StandardScaler` for numeric features.
- Data split into training and testing sets (around 10.5% test size).

---

## 📈 Evaluation Metrics

- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score (Coefficient of Determination)

---

## 📉 Learning Curves

- Learning curves plotted for polynomial regression and ridge regression to visualize training and validation performance relative to dataset size.
- Training and validation loss and R² plotted during neural network training.

---

## 🧪 How to Run

1. Ensure Python 3.x is installed.
2. Install required packages:
   ```bash
   pip install numpy pandas scikit-learn matplotlib seaborn tensorflow
