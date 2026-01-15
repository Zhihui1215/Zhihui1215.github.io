---
title: "Breast Cancer Diagnostic Analysis (WDBC)"
collection: portfolio
type: "Machine Learning"
permalink: /portfolio/breast-cancer-wdbc
date: 2025-01-15
excerpt: "Diagnostic modeling on the Wisconsin Breast Cancer dataset using logistic regression and random forest."
header:
  teaser: /images/portfolio/breast-cancer-wdbc/teaser.png
tags:
  - Breast Cancer
  - Medical Data Analysis
  - Classification
  - Machine Learning
tech_stack:
  - name: Python
  - name: Pandas
  - name: Scikit-learn
  - name: Matplotlib
  - name: Seaborn
---

## Project Overview
This project analyzes the Wisconsin Diagnostic Breast Cancer dataset (569 samples, 30 numeric features) to predict
malignant vs benign tumors. The workflow includes data cleaning, exploratory statistics, model training, and
evaluation with visual summaries.

## Data Summary
- Rows: 569
- Features: 30 (excluding ID and label)
- Class distribution: 357 benign, 212 malignant

![Class distribution](/images/portfolio/breast-cancer-wdbc/class_distribution.png)

## Exploratory Analysis
Top discriminative features show clear separation between benign and malignant samples.

![Top feature distributions](/images/portfolio/breast-cancer-wdbc/feature_boxplot.png)
![Correlation heatmap](/images/portfolio/breast-cancer-wdbc/correlation_heatmap.png)

## Modeling
Two classifiers were trained:
- Logistic Regression (standardized features)
- Random Forest (400 trees)

### Evaluation Metrics (Test Set)

| Model | Accuracy | Precision | Recall | F1 | ROC AUC |
| --- | --- | --- | --- | --- | --- |
| Logistic Regression | 0.974 | 0.976 | 0.952 | 0.964 | 0.995 |
| Random Forest | 0.974 | 1.000 | 0.929 | 0.963 | 0.997 |

![ROC curves](/images/portfolio/breast-cancer-wdbc/roc_curve.png)
![Confusion matrix](/images/portfolio/breast-cancer-wdbc/confusion_matrix.png)
![Feature importance](/images/portfolio/breast-cancer-wdbc/feature_importance.png)

## Report
The LaTeX report source is available at:
`/files/breast-cancer-wdbc-report.tex`

Compile it locally with a LaTeX engine to generate the PDF submission.
