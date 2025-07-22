# Salary Data Analysis and Feature Engineering

This project performs exploratory data analysis (EDA), data cleaning, filtering, and feature engineering on a salary dataset containing job titles, salaries, gender, country, education, and experience information.

---

## Project Overview

The analysis covers the following main parts:

- **Part 1: Initial Inspection**
  - Load dataset and display basic info: head, tail, shape, columns.
  - Summary statistics and missing/duplicate value checks.

- **Part 2: Exploration and Filtering**
  - Explore job titles and salaries.
  - Filter data by job title, education, salary thresholds, gender, and experience.
  - Identify high earners and specific subgroups.

- **Part 3: Data Cleaning and Normalization**
  - Convert salary column to numeric.
  - Normalize categorical columns (`Education Level`, `Gender`).
  - Handle missing values by filling with mode or median.
  - Remove extreme salary outliers.
  - Drop columns with excessive missing data.

- **Part 4: Statistical Summaries and Grouping**
  - Compute salary statistics (mean, median, std, percentiles).
  - Average salary by gender.
  - Highest median salaries by job title.
  - Pivot tables by country and education level.
  - Correlation between salary and experience.
  - Salary summaries by education and experience level.

- **Part 5: Advanced Filtering Queries**
  - Salary and experience-based filters (e.g., engineers with less than 5 years experience, high salary earners).
  - Queries on gender, education level, and job title combinations.

- **Part 6: Feature Engineering**
  - Create binary features (`IsSenior`, `IsManager`, `IsTech`).
  - Bin years of experience into levels (`Entry`, `Junior`, `Mid`, `Senior`, `Veteran`).
  - Normalize salary with z-score.
  - Encode gender as binary.
  - Categorize job types (`Engineer`, `Scientist`, `Analyst`, `Other`).
  - Calculate salary per year of experience.
  - One-hot encode `Country`.
  - Normalize years of experience.

---

## Dataset

The dataset `Salary.csv` includes the following key columns:

- `Job Title`: Job role of the employee.
- `Salary`: Annual salary in USD.
- `Gender`: Male/Female.
- `Country`: Country of residence/work.
- `Education Level`: Encoded numeric values representing education attainment.
- `Years of Experience`: Number of years of professional experience.

---

## Usage

1. Upload `Salary.csv` to your working environment.
2. Run the script to perform:
   - Data loading and inspection.
   - Cleaning and normalization.
   - Exploration and filtering.
   - Feature engineering.
3. Analyze outputs including summaries, filtered results, and new engineered features.

---

## Dependencies

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn (optional for scaling)

Install dependencies using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
