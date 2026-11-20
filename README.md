# NTI Machine Learning Portfolio

A portfolio of machine learning coursework and a final project developed for the NTI Machine Learning for Data Analysis course.

## Final Project: India Air Quality Forecasting

This project uses daily air-quality measurements from Indian cities to study pollution patterns and predict next-day Air Quality Index (AQI).

### Project objectives

- Predict the next day's AQI using regression models.
- Predict the next-day AQI category using classification models.
- Group cities with similar pollution profiles using clustering.

### Dataset

The dataset contains 29,531 records, 16 columns, and measurements from 26 Indian cities, covering 2015 to 2020.

Source: [Air Quality Data in India — Kaggle](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india/data)

### Methods

The workflow includes exploratory data analysis, missing-value handling, feature preprocessing, time-based train/test splitting, model comparison, temporal cross-validation, hyperparameter tuning, and city clustering.

### Selected results

| Task | Result |
|---|---|
| AQI regression | Bagging achieved the lowest test MAE: 17.098 |
| AQI regression | Random Forest achieved RMSE 27.739 and R² 0.908 |
| AQI category classification | Random Forest achieved Macro F1 0.735 |
| City clustering | Agglomerative clustering achieved a silhouette score of 0.421 |

The test-period results are exploratory because the same test period was used in repeated model comparisons. Temporal cross-validation results are also included in the analysis.

## Tools

Python, Jupyter Notebook, pandas, NumPy, Matplotlib, and scikit-learn.
