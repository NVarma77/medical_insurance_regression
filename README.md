# Medical Insurance Cost Prediction

## Overview
This project builds a **regression pipeline** to predict individual medical insurance charges based on demographic and health-related features. The goal is to understand cost drivers and compare linear and regularized models for predictive performance and interpretability.

## Dataset
- Features include:
  - Age
  - Sex
  - BMI
  - Number of children
  - Smoking status
  - Region
- Target:
  - Medical insurance charges

### Preprocessing
- One-hot encoding for categorical variables
- Feature scaling where appropriate
- Train/test split for evaluation

## Methods

### Models
- **Linear Regression** (baseline)
- **Ridge Regression**
- **Lasso Regression**

Regularization was used to reduce overfitting and analyze feature importance.

### Training & Evaluation
- Models trained on standardized feature sets
- Evaluation metrics:
  - R² score
  - Mean Squared Error (MSE)
- Coefficient analysis to interpret feature impact

## Results
- Smoking status and age emerged as the strongest predictors of insurance cost
- Regularized models improved generalization over plain linear regression
- Lasso performed implicit feature selection by shrinking weaker coefficients to zero

## Key Takeaways
- Healthcare costs are strongly influenced by lifestyle-related features
- Regularization improves stability and interpretability in linear models
- Simple models can perform competitively with proper preprocessing

## Tech Stack
- Python  
- pandas  
- NumPy  
- scikit-learn  
- Matplotlib / Seaborn  

## Future Work
- Add non-linear models (Random Forest, Gradient Boosting)
- Perform interaction feature engineering
- Extend to fairness and bias analysis across demographic groups
