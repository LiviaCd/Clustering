# Unsupervised Learning – Clustering Algorithms

**Goal:** Study and compare different clustering algorithms applied to various types of datasets.

## Methodology
For each clustering algorithm, a consistent approach was followed:
1. Data preprocessing (normalization or standardization, depending on dataset)
2. Applying the clustering algorithm
3. Visualizing the resulting clusters
4. Evaluating clustering quality using metrics such as silhouette score and visual inspection
5. Tuning relevant parameters (e.g., number of clusters, epsilon value, etc.)

## Overview of Algorithms
- **K-Means Clustering:** Partitions data into K clusters by minimizing intra-cluster variance. Works best with spherical and equally sized clusters.
- **Agglomerative Clustering:** A hierarchical bottom-up approach that merges clusters iteratively based on a linkage criterion (e.g., single, complete, average).
- **DBSCAN (Density-Based Spatial Clustering of Applications with Noise):** Groups together points that are closely packed and marks outliers as noise. Ideal for datasets with clusters of varying shape and density.
- **Expectation-Maximization (EM):** Uses Gaussian Mixture Models to assign probabilities of cluster membership. Suitable for soft clustering with overlapping clusters.


## Insights
Each algorithm performed differently based on the structure and distribution of the data:

- **K-Means** was effective for well-separated, equally sized clusters, but struggled with noise and irregular shapes.
- **DBSCAN** handled arbitrary shapes and noise well, but was sensitive to parameter selection (eps and min_samples).
- **EM** provided flexible cluster boundaries and probabilistic interpretations, making it useful when cluster overlap was expected.
- **Agglomerative Clustering** allowed for hierarchical interpretations and performed well without needing to predefine the number of clusters.

Choosing the right clustering algorithm and parameters proved essential for accurate grouping, especially when working with complex or noisy datasets. Visual and quantitative evaluations helped to better understand cluster quality and algorithm suitability.

