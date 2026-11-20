# Task 03: Stroke Prediction Classification

## Objective

Build a binary classification model to predict whether a record is associated with a stroke.

## Dataset

The dataset contains 5,110 records and 12 columns. The target is `stroke`: 249 records are positive cases and 4,861 are negative cases.

Source: [Stroke Prediction Dataset on Kaggle](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)

## Workflow

- Explore the data and review class balance.
- Impute missing BMI values using the median.
- Encode categorical features.
- Split the data into training and test sets using a stratified 80/20 split.
- Train a Logistic Regression baseline.
- Evaluate with a classification report and confusion matrix.

## Results

| Metric | Test result |
|---|---:|
| Accuracy | 0.952 |
| Stroke precision | 0.667 |
| Stroke recall | 0.040 |
| Stroke F1-score | 0.075 |

The test set contained 50 stroke-positive records; the model identified 2 of them. Accuracy alone can overstate performance because the dataset is highly imbalanced. The notebook also reports a convergence warning for Logistic Regression.

## Project files

- `healthcare-dataset-stroke-data.ipynb` — the notebook.
- `healthcare-dataset-stroke-data.csv` — the dataset.
