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
```
Business Understanding → Data Understanding → Data Preparation
        → Modeling → Evaluation → Deployment
```

### Datasets Used
| Dataset | Rows  | Features | Category                          |
|---------|-------|----------|-----------------------------------|
| mMTC    | 4,615 | 52       | Massive Machine-Type Comms (IoT)  |
| URLLC   | 4,033 | 52       | Ultra-Reliable Low-Latency Comms  |
| eMBB    | 5,808 | 52       | Enhanced Mobile Broadband         |
| G6      | 10,000| 13       | Aggregated 6G Smart City Traffic  |

### Feature Selection Strategy
| Dataset | Original | Selected | Reduction |
|---------|----------|----------|-----------|
| eMBB    | 32       | 12       | 62.5%     |
| mMTC    | 25       | 8        | 68%       |
| URLLC   | 28       | 8        | 71.4%     |
| G6      | 13       | 8        | 38.5%     |

## Contributors

| Name                   | Role         |
|------------------------|--------------|
| Zahra Bendhaw          | Team Member  |
| Tasnim Kheder          | Team Member  |
| Mustapha Aziz Belkadhi | Team Member  |
| Anas Yahyaoui          | Team Member  |
| Rami Klouz             | Team Member  |
| Ahmed Karray           | Team Member  |

## Academic Context

Developed at **Esprit School of Engineering – Tunisia**  
PI – 4DATA | Academic Year 2025–2026  

This project contributes to the following UN Sustainable Development Goals:
- **SDG 9** – Industry, Innovation and Infrastructure
- **SDG 11** – Sustainable Cities and Communities
- **SDG 17** – Partnerships for the Goals

## Getting Started

### Prerequisites
```bash
Python 3.x
pip
```

### Installation
```bash
git clone https://github.com/YOUR-USERNAME/Esprit-PI-4DATA-2026-SmartCityIoT6G.git
cd Esprit-PI-4DATA-2026-SmartCityIoT6G
pip install -r requirements.txt
```

### Required Libraries
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Dataset Setup
Place the following CSV files in the project root directory:
```
mMTC.csv
URLLC.csv
eMBB.csv
Global.csv
6G_English_Education_Network_Traffic.csv
```

### Run the Project
```bash
# Data Understanding
python data_understanding.py

# Data Preparation
python data_preparation.py

# Modeling & Evaluation
python modeling.py
```

## Acknowledgments
We would like to thank **Esprit School of Engineering** and our supervisor for their guidance throughout this project.

Special thanks to the open-source community for the datasets and tools used in this research.
