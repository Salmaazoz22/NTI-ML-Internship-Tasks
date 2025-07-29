# Titanic Survival Prediction

This project focuses on predicting passenger survival on the Titanic using machine learning classification techniques.

---

## 🛳 Dataset

- The Titanic dataset includes passenger information such as age, sex, fare, class, family relationships, and embarkation port.
- Data preprocessing involved:
  - Removing duplicates and irrelevant columns (`PassengerId`, `Name`, `Ticket`, `Cabin`)
  - Handling missing values in `Age` and `Embarked` columns
  - Encoding categorical variables (`Sex`, `Embarked`)
  - Creating new features: `FamilySize` and `IsAlone`
  - Removing outliers in `Age` and `Fare` using the IQR method
  - Scaling numeric features (`Age`, `Fare`)

---

## 🔧 Data Preprocessing

- Dropped weak or redundant features based on correlation analysis.
- Final feature set includes numeric and encoded categorical variables.
- Split dataset into training and testing sets (80/20 split).
- Features scaled using `StandardScaler` for better model performance.

---

## 🤖 Models and Techniques

### Logistic Regression

- Trained a logistic regression model to classify survival.
- Evaluated using accuracy, classification report, confusion matrix, and decision boundary visualization.

### Neural Network Classifier

- Built a deep neural network using TensorFlow/Keras with:
  - Multiple dense layers with ReLU activations and dropout for regularization
  - L2 kernel regularization
  - Sigmoid activation for binary classification output
  - Adam optimizer with binary crossentropy loss
  - Early stopping to prevent overfitting

---

## 📊 Model Evaluation

- Metrics reported for both training and test sets:
  - Accuracy
  - Precision, Recall, F1-score (via classification report)
- Visualizations include:
  - Correlation heatmap of features
  - Learning curve for logistic regression accuracy
  - Confusion matrix heatmap
  - Decision boundary plot for logistic regression (Age vs. Fare)
  - Training/validation loss and accuracy curves for the neural network

---

## 📈 Learning Curves and Visualizations

- Learning curve plots demonstrate model generalization with increasing training data.
- Neural network training progress visualized with loss and accuracy plots per epoch.
- Confusion matrix and classification report heatmap provide detailed model diagnostics.

---

## ⚙️ How to Run

1. Install dependencies:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn tensorflow
