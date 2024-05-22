# Machine Learning Project - Phase 3

## Overview

In this project, we aim to utilize the features extracted from the Flower102 dataset images to develop a robust classification model. The Flower102 dataset consists of images categorized into 102 different classes, with each image represented by a 512-dimensional feature vector. The dataset is divided into two sections: a training set with 4094 instances and a testing set with 4095 instances.

Our approach involves two main stages:

1. **Unsupervised Classification with k-means Algorithm**: We first perform an unsupervised classification of the dataset using the k-means clustering algorithm. This step helps in grouping similar data points together based on their feature vectors without any prior labels.

2. **Supervised Classification with K-Nearest Neighbors (KNN) Algorithm**: After the initial clustering, we break down the data into smaller groups and apply the K-Nearest Neighbors algorithm. This supervised learning technique is used to classify the data points more accurately by leveraging the labeled training data.

The objective is to achieve the best possible classification score by optimizing the parameters of the KNN algorithm, particularly the number of clusters (k1) and the number of nearest neighbors (k2).

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
<img src="./table images/Accuracy.png" width="50%" height="50%">
 
- **Computation Time**: The computational time for training and testing increases with higher values of \( k1 \) and \( k2 \).
  - Optimal balance achieved with \( k1 = 7 \) and \( k2 = 5 \).
<img src="./table images/Computation Time.png" width="50%" height="50%">

## Conclusion

The project demonstrates the implementation and optimization of the KNN algorithm. By experimenting with different parameters, the model's performance was optimized to achieve a balance between accuracy and computational efficiency.
