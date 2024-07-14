# Breach Analysis in Health Care System

## Description

This project evaluates undersampling versus oversampling techniques to enhance the detection of cybersecurity incidents in the healthcare sector. By comparing traditional SMOTE with the new SMOTE-NC method, the research aims to improve the identification of potential breaches using a dataset from FauxCura Health's Security Incident and Event Management (SIEM) system.

## Objectives

- Analyze historical network data to identify undetected cybersecurity breaches.
- Compare the performance of various machine learning models using different sampling techniques.

## Data Overview

The dataset consists of records extracted from FauxCura's SIEM, which aggregates log data from multiple sources, including servers, routers, and network equipment. The data is processed to summarize individual event detections and contains inconsistencies that require cleaning.

## Methodology

1. **Data Preprocessing**: Cleaning and preparing the data for analysis.
2. **Modeling Approaches**:
   - **Undersampling**:
     - Logistic Regression
     - XGBoost
     - Neural Networks
   - **Oversampling (SMOTE-NC)**:
     - Logistic Regression
     - XGBoost
     - Neural Networks

## Results

| Model               | Undersampling Accuracy | Oversampling (SMOTE-NC) Accuracy |
|---------------------|------------------------|-----------------------------------|
| Logistic Regression  | 0.8795                 | 0.9063                            |
| XGBoost              | 0.9216                 | 0.9368                            |
| Neural Network       | 0.9250                 | 0.9444                            |

The results demonstrate that SMOTE-NC significantly improves model performance across various metrics, underscoring its importance in cybersecurity applications.

## Installation

To run this project, ensure you have the necessary dependencies installed:

```bash
pip install -r requirements.txt
