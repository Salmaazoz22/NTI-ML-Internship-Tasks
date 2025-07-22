# Titanic Dataset Analysis & Feature Engineering

This project performs an extensive exploratory data analysis (EDA), data cleaning, and feature engineering on the Titanic dataset. It prepares the data for further modeling and analysis by handling missing values, encoding categorical variables, and creating new features.

---

## Project Overview

The workflow covers:

- Initial inspection of the dataset (head, tail, shape, columns, data types, duplicates).
- Data cleaning including handling missing values and duplicates.
- Exploratory analysis with value counts, filtering, and summary statistics.
- Feature engineering to create new meaningful variables that may improve model performance.
- Exporting the cleaned and enriched dataset for downstream tasks.

---

## Dataset

- Source file: `train.csv`
- Key columns: PassengerId, Survived, Pclass, Name, Sex, Age, SibSp, Parch, Ticket, Fare, Cabin, Embarked

---

## Data Cleaning & Preparation

- Duplicate rows are removed.
- Missing values:
  - `'?'` replaced with NaN and rows with missing values handled.
  - Missing `Embarked` values filled with the most common port.
  - Missing `Age` values filled with median age.
- Outliers handled by filtering using Z-score (optional).
- Categorical variables like `Sex` and `Embarked` encoded.
- Unnecessary columns such as `Cabin` dropped due to many missing values.

---

## Exploratory Data Analysis

- Summary statistics (mean, median, std, percentiles) for numerical columns.
- Grouped statistics by Sex, Pclass, and Embarked.
- Correlations calculated between numerical variables.
- Filtering and sorting examples for deeper insight.

---

## Feature Engineering

- **FamilySize**: Sum of siblings/spouses and parents/children aboard plus one (self).
- **IsAlone**: Binary feature indicating if the passenger is alone.
- **Title**: Extracted from passenger names and grouped rare titles.
- **AgeBin**: Age groups categorized into bins like Child, Teen, Adult, MidAge, Senior.
- **FareBin**: Fare categorized into quartiles.
- **Fare_Normalized**: Standardized fare using Z-score.
- **Sex_Code**: Binary encoding for Sex.
- One-hot encoding of **Embarked**.
- **FarePerPerson**: Fare divided by family size.
- Extraction of **LastName** and identification of repeated surnames.

---

## How to Run

1. Upload `train.csv` dataset to your working directory.
2. Run the provided script in Python (Google Colab recommended).
3. Outputs:
   - Prints detailed inspection and statistics to console.
   - Creates new engineered features.
   - Saves cleaned dataset to `titanic_cleaned.csv`.
4. The cleaned CSV file can be downloaded for further use.

---

## Dependencies

Ensure you have the following Python libraries installed:

```bash
pip install pandas numpy matplotlib seaborn

