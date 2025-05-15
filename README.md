#  Credit Card Customer Segmentation Using K-Means Clustering

This project applies **K-Means Clustering** to segment credit card customers based on their behavioral and financial patterns. The aim is to uncover actionable insights to support **targeted marketing, risk analysis, and customer relationship management**.

---

## 📁 Contents

| File Name                        | Description |
|----------------------------------|-------------|
| `CC_dataset.csv`                | Raw dataset downloaded from [Kaggle](https://www.kaggle.com/datasets/arjunbhasin2013/ccdata). |
| `CC_seg_kmeans.ipynb`           | Jupyter Notebook containing all steps of the segmentation process: preprocessing, feature engineering, dimensionality reduction, clustering, and visualization. |
| `Customer_segmentation_report.docx` | Full project report summarizing methods, visualizations, and business insights derived from the clustering. |

---

## 📊 Project Overview

**Goal**: Segment customers into distinct groups based on spending, payment behavior, and credit usage to enable more effective customer strategies.

**Approach**:
- Preprocessing: Handled missing values (KNN Imputer), removed outliers (LOF), and normalized features.
- Feature Engineering: Created behavior-driven features like `BALANCE_TO_LIMIT` and `CASH_ADVANCE_FREQUENCY`.
- Dimensionality Reduction: Used PCA followed by UMAP for visual separation.
- Clustering: Applied KMeans with optimal number of clusters determined via Silhouette Score and Elbow Method.

---

## 🔍 Key Steps

1. **Data Cleaning & Outlier Removal**  
   - Removed duplicates  
   - Imputed missing values using KNN  
   - Removed outliers using Local Outlier Factor  

2. **Feature Engineering**  
   - Constructed domain-specific features to enhance signal  

3. **Dimensionality Reduction**  
   - PCA (95% variance)  
   - UMAP (10D to 2D embedding)  

4. **Clustering (KMeans)**  
   - Evaluated cluster count from K=2 to 10  
   - Finalized on **K = 6** using Elbow and Silhouette methods  

---

## 📌 Results Summary

- Identified **6 distinct customer segments**
- Segmentation revealed behavioral patterns such as:
  - Purchase-focused users
  - Cash-advance-dependent customers
  - Installment users
  - Short-tenure high-activity users

Visualizations include:
- 2D UMAP cluster plots
- Cluster size bar charts
- Cluster profiling based on key features

---

## 💡 Business Insights

Each customer cluster was profiled and mapped to actionable recommendations:
- Loyalty rewards for high-value buyers
- Financial wellness strategies for high-risk cash users
- Installment plan promotions for structured payers
- Onboarding & retention programs for new users

For more details, see the full [`Customer_segmentation_report.docx`](./Customer_segmentation_report.docx).

---
