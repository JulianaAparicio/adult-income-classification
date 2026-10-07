# Adult Income Classification

Machine learning project focused on predicting whether an individual's annual income exceeds $50,000 using demographic and employment-related variables.

## Academic Context

This project was completed for CIS 8693: Data Analytics, AI for Digital Innovation as part of the Master of Science in Information Systems (MSIS) program at Georgia State University.

## Objective

Compare multiple classification algorithms and identify the model with the strongest predictive performance for predicting income levels.

## Dataset

The Adult Income dataset contains demographic and employment-related information used to predict whether an individual's annual income exceeds $50,000.

Target classes:

- Income > $50K
- Income ≤ $50K

## Models Evaluated

- Logistic Regression
- Decision Tree
- Random Forest

Additional models, including K-Nearest Neighbors (KNN), were explored during development. The final analysis focused on Logistic Regression, Decision Tree, and Random Forest, which were included in the report.

## Results

Four models were evaluated during the analysis:

| Model | Accuracy | Precision | Recall | ROC-AUC |
|---------|---------|---------|---------|---------|
| Logistic Regression | 76.87% | 50.43% | 76.35% | 76.69% |
| Decision Tree | 81.66% | 60.84% | 61.09% | 74.52% |
| Tuned Decision Tree | 79.66% | 54.23% | 84.69% | 81.40% |
| Random Forest | 81.82% | 57.54% | 85.63% | 83.14% |

The Random Forest model achieved the strongest overall performance and was selected as the final model.

## Key Findings

Several factors were found to be strongly associated with higher income levels:

- Education level
- Age
- Marital status
- Hours worked per week
- Capital gains

The Random Forest model demonstrated the best ability to identify individuals earning more than $50,000 annually.

## Technologies

- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn

## Repository Contents

- Source code
- Dataset
- Final report
- Model evaluation results
- Visualizations

## Status

Completed academic project.
