# AI-Based Patient Risk Scoring System

## Overview
This project presents an end-to-end Artificial Intelligence system designed to assess patient heart disease risk using machine learning.  
Instead of producing a simple binary prediction, the system generates an interpretable **risk score (0–100)** and categorizes patients into **Low, Medium, or High risk**, providing decision-support insights suitable for healthcare applications.

---

## Problem Statement
Traditional classification models provide limited interpretability in medical contexts.  
The goal of this project is to build a **risk-oriented AI system** that:
- Estimates the probability of heart disease
- Converts predictions into meaningful risk scores
- Explains model decisions using feature importance

---

## Dataset
- **Heart Disease Dataset (UCI / Kaggle)**
- Approximately 300 patient records
- Medical features such as age, chest pain type, cholesterol, blood pressure, and exercise-related indicators

---

## Methodology

### 1. Data Exploration
- Dataset inspection and statistical analysis
- Target distribution analysis
- Correlation analysis to identify influential medical features

### 2. Feature Engineering
Custom risk-oriented features were created, including:
- Age-based risk transformations
- Cholesterol-to-age and blood-pressure-to-age ratios
- **Cardiac Stress Score** combining exercise-induced angina, ST depression, and heart rate
- Vessel severity feature integrating blood flow and vessel count

### 3. Model Training
- Logistic Regression used as a baseline model
- Random Forest used to capture non-linear relationships
- Overfitting detected and mitigated using depth and sample constraints
- Cross-validation applied to estimate real-world performance

### 4. Risk Scoring System
- Model probabilities converted to risk scores (0–100)
- Risk categories defined as:
  - **Low Risk:** < 40
  - **Medium Risk:** 40–70
  - **High Risk:** > 70

### 5. Model Explainability
- Feature importance analysis applied
- High-risk predictions interpreted using top contributing features
- Ensured model decisions align with clinical relevance

---

## Results
- The model demonstrates strong predictive performance with improved generalization
- Risk scores provide more actionable insights than binary outputs
- Feature importance confirms reliance on medically meaningful factors such as chest pain type and cardiac stress indicators

Example outputs include:
- Patient risk distribution visualization
- Feature importance chart
- Detailed patient risk report



---

## Tools & Technologies
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook

---

## Key Takeaways
- Demonstrates a complete machine learning pipeline
- Focuses on interpretability and decision support
- Applies AI concepts to a real-world healthcare problem
- Highlights the importance of feature engineering and model explainability

---

## Author
**Khaled Mohamed**  
Junior AI / Machine Learning Engineer  


