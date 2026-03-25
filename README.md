# Credit Card Default Risk - Segmentation & Analysis

## Overview
Exploratory analysis and risk segmentation on 30,000 credit card clients (UCI dataset) to identify default risk profiles using advanced clustering techniques.

## Objectives
- Identify key factors influencing credit card default behavior
- Segment clients into homogeneous risk profiles
- Identify high-risk groups with elevated default probability
- Compare clustering approaches to select the most reliable method

## Methodology
1. **Data Preparation** — Missing values check, outlier detection (IQR), variable recoding
2. **Univariate & Bivariate Analysis** — Distribution analysis, correlation matrix, PAY_0 vs default
3. **Dimensionality Reduction** — PCA (10 components capturing 90% variance), AFC, MCA
4. **Clustering** — K-Means (k=4) selected via elbow method + silhouette score
5. **Model Comparison** — 3 approaches compared via radar chart (silhouette, Davies-Bouldin, cluster balance)

## Key Results
- Identified a high-risk cluster with **62.6% default rate**
- PCA + K-Means outperformed raw K-Means and 23-variable K-Means
- PAY_0 (payment status) is the strongest predictor of default

## Tools & Libraries
- Python, pandas, NumPy
- scikit-learn (KMeans, StandardScaler)
- Prince (PCA, MCA, AFC)
- Seaborn, Matplotlib

## Dataset
[UCI - Default of Credit Card Clients](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients)
