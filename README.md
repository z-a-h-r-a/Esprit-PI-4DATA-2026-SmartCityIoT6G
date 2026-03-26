# AI-Driven Attack Defense for IoT Smart City in 6G Networks

## Overview
This project was developed as part of the PI – 4th Year Engineering Program at **Esprit School of Engineering** (Academic Year 2025–2026).

It presents an AI-powered intrusion detection system designed to automatically detect and defend against cyber-attacks (DDoS, MITM, Botnet) targeting IoT devices within Smart City infrastructures operating over 6G networks. The project follows the **CRISP-DM methodology** and evaluates detection models across four network slicing datasets: mMTC, URLLC, eMBB, and G6.

## Features
- AI-based cyber-attack detection across 6G network slices (mMTC, URLLC, eMBB, G6)
- Multi-model comparison: Logistic Regression, KNN, Random Forest, Gradient Boosting
- Slice-specific preprocessing pipelines tailored to each network category
- Feature selection with 62–71% dimensionality reduction while preserving detection accuracy
- Class imbalance handling via stratified sampling and class-weighted approaches
- Model evaluation using Accuracy, Precision, Recall, F1-score, ROC-AUC
- Permutation-based feature importance analysis

## Tech Stack

### Language
- Python 3.x

### Data Manipulation & Computing
- Pandas
- NumPy

### Data Visualization
- Matplotlib
- Seaborn

### Preprocessing & Feature Engineering
- Scikit-learn (StandardScaler, RobustScaler, OneHotEncoder, SimpleImputer, KNNImputer, ColumnTransformer, Pipeline)

### Machine Learning Models
- Logistic Regression (baseline)
- K-Nearest Neighbors (KNN)
- Random Forest Classifier
- Gradient Boosting Classifier

### Model Evaluation
- classification_report, confusion_matrix
- roc_auc_score, RocCurveDisplay
- Permutation Feature Importance

### Project Organization
- Pathlib

## Architecture

The project follows the CRISP-DM methodology across 6 phases:
