# Final Project: Next-Day Air Quality Forecasting in India

## Overview

This project analyzes daily air-quality readings from Indian cities. It predicts next-day AQI and AQI category, and uses clustering to explore similarities between city pollution profiles.

## Dataset

The dataset contains 29,531 records, 16 columns, and measurements from 26 cities, covering 2015–2020.

Source: [Air Quality Data in India — Kaggle](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india/data)

## Project workflow

- Explore the data and review missing values and AQI distributions.
- Create next-day targets within each city, using only consecutive calendar dates.
- Cap AQI values at 500 for modeling.
- Split training and test data chronologically.
- Compare regression and classification models using temporal validation.
- Cluster city pollution profiles and examine feature importance.

## Selected results

| Task | Result |
|---|---|
| AQI regression | Bagging achieved the lowest test MAE: 17.098 |
| AQI regression | Random Forest achieved RMSE 27.739 and R² 0.908 |
| AQI category classification | Random Forest achieved Macro F1 0.735 |
| City clustering | Agglomerative clustering achieved a silhouette score of 0.421 with two clusters |

The test-period results are exploratory because the same test period was reused during model comparisons.

## Project files

- `Air.ipynb` — project notebook.
- `city_day.csv` — dataset.

## Deployment

The live deployment link will be added after deployment is completed.
