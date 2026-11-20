# Task 02: Student Performance Regression

## Objective

Predict a student's Performance Index using previous scores, sleep hours, and extracurricular activity.

## Dataset

The task uses `Student_Performance.csv`, which contains 10,000 records and 6 original columns. The target variable is `Performance Index`.

After preprocessing and removing duplicates, 7,837 records remained.

## Workflow

- Explore the data and visualize feature relationships.
- Remove the `Unnamed: 0` column.
- Drop `Sample Question Papers Practiced`, which has 28.56% missing values.
- Fill missing extracurricular activity values with the most frequent category.
- Remove duplicate records.
- One-hot encode extracurricular activity.
- Scale Previous Scores and Sleep Hours using MinMaxScaler.
- Split the data into training and test sets using an 80/20 split.
- Train and evaluate a Ridge Regression model.

## Results

| Model | MAE | MSE | RMSE | R² |
|---|---:|---:|---:|---:|
| Ridge Regression | 6.832 | 62.965 | 7.935 | 0.833 |

The train/test split does not set a fixed random state, so results may vary slightly when the notebook is run again.

## Project files

- `Student Performance.ipynb` — the notebook.
- `Student_Performance.csv` — the dataset.
