# dimensionality-reduction
This is implementation of dimensionality reduction on two datasets.

### Image Dataset: sign-language-mnist
The Sign Language MNIST dataset is an American Sign Language letter dataset of hand gestures. It has 24 classes of letters and can be categorized as a multi-class problem.

### Tabular Dataset: Titanic Survivor Dataset
Titanic Survivor Dataset contains tabular data with name, gender and other info of the survivors of the Titanic.

## Various dimensionality reduction techniques are implemented as follows:
1. PCA
2. SVD
3. LLE
4. t-SNE
5. ISOMAP
6. UMAP

## Observations and Comparisons
We compared each technique on the basis of time of execution and accuracy on image and tabular datasets.

### Algorithm on Image Dataset - Accuracy

|   Algorithm   |    Accuracy    |
| ------------- | -------------  |
|     PCA       |     0.98       |
|     SVD       |     0.64       |
|     LLE       |     0.96       |
|     ISOMAP    |     0.78       |
|     UMAP      |     0.62       |

### Algorithm on Image Dataset - Execution Time

|   Algorithm   | Execution Time |
| ------------- | -------------  |
|     PCA       |     828ms      |
|     SVD       |     951ms      |
|     LLE       |   1min 23sec   |
|     t-SNE     |     2min       |
|     ISOMAP    |   1min 22sec   |
|     UMAP      |     42.4s      |

### Algorithm on Tabular Dataset - Accuracy

|   Algorithm   |    Accuracy    |
| ------------- | -------------  |
|     PCA       |     0.58       |
|     SVD       |     0.68       |
|     LLE       |     0.59       |
|     ISOMAP    |     0.59       |
|     UMAP      |     0.58       |	

### Algorithm on Tabular Dataset - Execution Time

|   Algorithm   | Execution Time |
| ------------- | -------------  |
|     PCA       |     32.6ms     |
|     SVD       |     14ms       |
|     LLE       |     63.5ms     |
|     t-SNE     |     942ms      |
|     ISOMAP    |     55.8ms     |
|     UMAP      |     11s        |

## Analysis
Here, we can observe that for image dataset, t-SNE took maximum time for execution and PCA was most effective with highest accuracy in less time. And for tabular dataset, UMAP took maximum time for execution and SVD was a better option in terms of accuracy in less time. We can see data visualization is pretty clear with SVD technique.