# PCA - Principal Component Analysis

PCA - Principal Component Analysis | Example code and own notes while taking the course "Intro to Machine Learning" on Udacity

## How to determine the principle component?

**Variance:** _Technical term in statistics - roughly the "spread" of a data distribution (similar to standard daviation)._

![variance](variance.png)

### Example:
![example](example.png)

## PCA as a General Algorithm for Feature Information
![feature-transformation](feature-transformation.png)

## Eigen vector & value
![eigen-vector](eigen-vector.png)

## Review / Definition of PCA
- Systemized way to transform input features into principal components.
- Use principal components as new features.
- PCs are directions in data that maximize variance (minimize information loss) when you project/compress down onto them.
- More variance of data along a PC, higher that PC is ranked.
- Most variance/most information -> First PC
- Second most variance (without overlapping w/first PC) -> Second PC
- Max no. of PCs = no. of input features.

## When to use PC
- Latent features driving the patterns in data.
- Dimensionality reduction
    - Visualizing high-dimensional data
    - Reduce noise
    - Make other algorithmg (regression, classification)

## F1 score
Accuracy is a less-intuitive metric than in the 2-class case. Instead, a popular metric is the F1 score. 

Higher F1 score is better.

## Selecting a number of principal components

Train on different number of PCs, and see how accuracy responds, cut off when it becomes apparent that adding more PCs doesn't buy you much more discrimination.

