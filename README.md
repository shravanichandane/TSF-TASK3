# TASK - 3
---

# Prediction using Unsupervised Machine Learning

### Task Overview

The objective of this task is to predict the optimal number of clusters in the Iris dataset using unsupervised machine learning techniques and represent the results visually.

### Steps to Complete the Task

1. **Load the Dataset**
   - Download and load the Iris dataset.
   - The dataset can be accessed [here](https://bit.ly/3kXTdox).

2. **Preprocess the Data**
   - Ensure the dataset is in the correct format for clustering.
   - Standardize the features to ensure they contribute equally to the clustering algorithm.

3. **Apply K-means Clustering**
   - Run the K-means clustering algorithm for different numbers of clusters (e.g., 1 to 10).
   - Calculate the sum of squared errors (SSE) for each number of clusters.

4. **Determine the Optimal Number of Clusters**
   - Use the Elbow method to find the optimal number of clusters.
   - Plot the SSE against the number of clusters to identify the "elbow point" where the SSE starts to decrease more slowly.

5. **Visualize the Clusters**
   - Create visualizations to represent the clustering results.
   - Use a pair plot to visualize the clusters across all feature pairs.
   - Apply Principal Component Analysis (PCA) to reduce the dataset to two dimensions for a clear 2D visualization of the clusters.

### Resources

- **Dataset**: [Iris Dataset](https://bit.ly/3kXTdox)
- **Solution**: ([tsf cluster task.ipynb](https://github.com/shravanichandane/TSF-TASK3/blob/main/tsf%20cluster%20task.ipynb)) You can find this in same respository.

### Tools and Libraries

- **Programming Language**: Python
- **Libraries**: 
  - `pandas` for data manipulation
  - `numpy` for numerical computations
  - `matplotlib` and `seaborn` for data visualization
  - `scikit-learn` for machine learning algorithms and preprocessing

### Visualization Goals

- **Elbow Curve**: Plot showing the SSE for each number of clusters to determine the optimal number.
- **Pair Plot**: Visual representation of the clusters across different feature pairs.
- **PCA Plot**: 2D plot showing the clusters based on the first two principal components for better visualization.

### Conclusion

#### Review of Results

**Optimal Number of Clusters**:
- The Elbow method indicated that the optimal number of clusters for the Iris dataset is three. The Elbow plot showed a noticeable "elbow" point at three clusters, where the reduction in SSE begins to level off.

**Clustering Results**:
- After applying K-means clustering with the optimal number of clusters (three), the data was grouped into three distinct clusters. These clusters correspond to the three species of Iris in the dataset: setosa, versicolor, and virginica.

**Visualizations**:
- **Elbow Plot**: The Elbow plot clearly illustrated the point where adding more clusters did not significantly decrease the SSE, confirming the choice of three clusters.
- **Pair Plot**: The pair plot provided a detailed view of how the clusters are distributed across different feature combinations. The clusters formed distinct groups, which align well with the known species of Iris.
- **PCA Plot**: The PCA plot offered a 2D representation of the clusters, showing a clear separation and compactness of the three clusters, making it easier to visualize the grouping.

**Insights**:
- The clustering results were consistent with the biological classification of the Iris dataset, demonstrating that K-means clustering can effectively identify the inherent grouping in the data.
- The visualizations helped in understanding the structure and distribution of the clusters, making it easier to interpret the results.

By completing this task, you have successfully determined the optimal number of clusters and visually confirmed the effectiveness of the K-means algorithm in clustering the Iris dataset. This exercise has enhanced your skills in unsupervised learning, data preprocessing, and data visualization, which are crucial for more advanced machine learning tasks and real-world data analysis.

---
