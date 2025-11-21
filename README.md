# Wine Dataset Clustering – Hierarchical & DBSCAN

## Overview
This lab explores two clustering techniques—Hierarchical Clustering and DBSCAN—using the Wine dataset from the sklearn library. The goal was to understand how different clustering algorithms behave, how parameter choices influence results, and how visualizations can support the interpretation of clustering outcomes.

## What This Lab Covers
- Loading and preparing the Wine dataset  
- Standardizing features for distance-based learning  
- Applying hierarchical clustering and generating a dendrogram  
- Testing multiple `n_clusters` values  
- Applying DBSCAN with several `eps` and `min_samples` settings  
- Highlighting cluster assignments and noise points through visualizations  
- Evaluating clustering quality using:
  - Silhouette Score  
  - Homogeneity Score  
  - Completeness Score  

## Key Insights
- Hierarchical clustering produced stable clusters and was easier to interpret thanks to the dendrogram.  
- DBSCAN required more experimentation, as small changes to `eps` significantly altered cluster structure.  
- DBSCAN was effective in identifying noise, but hierarchical clustering aligned better with the dataset’s structure.  
- Standardizing features was essential for both models due to their reliance on distance calculations.

## Challenges and Decisions
- Selecting meaningful `eps` values for DBSCAN required trial and error because the dataset does not naturally exhibit density-based clusters.  
- Some DBSCAN configurations labeled a high number of samples as noise, reducing the usefulness of the silhouette score.  
- Visualizing clusters in high-dimensional data required dimensionality considerations, so initial visualizations were plotted using two standardized features.

## Files Included
- `Lab_Clustering_Wine.ipynb` – Full implementation with explanations, visualizations, and metrics  
- `README.md` – Summary of the objectives, insights, and decisions made during the lab  