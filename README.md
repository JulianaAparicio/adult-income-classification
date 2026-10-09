# Adult Income Classification

Machine learning project that predicts whether an individual's annual income exceeds $50,000 using demographic and employment-related variables.

## Academic Context

Team project completed for **CIS 8693: Data Analytics, AI for Digital Innovation** in the Master of Science in Information Systems (MSIS) program at Georgia State University (J. Mack Robinson College of Business).

**Team:** Juliana Aparicio, [Teammate 2], [Teammate 3]
Analysis, modeling decisions, and interpretation of results were done jointly by the team.

## Objective

Compare classification algorithms and identify the model with the strongest predictive performance for income level, with attention to the trade-off between precision and recall.

## Dataset

The Adult Income (Census) dataset contains demographic and employment information such as age, education, marital status, hours worked per week, and capital gains.

**Target classes:**
- Income > $50K
- Income ≤ $50K

## Models Evaluated

Three models were evaluated (four configurations, including a decision tree before and after tuning):

1. Logistic Regression
2. Decision Tree (default)
3. Decision Tree (tuned)
4. Random Forest

K-Nearest Neighbors was explored informally during development and is not part of the final analysis or report.

## Results

| Model               | Accuracy | Precision | Recall | ROC-AUC |
| ------------------- | -------- | --------- | ------ | ------- |
| Logistic Regression | 76.87%   | 50.43%    | 76.35% | 76.69%  |
| Decision Tree       | 81.66%   | 60.84%    | 61.09% | 74.52%  |
| Tuned Decision Tree | 79.66%   | 54.23%    | 84.69% | 81.40%  |
| Random Forest       | 81.82%   | 57.54%    | 85.63% | 83.14%  |

**Selected model: Random Forest**, which achieved the highest ROC-AUC (83.14%) and recall (85.63%) and the highest accuracy.

## Key Findings

Factors most strongly associated with higher income:
- Education level
- Age
- Marital status
- Hours worked per week
- Capital gains

## Business Interpretation

The Random Forest identifies most higher-income individuals (high recall), but about 4 in 10 of its positive predictions are wrong (precision of 57.5%). It fits situations where missing a true positive is costly. When false positives are expensive, the default Decision Tree (precision 60.8%) may be preferable.

## Limitations and Possible Next Steps

- Add cross-validation to confirm the stability of the results.
- Examine class imbalance handling and its effect on precision and recall.
- Add a feature-importance plot to support the key findings.
- Test additional models and compare them under the same evaluation setup.

## Technologies

Python · pandas · NumPy · scikit-learn · Matplotlib · Seaborn

## Repository Contents

- `census_income.py`: data preparation, modeling, and evaluation
- `adult.csv`: dataset
- `Final_Report.pdf`: final team report
- `requirements.txt`: dependencies

## How to Run

```bash
pip install -r requirements.txt
python census_income.py
```

## Status

Completed academic project.
