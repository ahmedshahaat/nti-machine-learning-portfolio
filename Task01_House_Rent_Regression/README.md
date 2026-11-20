# Task 01: House Rent Regression

## Objective

Use regression models to estimate house rent from property and listing features.

## Dataset

The task uses the `House_Rent_Dataset.csv` dataset. The original dataset contains 4,746 records and 12 columns. The target variable is `Rent`.

Dataset source: [House Rent Prediction Dataset on Kaggle](https://www.kaggle.com/datasets/iamsouravbanerjee/house-rent-prediction-dataset/data)

After the cleaning and filtering steps in the notebook, 4,727 records remained.

## Workflow

- Explore the dataset and visualize its features.
- Handle missing values and duplicate records.
- Filter extreme values.
- Encode categorical features and scale the input features.
- Split the data into training and test sets using an 80/20 split.
- Train and compare Linear Regression and SGDRegressor.

## Results

Results on the test set:

| Model | MAE | R² |
|---|---:|---:|
| Linear Regression | 23,042.12 | 0.5003 |
| SGDRegressor | 24,336.14 | 0.4514 |

For Linear Regression, the notebook also reports an MSE of 1,444,428,483.75 and an RMSE of 38,005.64.

## Project files

- `House Rent Regression.ipynb` — the Google Colab notebook for this task.
- Dataset source — [House Rent Prediction Dataset on Kaggle](https://www.kaggle.com/datasets/iamsouravbanerjee/house-rent-prediction-dataset/data).
