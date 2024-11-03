# BreastCancerDataAnalysis
## Problem Statement
### Predicting if the cancer diagnosis is benign or malignant based on several observations/features
## 1. Dataset
-> 30 features are used, examples: - radius (mean of distances from center to points on the perimeter) - texture (standard deviation of gray-scale values) - perimeter - area - smoothness (local variation in radius lengths) - compactness (perimeter^2 / area - 1.0) - concavity (severity of concave portions of the contour) - concave points (number of concave portions of the contour) - symmetry - fractal dimension ("coastline approximation")

-> Datasets are linearly separable using all 30 input features

->Number of Instances: 569

->Class Distribution: 212 Malignant, 357 Benign

->Target class: - Malignant - Benign
## 2.Data visualization
## 3.Model Training(Finding a problem solution)
## 4.Support vector Mechines(kernel)
->C parameter: Controlls trade-off between classifying training points correctly and having a smooth decision boundary.

Small C (loose) makes cost (penalty) of misclassification low (soft margin)
Large C (strict) makes cost of misclassification high (hard margin), forcing the model to explain input data stricter and potentially over it.

->gamma parameter: Controlls how far the influence of a single training set reaches.

->Large gamma: close reach (closer data points have high weight)

->Small gamma: far reach (more generalized solution)

->degree parameter : Degree of the polynomial kernel function ('poly'). Ignored by all other kernels.
A common approach to find the right hyperparameter values is to use grid search. It is often faster to first do a very coarse grid search, then a finer grid search around the best values found. Having a good sence of the what each hyperparameter actually does can also help you search in the right part of the hyperparameter space.
### 4.1 Linear kernel SVM
### 4.2 Polynomial Kernel SVM
### 4.3 Radial Kernel SVM

## 5.Data Preparation for SVM
###Numerical Inputs: SVM assumes that your inputs are numeric. If you have categorical inputs you may need to covert them to binary dummy variables (one variable for each category).
###Binary Classification: Basic SVM as described in this post is intended for binary (two-class) classification problems. Although, extensions have been developed for regression and multi-class classification.
## 6. Support Vector Machine Hyperparameter tuning
## 7.Principal Component Analysis
### 7.1 PCA Visualization
    We can use PCA to find the first two principal components, and visualize the data in this new, two-dimensional space, with a single scatter-plot. Before we do this though, we'll need to scale our data so that each feature has a single unit variance.
### 7.2 Interpreting the components
    With this great power of dimensionality reduction, comes the cost of being able to easily understand what these components represent.
## Note:
### Principal Component Analysis:

Used in exploratory data analysis (EDA)

Visualize genetic distance and relatedness between populations.

### Method:

Eigenvalue decomposition of a data covariance (or correlation) matrix
Singular value decomposition of a data matrix (After mean centering / normalizing ) the data matrix for each attribute.
Output

Component scores, sometimes called factor scores (the transformed variable values)
loadings (the weight)
Data compression and information preservation

### Visualization

### Noise filtering

### Feature extraction and engineering