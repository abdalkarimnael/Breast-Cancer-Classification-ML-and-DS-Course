# Breast Cancer Classification

## 📌 Course Information  
- **Course:** Machine Learning & Data Science (ENCS5341)  
- **Assignment:** Assignment #3 - Data Analysis  
- **Instructors:** Dr. Yazan Abu Farha & Dr. Ismail Khater  
- **Institution:** Faculty of Engineering & Technology, Electrical & Computer Engineering Department  
- **Team Members:**
  - **Abdalkarim Eiss** (Me)
  - **Razi Atyani**
- **Date:** 12/27/2024

## Overview
This project investigates multiple supervised machine learning models for classifying breast cancer tumors as benign or malignant. The dataset used is the Breast Cancer dataset from Scikit-learn, and models include:
- **K-Nearest Neighbors (KNN)**
- **Logistic Regression**
- **Support Vector Machines (SVM)**
- **Ensemble Methods (AdaBoost, Random Forest)**

Each model undergoes hyperparameter tuning and is evaluated using accuracy, precision, recall, F1-score, and ROC-AUC metrics.

## Dataset
The dataset consists of **569 samples** with **30 numerical features** representing tumor characteristics. The target variable indicates whether the tumor is **benign (0) or malignant (1)**.

### **Preprocessing**
- Standardization using `StandardScaler`
- Dimensionality reduction using **Principal Component Analysis (PCA)**

## Models Implemented
### **1. K-Nearest Neighbors (KNN)**
- Used different distance metrics: **Euclidean, Manhattan, Cosine**
- Best results achieved with **Euclidean distance (k=3)**

### **2. Logistic Regression**
- Compared **L1 (Lasso) and L2 (Ridge) regularization**
- **L2 regularization** achieved the best performance

### **3. Support Vector Machine (SVM)**
- Tested **Linear, Polynomial, and RBF Kernels**
- **Linear Kernel** outperformed other models with **99.12% accuracy**

### **4. Ensemble Methods**
- **Boosting (AdaBoost)**: Improved weak learners iteratively
- **Bagging (Random Forest)**: Built multiple trees for robust classification
- **AdaBoost** performed better than Random Forest
