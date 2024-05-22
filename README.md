# Machine Learning Project - Phase 3

## Overview

This project involves implementing and evaluating a K-Nearest Neighbors (KNN) algorithm to classify the Oxford 102 Flowers Dataset. The primary goal is to optimize the algorithm's parameters and assess its performance using various metrics.

Unsupervised Classification with K-Means Algorithm:
We begin by applying the K-means algorithm to cluster the data into meaningful groups.
K-means identifies patterns and structures within the feature space without relying on labeled data.
The resulting clusters provide insights into the underlying data distribution.
Supervised Classification with K-Nearest Neighbors (K-NN):
In the subsequent section, we delve into supervised classification using the K-Nearest Neighbors (K-NN) algorithm.
K-NN assigns labels to data points based on the majority class among their nearest neighbors.
Our objective is to achieve the best possible classification accuracy.

## Installation

To run the project, ensure you have Python installed along with the necessary libraries. You can install the required packages using:

```bash
pip install -r requirements.txt
```

## Key Functions

### `gather_clusters_data`

- **Purpose**: Collects data from the nearest clusters.
- **Parameters**:
  - `nearest_indices`: Indices of the nearest clusters.
- **Output**: Aggregated data from the specified clusters.

### `classify_knn`

- **Purpose**: Classifies the input data using the KNN algorithm.
- **Parameters**:
  - `train_data`: Training dataset.
  - `test_data`: Testing dataset.
  - `k1`: Number of clusters.
  - `k2`: Number of nearest neighbors.
- **Output**: Predicted labels for the test data.

## Results

- **Accuracy**: The accuracy of the model varies with different \( k1 \) and \( k2 \) values.
  - Best performance observed with \( k1 = 7 \) and \( k2 = 5 \).
  - Detailed results and comparisons are available in the document file.
 
- **Computation Time**: The computational time for training and testing increases with higher values of \( k1 \) and \( k2 \).
  - Optimal balance achieved with \( k1 = 7 \) and \( k2 = 5 \).

## Conclusion

The project demonstrates the implementation and optimization of the KNN algorithm. By experimenting with different parameters, the model's performance was optimized to achieve a balance between accuracy and computational efficiency.
