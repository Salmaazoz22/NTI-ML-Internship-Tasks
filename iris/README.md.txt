# 🌸 Iris Dataset - Logistic Regression Classifier

This project applies **Logistic Regression** to the classic Iris dataset to classify flower species based on their sepal and petal measurements. It includes preprocessing, visualization, model training, and evaluation using various metrics.

---

## 📁 Dataset

The [Iris dataset](https://scikit-learn.org/stable/auto_examples/datasets/plot_iris_dataset.html) is a multiclass classification dataset with:
- 150 samples
- 4 features: Sepal Length, Sepal Width, Petal Length, Petal Width
- 3 target classes: Setosa, Versicolor, Virginica

---

## 🛠️ Steps Performed

### 1. Data Preprocessing
- Loaded dataset via `sklearn.datasets.load_iris()`
- Converted it to a pandas DataFrame
- Mapped numeric target to class labels
- Checked for nulls and duplicates
- Removed outliers using the IQR method

### 2. Model Training
- Split data into training and testing sets (80/20 stratified)
- Scaled features using `StandardScaler`
- Trained `LogisticRegression` model with `max_iter=200`

### 3. Evaluation Metrics
- Accuracy Score (Train & Test)
- Classification Report with heatmap
- Confusion Matrix
- Predicted Probabilities for each class

### 4. Visualization
- **Classification Report Heatmap**
- **Confusion Matrix**
- **Decision Boundary** plot using:
  - Selected features: `petal length (cm)` & `petal width (cm)`
  - Logistic Regression with `multi_class='ovr'`

---

## 📈 Results

- **Train Accuracy**: ~0.97
- **Test Accuracy**: ~1.00 (depending on random split)
- Petal-based features proved to be most effective for class separation.

---

## 📂 File Structure

```plaintext
├── iris_logistic_regression.ipynb
├── README.md
