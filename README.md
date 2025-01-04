# NVIDIA Market Analytics - K-Means Clustering

## Overview
This project performs K-Means clustering on NVIDIA market analytics data to identify meaningful customer or market segments. The results include group categorization and the counts of each cluster for further analysis.



## Workflow

### 1. Data Preprocessing
- Load the `nvidia_market_analytics.csv` dataset.
- Select numerical columns for clustering.
- Remove rows with missing values.

### 2. Elbow Method
- Use the **Elbow Method** to determine the optimal number of clusters.
- Visualize inertia (within-cluster sum of squares) for k values ranging from 1 to 10.

### 3. K-Means Clustering
- Apply K-Means with `n_clusters=3` (based on the Elbow Method).
- Assign cluster labels to the original dataset.

### 4. Group Naming
- Map cluster labels to descriptive group names:
  - Cluster 0 → First Group
  - Cluster 1 → Second Group
  - Cluster 2 → Third Group

### 5. Group Analysis
- Calculate the counts for each group to understand the distribution of observations across clusters.



## Libraries Used
- **pandas**: For data manipulation and cleaning.
- **scikit-learn**: For implementing K-Means clustering.
- **yellowbrick**: For visualizing the Elbow Method.
- **warnings**: To suppress unnecessary warnings.



## Key Outputs
1. **Optimal Clusters**: Determined using the Elbow Method.
2. **Cluster Labels**: Assigned to the dataset as a new column (`Cluster_Made`).
3. **Group Names**: Replaced numeric labels with descriptive group names.
4. **Cluster Counts**: Summary of the number of observations in each cluster.



## How to Run
1. Ensure the dataset `nvidia_market_analytics.csv` is in the working directory.
2. Install required libraries:
   ```bash
   pip install pandas scikit-learn yellowbrick
3. Run the script in a Python environment.



## Results
- 3 Clusters Identified
- Group Distribution:
  - First Group: 36591
  - Second Group: 646
  - Third Group: 2051
- Dataset updated with a Cluster_Made column for further analysis or visualization.



## Author
Reetika Singh
