# ❤️ Heart Disease Clustering Project

This project explores **unsupervised machine learning** techniques on a heart disease dataset to identify natural clusters of patients using **KMeans**, **Agglomerative Hierarchical Clustering**, and **Bisecting KMeans (Divisive Clustering)**. The project also applies **PCA for visualization** and evaluates clusters using **Silhouette Score** and **Elbow Method**.

---

## 📁 Dataset

- **Filename**: `heart_disease.csv`
- **Type**: Tabular (CSV)
- **Attributes**: Numeric and categorical
- **Target**: Not used (unsupervised)

---

## 📊 Objectives

- Handle missing values and outliers
- Scale numerical data
- Apply multiple clustering algorithms:
  - ✅ KMeans (with optimal k using Silhouette Score)
  - ✅ Agglomerative Clustering (with dendrogram)
  - ✅ Bisecting KMeans (divisive)
- Visualize clusters using **PCA (2D)**
- Compare clustering results

---

## 🛠️ Pipeline Summary

### 🔧 Preprocessing
- Replaced numeric missing values with **median**
- Replaced object/categorical missing values with **mode**
- Capped outliers using the **IQR method**
- Applied **StandardScaler** to normalize data

### 🔍 KMeans Clustering
- Range of k (2 to 10) evaluated
- Chose best `k` using **Silhouette Score**
- Also plotted **Elbow Method** using Inertia

### 🌳 Agglomerative Clustering
- Used **Ward linkage**
- Visualized using a **Dendrogram**
- Extracted flat clusters for comparison

### 🔀 Bisecting KMeans (Divisive)
- Custom implementation using recursive bisection
- Built binary cluster tree and visualized final clusters using PCA

---

## 📈 Visualizations

- 📉 Elbow Curve
- 🔵 Silhouette Scores
- 🌿 Dendrogram for Hierarchical Clustering
- 🧩 PCA 2D scatter plots for:
  - KMeans clusters
  - Bisecting KMeans clusters
  - Agglomerative clusters

---

## ✅ Evaluation Metrics

- **Silhouette Score** for cluster quality
- **Cluster sizes** for distribution overview
- Tree structure of bisecting KMeans

---

## ▶️ How to Run

1. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn scipy
