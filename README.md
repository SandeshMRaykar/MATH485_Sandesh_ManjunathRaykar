# Assignment 2: Recursive Feature Elimination on Diabetes Dataset
Course: MATH/CSCI 485 - Advanced Topics in Data Science  
Student: Sandesh Manjunath Raykar 
Date: February 2026

## Overview
This project implements Recursive Feature Elimination (RFE) with Linear Regression on the scikit-learn Diabetes dataset to identify the most important features for predicting disease progression.

## Key Findings
- Optimal Features: 5 features (50% reduction) with <1% R² loss
- Top 3 Most Important: 
  1. BMI (coefficient: 998.58)
  2. Triglycerides/s5 (coefficient: 562.23)
  3. Total Cholesterol/s1 (coefficient: 228.34)
- Baseline R²: 0.4526
- Optimal R²: 0.4489 (with 5 features)

## Setup & Installation
### Prerequisites
- Python 3.8+
- Jupyter Notebook

Required packages:
numpy
pandas
matplotlib
scikit-learn
jupyter

## How to Run
### Option 1: Jupyter Notebook (Recommended)
   bash
jupyter notebook diabetes.ipynb

Run all cells sequentially. The notebook includes:
- Data exploration
- Baseline model training
- RFE implementation (10 iterations)
- Visualization generation
- Feature importance analysis

### Option 2: Python Script
   bash
python diabetes.py

## Expected Outputs
1. Console Output:
   - Baseline R² score
   - R² at each RFE iteration
   - Top 3 features with coefficients
   - Coefficient evolution table

2. Key Results:
   - Baseline (10 features): R² = 0.4526
   - Optimal (5 features): R² = 0.4489
   - BMI emerges as most important feature

## Methodology
1. Load Dataset: Diabetes dataset (442 samples, 10 features)
2. Train Baseline: Linear regression with all features
3. Run RFE: Iteratively remove least important feature
4. Track Metrics: R² score and coefficients at each iteration
5. Identify Optimal: Find feature count where R² drop > 0.01
6. Analyze: Compare initial vs final feature rankings

## Results
- Optimal: 5 features, R² = 0.4489
- Top 3: BMI (998.58), s5 (562.23), s1 (228.34)
- 50% feature reduction, <1% performance loss

## Files
- diabetes.ipynb - Main code
- MATH_485 Asignment#2_.pdf - Analysis

