# Binary Logistic Regression Using Five Optimization Methods

## 1. Project Overview

This project implements **Binary Logistic Regression** using five different optimization methods to investigate their effects on model convergence, training efficiency, and classification performance.

All experiments use the same dataset, preprocessing steps, model architecture, and data splitting strategy to support a consistent comparison.

## 2. Dataset

**Dataset:** Breast Cancer Wisconsin Diagnostic Dataset

The dataset contains:

- **569 samples**
- **30 numerical features**
- **Target variable:** `diagnosis`
- **Classification type:** Binary Classification

### Target Classes

- **0 — Benign (B)**
- **1 — Malignant (M)**

The objective is to classify breast tumors as benign or malignant based on numerical tumor measurements.

## 3. Data Preprocessing

The following preprocessing steps are applied:

1. Dataset loading and inspection
2. Missing value analysis
3. Duplicate detection and removal
4. Removal of unnecessary columns
5. Target encoding
6. Class distribution analysis
7. Feature and target separation
8. Training, validation, and testing split
9. Feature standardization using StandardScaler
10. Conversion to PyTorch tensors

The dataset is divided into approximately:

- **70% Training**
- **15% Validation**
- **15% Testing**

Feature standardization is fitted only on the training data to prevent data leakage.

## 4. Model Architecture

**Model:** Binary Logistic Regression

The model consists of a single linear layer with 30 input features and one output.

**Loss Function:** Binary Cross-Entropy with Logits

**Framework:** PyTorch

## 5. Optimization Methods

Five optimization approaches are implemented in separate Jupyter notebooks.

| Notebook | Optimization Method | Batch Size |
|---|---|---|
| 01 | Full-Batch Gradient Descent | Entire training set |
| 02 | Stochastic Gradient Descent | 1 |
| 03 | Mini-Batch Gradient Descent | 32 |
| 04 | RMSprop | 32 |
| 05 | Adam | 32 |

Each notebook follows the same general workflow, while the optimization method or batch configuration changes.

## 6. Model Evaluation

The following evaluation metrics are used:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- ROC-AUC
- Log Loss

Training and validation loss curves are also visualized to analyze convergence behavior.

## 7. Experimental Comparison

The optimization methods will be compared based on:

- Classification performance
- Training time
- Loss convergence
- Training stability
- Final training and validation loss

The final comparison will identify differences in the behavior and performance of the five optimization approaches.

## 8. Technologies and Libraries

- Python
- Kaggle Notebooks
- PyTorch
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- GitHub



## 10. Expected Outcome

The project aims to compare how different optimization methods affect the training and performance of Binary Logistic Regression.

The final analysis will examine which methods achieve faster convergence, stable training, and strong classification performance on the selected dataset.


**Project Type:** Machine Learning — Binary Classification

**Platform:** Kaggle

**Programming Language:** Python
