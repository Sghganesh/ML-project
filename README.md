# Cluster-Based Analysis for Customer Segmentation in E-commerce

This repository contains the code and documentation for the project "Cluster-Based Analysis for Customer Segmentation in E-commerce." The primary goal of this project is to segment customers based on their purchasing behaviors using various clustering techniques, which can then support businesses in crafting targeted marketing strategies.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Project Structure](#project-structure)
4. [Methodology](#methodology)
5. [Clustering Algorithms](#clustering-algorithms)
6. [Results](#results)
7. [Learning Outcomes](#learning-outcomes)
8. [Tools and Libraries](#tools-and-libraries)
9. [Conclusion](#conclusion)

---

## Project Overview

This project aims to analyze customer purchasing behavior using clustering algorithms to create distinct customer groups. The segmentation is based on RFM (Recency, Frequency, and Monetary) metrics and helps reveal patterns in customer behavior, allowing businesses to enhance marketing strategies, customer retention, and engagement.

## Dataset

The dataset used in this project includes over 500,000 transactions from a UK-based online retailer, covering the period from 2010 to 2011. Key attributes include:
- `InvoiceNo`: Unique transaction ID
- `StockCode`: Product ID
- `Quantity`: Units purchased
- `InvoiceDate`: Date of transaction
- `UnitPrice`: Price per unit
- `CustomerID`: Unique customer ID
- `Country`: Customer's location

## Project Structure

- **Data**: Contains the dataset and any derived data files.
- **Code**: Python scripts for data preprocessing, clustering, and evaluation.
- **Results**: Figures, tables, and other outputs from the clustering models.
- **Documentation**: Project report and supplementary information.

## Methodology

1. **Data Preprocessing**:
   - Imputed missing values.
   - Encoded categorical data and standardized numerical features.
2. **Feature Engineering**:
   - Created RFM metrics for clustering.
   - Additional metrics, such as average basket size and average order value, were also calculated.
3. **Dimensionality Reduction**:
   - Applied PCA to visualize clusters effectively.
4. **Clustering**:
   - Implemented K-Means, DBSCAN, and Hierarchical Clustering.

## Clustering Algorithms

### 1. K-Means Clustering
Identifies distinct clusters by minimizing intra-cluster variance. Applied to the RFM metrics with 8 clusters, yielding a silhouette score of 0.7048.

### 2. DBSCAN
A density-based clustering algorithm that handles outliers well. Applied with `eps = 0.1` and `min_samples = 7`, achieving a silhouette score of 0.7305.

### 3. Hierarchical Clustering
Creates a dendrogram to visualize relationships between clusters. Achieved the highest silhouette score (0.7614), revealing fine-grained patterns in customer behavior.

## Results

Each clustering algorithm's performance was evaluated based on its silhouette score. Hierarchical clustering outperformed other methods, followed by DBSCAN and K-Means. This segmentation allows e-commerce platforms to implement targeted marketing strategies based on distinct customer profiles.

## Learning Outcomes

- **Clustering Techniques**: Gained hands-on experience with K-Means, DBSCAN, and Hierarchical Clustering.
- **Data Preprocessing**: Mastered data cleaning, feature engineering, and scaling for better clustering results.
- **Evaluation**: Used silhouette scores to evaluate model effectiveness.

## Tools and Libraries

- **Programming Language**: Python
- **Libraries**:
  - `pandas` and `numpy` for data manipulation
  - `scikit-learn` for clustering models
  - `matplotlib` and `seaborn` for visualization

## Conclusion

The project demonstrates the effectiveness of clustering techniques in e-commerce customer segmentation, providing actionable insights to improve customer engagement and marketing strategies. Hierarchical clustering proved to be the most informative, highlighting both broad and niche customer groups.

---

Feel free to explore the code and provide any feedback. Happy analyzing!
