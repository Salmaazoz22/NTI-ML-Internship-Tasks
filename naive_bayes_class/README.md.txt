# Naive Bayes Classification on Custom Dataset

This project demonstrates classification using the **Gaussian Naive Bayes** algorithm. The model is trained to predict the target variable from a given dataset, including preprocessing, model evaluation, and visualization.

---

## Dataset

- File: `Naive-Bayes-Classification-Data.csv`
- The last column in the dataset is used as the target variable.
- Features are numerical and scaled before training.

---

## Project Workflow

1. **Data Loading & Inspection**
   - Displays dataset info, checks for missing values and duplicates.

2. **Preprocessing**
   - Separates features and target.
   - Applies `StandardScaler` to normalize features.

3. **Train-Test Split**
   - Splits the dataset into 80% training and 20% testing sets.

4. **Model Training**
   - Uses Gaussian Naive Bayes classifier.
   - Trains on the training data.

5. **Evaluation**
   - Prints training and testing accuracy.
   - Displays detailed classification report (precision, recall, f1-score).
   - Plots learning curve showing model performance vs training size.
   - Visualizes confusion matrix to assess prediction errors.

---

## How to Run

1. Install required packages:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
