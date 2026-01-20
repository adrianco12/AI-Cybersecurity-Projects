# AI-Powered Cybersecurity Projects in Python

This repository contains a collection of **Python AI projects** focused on practical cybersecurity applications. Each project demonstrates how machine learning and AI techniques can be applied to detect, classify, and analyze security threats.

---

## Projects Overview

## Project 1: Cybersecurity Event Classifier (Logistic Regression)

This project uses **Logistic Regression** to classify cybersecurity events such as normal traffic, phishing, DoS attacks, and malware. The model is trained on numeric features like packet size, failed logins, suspicious port usage, and connection duration.

**How it works:**
- Each feature is assigned a **weight (coefficient)** during training.
- The weighted sum of features is transformed into probabilities using a **sigmoid function**.
- The model predicts the event type with the highest probability.
- Users can input new event data to see predictions and probability scores.

## Project 2: Multi-Cloud User Authentication Analysis (PCA + Clustering + Isolation Forest)

This project analyzes multi-cloud authentication session logs to detect anomalies and uncover patterns in user behavior. It uses **PCA for dimensionality reduction**, **Isolation Forest for anomaly detection**, and **hierarchical clustering/t-SNE** for pattern discovery and visualization.

**How it works:**
- Categorical features (e.g., session type, outcome, IP) are converted to **numeric values**, and all features are standardized.  
- **PCA** reduces high-dimensional session data into 5 principal components, capturing the most important patterns while removing noise.  
- **Isolation Forest** identifies unusual or anomalous sessions based on PCA-transformed data.  
- **Hierarchical clustering** groups similar sessions and highlights clusters with high anomaly ratios.  
- **t-SNE** visualizes sessions in 2D, showing natural clusters and outliers for easy interpretation.  
- Users can explore session clusters, anomaly scores, and unusual authentication patterns for security analysis.


---

## Features

- Implemented in Python using popular libraries like `scikit-learn`, `pandas`, and `matplotlib`.  
- Includes data preprocessing, model training, and evaluation.  
- Visualizations to better understand model decisions and feature importance.  
- Interactive scripts for testing with custom inputs.


