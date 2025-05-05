 # K-Means Clustering 
 
## Libraries Used

* **NumPy:** For numerical operations.
* **Pandas:** For data manipulation and analysis (using DataFrames).
* **Seaborn:** For data visualization.
* **Matplotlib.pyplot:** For plotting.
* **Scikit-learn:** For K-Means clustering and silhouette score calculation.

## Data Preprocessing

1.  The notebook loads the data using Pandas.
2.  The "Unnamed: 0" column is dropped as it appears to be an index column.

## K-Means Clustering

1.  **Elbow Method:** The notebook uses the Elbow Method to determine the optimal number of clusters (`k`). It iterates through a range of `k` values (2 to 9), calculates the Within-Cluster Sum of Squares (WCSS) for each `k`, and plots the WCSS against `k`. The "elbow" point in the plot helps visualize the best `k`.
2.  **Clustering:** K-Means clustering is performed with the chosen optimal `k` (in this case, `k=3`).
3.  **Cluster Assignment:** The data is labeled with the cluster assignments.

## Cluster Analysis

1.  **Cluster Centers:** The notebook prints the cluster centers to understand the average regulatory performance of each cluster.
2.  **Performance Grouping:** A new column "Performance" is created to categorize countries based on their cluster: "High" (cluster 2), "Medium" (cluster 1), and "Low" (cluster 0).
3.  **Countries with Highest Performance:** The notebook identifies and prints the list of countries belonging to the "High" performance cluster.

## Evaluation

* **Silhouette Score:** The Silhouette Score is calculated to evaluate the quality of the clustering.  A score closer to 1 indicates better-defined clusters.

## Summary

This notebook provides a basic K-Means clustering analysis to group countries based on their construction permit regulatory data. The analysis helps to identify groups of countries with high, medium, and low regulatory performance, which could be useful for policy-making or further research.# K-Means-Clustring
