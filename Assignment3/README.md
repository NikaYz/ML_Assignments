
# Assignment 3: Clustering News Headlines

## Overview
This project involves clustering news headlines to uncover patterns in textual data. Using a preprocessed dataset of 19,685 headlines transformed into a 1,000-dimensional feature vector via the TF-IDF method, we apply **K-Means Clustering** and compare it with **Hierarchical Clustering** on a smaller subset of the data.

---

## Dataset
The dataset includes:
1. **headlines.csv**: A CSV file containing 19,685 news headlines.
2. **tfidf_features.npy**: A NumPy file containing the corresponding TF-IDF feature matrix of shape (19,685, 1000).

---

## Tasks

### 1. Load and Explore the Dataset
- Load the dataset and feature matrix.
- Confirm successful loading by inspecting shapes and basic statistics.

### 2. K-Means Clustering
- Identify the optimal number of clusters (**k**) using methods like the elbow method or KNeedLocator.
- Cluster headlines and analyze the contents of at least three clusters by examining representative headlines.

### 3. Hierarchical Clustering (Subset of 1,000 Headlines)
- Perform Agglomerative Hierarchical Clustering on a random subset.
- Visualize clusters using a dendrogram.
- Assign clusters based on dendrogram analysis.

### 4. Comparison and Summary
- Compare themes and patterns from K-Means and Hierarchical Clustering.
- Summarize observations in the report.

---

## Methods and Models

### 1. K-Means Clustering
- Implemented using Scikit-learn’s API.
- Optimal clusters identified as **146** using KNeedLocator.
- Observations: Common words within clusters (e.g., *Parenting*) highlight the influence of TF-IDF.

### 2. Hierarchical Clustering
- Implemented via Agglomerative Clustering on a subset of 1,000 headlines.
- Number of clusters estimated as **225**, with challenges in interpreting dendrograms due to sample randomness.
- Observations: Clustering primarily based on recurring keywords (e.g., *Need*).

---

## Report Summary
- **K-Means Clustering**: Efficient clusters formed with optimal k=146, highlighting patterns based on specific keywords.
- **Hierarchical Clustering**: Dendrogram-based clustering revealed inconsistencies due to random sampling.
- **Challenges**: Discrepancies in cluster numbers and themes emphasize the role of preprocessing and sampling strategies.

---

## Deliverables

1. **Jupyter Notebook (.ipynb)**
   - Contains all code, visualizations, and brief explanations.

2. **Report (.pdf/.docx)**
   - Summarizes findings with:
     - Optimal clusters for K-Means.
     - Themes from selected clusters.
     - Observations from Hierarchical Clustering.
   
---


## Resources
1. [K-Means Clustering](https://scikit-learn.org/stable/modules/clustering.html#k-means)
2. [Hierarchical Clustering](https://scikit-learn.org/stable/modules/clustering.html#hierarchical-clustering)

