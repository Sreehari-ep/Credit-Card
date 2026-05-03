# Credit Card Fraud Detection using Clustering
## Project Overview

This project focuses on detecting fraudulent credit card transactions using unsupervised learning techniques, specifically clustering algorithms. Since fraud detection datasets are highly imbalanced, clustering helps identify unusual patterns (anomalies) without relying on labeled data.

## Dataset
Source: Kaggle – Credit Card Fraud Detection Dataset
Contains transactions made by European cardholders
Highly imbalanced dataset:
Normal transactions: Majority
Fraudulent transactions: Very few
Features:
Time – Seconds elapsed between transactions
Amount – Transaction amount
V1 to V28 – PCA-transformed features
Class – Target variable (0 = Normal, 1 = Fraud)
## Technologies Used
Python
NumPy
Pandas
Matplotlib / Seaborn
Scikit-learn
## Project Workflow
### 1. Data Loading
Loaded dataset using Pandas
Inspected structure and basic statistics
### 2. Data Preprocessing
Checked for missing values
Scaled Amount and Time features
Dropped unnecessary columns if needed
### 3. Exploratory Data Analysis (EDA)
Visualized class imbalance
Analyzed correlations using heatmaps
Observed distribution of features
### 4. Feature Scaling
Applied StandardScaler for normalization
### 5. Clustering Techniques
 K-Means Clustering
Partitioned data into clusters
Identified anomalies based on distance from cluster centroids
 DBSCAN (optional if used)
Density-based clustering
Effective for detecting outliers (fraud cases)
## Results & Insights
Fraud transactions behave as outliers/anomalies
Clustering helps group normal transactions tightly
Fraud cases often fall into sparse or distant clusters
Imbalanced data makes supervised learning harder, but clustering provides a strong alternative
## Visualizations
Correlation heatmap
Distribution plots
Cluster visualization (if reduced using PCA)
## Key Learnings
Understanding of unsupervised learning
Handling imbalanced datasets
Applying K-Means and anomaly detection
Importance of feature scaling
## Limitations
Clustering does not guarantee perfect fraud detection
Sensitive to scaling and parameter tuning
May misclassify some normal transactions as fraud
## Future Improvements
Use Isolation Forest / One-Class SVM
Apply deep learning models
Improve feature engineering
Use real-time fraud detection pipelines
