# Seattle Weather Prediction using Decision Trees

This repository contains a Jupyter Notebook that demonstrates how to build and evaluate a Decision Tree Classifier to predict Seattle weather (Rain or Sun) using historical weather data. The project covers everything from data loading and cleaning to model training, visualization, and evaluation.

---

## Dataset

The dataset includes daily weather records with the following features:
- `precipitation`
- `temp_max`
- `temp_min`
- `wind`
- `weather` (target label: Rain or Sun)

---

## Libraries Used

- `pandas` for data manipulation
- `matplotlib` for data visualization
- `scikit-learn` for machine learning

---

## Tasks Performed

### 1. Data Preparation
- Loaded the dataset and filtered for only "Rain" and "Sun" days
- Handled missing values and cleaned the data

### 2. Exploratory Analysis
- Generated summary statistics
- Counted days with rain
- Plotted the distribution of weather types

### 3. Train-Test Split
- Split the dataset into 80% training and 20% testing using `train_test_split`
- Set `random_state=42` for reproducibility

### 4. Model Training
- Trained a Decision Tree Classifier using `max_depth=6` to prevent overfitting
- Used `fit()` with the training data

### 5. Tree Visualization
- Visualized the trained decision tree using `plot_tree()` from `sklearn.tree`

### 6. Model Evaluation
- Made predictions on the test set
- Calculated the accuracy score of the model

### 7. Optional Task: Overfitting Analysis
- Trained a second model without specifying `max_depth`
- Observed a drop in accuracy due to overfitting on training data

---

## Results

| Model Configuration           | Accuracy |
|------------------------------|----------|
| Decision Tree (max_depth=6)  | 81.23%   |
| Full Tree (no depth limit)   | 73.04%   |

The second model overfits the training data, which led to a lower accuracy score on the test set.

---

