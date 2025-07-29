# Auto MPG Regression Project

This project focuses on predicting **Miles Per Gallon (MPG)** using the **Auto MPG** dataset with multiple regression techniques and a neural network model.

---

## 🚗 Dataset

- The Auto MPG dataset contains various attributes related to car features such as cylinders, displacement, horsepower, weight, acceleration, model year, and origin.
- The dataset was preprocessed by:
  - Removing duplicates
  - Handling missing values (`'?'` replaced and rows dropped)
  - Outlier removal using Z-score filtering on the target variable `mpg`
  - Encoding categorical variables (`origin`) using one-hot encoding
  - Scaling high-value numeric features for better model convergence

---

## 🔧 Data Preprocessing

- Cleaned column names by stripping whitespace.
- Converted horsepower column to numeric, with coercion for invalid values.
- Dropped irrelevant columns like `car name`.
- Standardized features with `StandardScaler`.
- Split data into training and testing sets (80% train, 20% test).

---

## 🧮 Models Evaluated

1. **Linear Regression**  
   Simple baseline model predicting MPG from features.

2. **Ridge Regression**  
   Linear model with L2 regularization to reduce overfitting.

3. **Lasso Regression**  
   Linear model with L1 regularization to promote sparsity in features.

4. **Neural Network Regression**  
   - Built with TensorFlow/Keras  
   - Two hidden layers with LeakyReLU activations and dropout for regularization  
   - L2 kernel regularization on hidden layers  
   - Adam optimizer with early stopping to prevent overfitting  
   - Mean squared error loss and monitoring MSE metric

---

## 📊 Model Evaluation Metrics

For each model, both on training and testing sets:

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- R² Score (Coefficient of Determination)

---

## 📈 Learning Curves

- For classical models (Linear, Ridge, Lasso), learning curves showing training and testing MSE across increasing training set sizes are plotted.
- For the neural network:
  - Loss (MSE) over epochs for training and validation sets is plotted.
  - MSE metric progress tracked during training.

---

## ⚙️ How to Run

1. Install the required packages:
   ```bash
   pip install numpy pandas scikit-learn matplotlib seaborn tensorflow
