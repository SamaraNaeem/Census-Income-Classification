# Census Income Classification

This project presents a comparative study of machine learning models for predicting income levels (≤50K or >50K) using the UCI Census Income dataset. The study evaluates Artificial Neural Networks (ANN), Decision Tree, and Random Forest classifiers.

## Objective
To compare traditional machine learning and neural network-based models for income classification and identify the most effective approach based on performance metrics.

## Dataset
- Source: UCI Machine Learning Repository (Adult / Census Income Dataset)
- Features include demographic and socio-economic attributes such as:
  - age, education, occupation
  - marital status, relationship
  - capital gain/loss, hours per week
- Target variable: income (≤50K or >50K)

## Models Implemented
- Artificial Neural Network (Feed-forward ANN with ReLU and Adam optimizer)
- Decision Tree Classifier (Gini index-based splitting)
- Random Forest Classifier (100 decision trees, ensemble voting)

## Methodology
- Data cleaning and preprocessing
- Handling missing values
- Encoding categorical variables
- Model training and validation
- Performance comparison across models

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- Area Under the Curve (AUC)
- ROC and Precision-Recall curves

## Results Summary
| Model | Accuracy | Precision | Recall | F1-score | AUC |
|------|----------|-----------|--------|----------|-----|
| ANN | 84.7% | 74.1% | 59.6% | 66.1% | 0.91 |
| Decision Tree | 79.9% | 59.5% | 61.0% | 60.0% | 0.73 |
| Random Forest | 85.0% | 74.1% | 61.4% | 67.1% | 0.90 |

Random Forest achieved the highest accuracy, while ANN and Random Forest demonstrated superior class discrimination based on AUC values.

## Feature Importance
Feature importance analysis revealed that variables such as:
- relationship
- education_num
- capital_gain  
were key predictors of income level.

## Project Structure
- notebooks/ : Jupyter notebooks containing analysis and experiments
- README.md : Project overview

## Tools & Technologies
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- TensorFlow / Keras
- Jupyter Notebook

## How to Run
1. Clone the repository
   ```bash
   git clone https://github.com/SamaraNaeem/Census-Income-Classification.git
