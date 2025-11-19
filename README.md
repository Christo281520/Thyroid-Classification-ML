# Thyroid-Classification-ML
A complete ML pipeline for thyroid disease classification, including preprocessing, mutual information feature selection, outlier removal, and evaluation of four algorithms: KNN, SVM, Decision Tree, and GBM.

# Thyroid Disease Classification – Machine Learning Project

This repository contains a complete end-to-end thyroid disease classification system built using multiple supervised ML algorithms.  
The project includes data preprocessing, feature selection, outlier removal, and performance comparison of 4 models.

---

# Files Included

# Jupyter Notebooks
- **Thyroid_GBM.ipynb** – Gradient Boosting Model  
- **Thyroid_KNN.ipynb** – K-Nearest Neighbors  
- **Thyroid_SVM.ipynb** – SVM with Linear, Polynomial, RBF and Sigmoid kernels  
- **Thyroid_DecisionTree.ipynb** – Decision Tree Classifier  

# Dataset
- balanced_thyroid_dataset.csv** – Cleaned and balanced dataset used for training and testing.

---

# Project Overview

This project classifies thyroid conditions into multiple categories using:
- KNN  
- SVM (all kernels)  
- Decision Tree  
- Gradient Boosting  

The goal is to compare different algorithms and determine the best performing model.

---

# Preprocessing Steps

All four notebooks use the SAME preprocessing pipeline:

# 1. Handle Missing Values  
Checked and ensured no missing entries.

# 2. Feature Scaling  
Used **StandardScaler** for:
- `TSH Measured`
- `Tumor`

# 3. Feature Selection  
Used **Mutual Information (mutual_info_classif)**  
Selected **Top 10 important features**.

# 4. Outlier Removal (IQR Method)  
Removed outliers from training data using Interquartile Range.

# 5. Train-Test Split  
80% training – 20% testing.

---

# Model Performance

| Model | Accuracy |
|-------|----------|
| **KNN** | **82.06%** |
| **SVM (Linear Kernel)** | **84.38%** BEST classical model |
| **Decision Tree** | **83.74%** |
| **Gradient Boosting (GBM)** | **~88–90%**  OVERALL BEST |

---

# Why These Models Were Used?

# **KNN**
- Simple, fast baseline model  
- Performs well after scaling  

# **SVM**
- Excellent for medium-sized datasets  
- Linear kernel performed best  

# **Decision Tree**
- Interpretability  
- Handles non-linear patterns  

# **Gradient Boosting**
- Most powerful model  
- Handles complex feature interactions  
- Highest accuracy overall  

---

# Confusion Matrix Example (SVM Best Kernel)

The notebook displays:
- Confusion matrix  
- Precision, Recall, F1-score  
- Class-wise performance  

---

# How to Run the Project

### **Step 1 — Upload dataset to Colab**
python
from google.colab import files
files.upload() 

### OR Use VS code 
upload the files then run

Step 2 — Open any notebook

Thyroid_KNN.ipynb

Thyroid_SVM.ipynb

Thyroid_DecisionTree.ipynb

Thyroid_GBM.ipynb

Step 3 — Run all cells

Models will:

preprocess data

select features

clean outliers

train

predict

show accuracy + reports

Developer

Christo Thomas
MCA Student | Full-Stack Developer | ML Enthusiast | Fresher
GitHub: Christo281520

Email: crisssthomas15@gmail.com
