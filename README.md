# Iris Flower Classification

A machine learning project that classifies iris flowers into three species (setosa, versicolor, and virginica) based on sepal and petal measurements. Built as an internship machine learning task using scikit-learn.

## Dataset
The Iris dataset is loaded directly using `sklearn.datasets.load_iris()`. It contains 150 samples across 3 classes (50 samples each) with 4 features: sepal length, sepal width, petal length, and petal width.

## Models
Three classification algorithms were implemented and trained:
- Logistic Regression
- K-Nearest Neighbors (k=5)
- Decision Tree Classifier (max_depth=3)

## Results
Evaluation metrics obtained on the 20% stratified test set (30 samples) and 5-fold cross-validation:

| Model | Test Accuracy | Macro F1 | 5-Fold CV Mean | CV Std |
|---|---|---|---|---|
| Logistic Regression | 93.33% | 0.9333 | 96.00% | 0.0389 |
| K-Nearest Neighbors (k=5) | 93.33% | 0.9327 | 96.00% | 0.0249 |
| Decision Tree (max_depth=3) | 96.67% | 0.9666 | 97.33% | 0.0249 |

All models classified setosa with 100% precision and recall. Errors were limited to slight overlap between versicolor and virginica.

## How to Run
1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Open and run the notebook:
   ```bash
   jupyter notebook iris_classification.ipynb
   ```
