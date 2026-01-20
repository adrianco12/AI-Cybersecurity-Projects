# Multi-Cloud User Authentication Analysis

## Overview
This project analyzes multi-cloud user authentication session logs to detect anomalies and uncover patterns in user behavior. By combining dimensionality reduction, clustering, and visualization techniques, the pipeline simplifies complex session data and highlights unusual or suspicious activity.

## How It Works
1. **Data Loading:** Download session log data from Kaggle using `kagglehub` and load into a Pandas DataFrame.  
2. **Preprocessing:** Convert categorical features to numeric values, standardize features, and ensure all relevant metrics are numeric.  
3. **Dimensionality Reduction (PCA):** Reduce high-dimensional session data into 5 principal components, capturing ~86% of variance to remove noise and emphasize meaningful patterns.  
4. **Anomaly Detection (Isolation Forest):** Train an Isolation Forest on PCA-transformed data to identify unusual authentication sessions.  
5. **Hierarchical Clustering:** Group similar sessions, visualize clusters via dendrograms, and identify clusters with high anomaly ratios.  
6. **t-SNE Visualization:** Map sessions into 2D space to visually explore natural clusters, user behavior patterns, and outliers.

## Key Benefits
- Detects unusual authentication behavior for potential security threats.  
- Reduces dimensionality while preserving key information for clustering and anomaly detection.  
- Visualizes complex session patterns for intuitive understanding.  

## Technologies Used
Python, Pandas, NumPy, Scikit-learn, TensorFlow/Keras (optional), Matplotlib, Seaborn, SciPy

