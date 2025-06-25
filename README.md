# 🌦️ Seattle Weather Prediction using Decision Tree

This project demonstrates how to build and evaluate a **Decision Tree Classifier** to predict Seattle's weather (Rain or Sun) based on historical data. The notebook includes steps from data preprocessing to model training, evaluation, and visualization.

---

## 📁 Dataset

The dataset includes daily records of:
- `precipitation`
- `temp_max`
- `temp_min`
- `wind`
- `weather` (target label: Rain or Sun)

---

## 📚 Tools Used

- **Python 3.9+**
- **pandas** – Data manipulation
- **matplotlib** – Visualization
- **scikit-learn** – Machine learning

---

## 🧠 Tasks Covered

### ✅ 1. Data Loading & Cleaning
- Loaded data using `pandas`
- Filtered relevant weather classes (Rain, Sun)
- Dropped missing/null values

### ✅ 2. Data Exploration
- Summary statistics
- Count of rainy days
- Visualized weather distribution

### ✅ 3. Train-Test Split
- Used `train_test_split` with `test_size=0.2`
- Set `random_state=42` for reproducibility

### ✅ 4. Model Training
- Trained a `DecisionTreeClassifier` with `max_depth=6`
- Used `fit()` with training data

### ✅ 5. Visualization
- Visualized decision tree using `sklearn.tree.plot_tree()`

### ✅ 6. Model Evaluation
- Predictions made with `predict()`
- Accuracy score using `accuracy_score`

### ✅ 7. Bonus (Optional)
- Trained a second model without `max_depth`
- Accuracy dropped due to overfitting

---

## 📊 Accuracy Results

| Model Type                  | Accuracy |
|-----------------------------|----------|
| Decision Tree (`max_depth=6`)   | **81.23%** |
| Full Tree (no depth limit)      | **73.04%** ❌ Lower due to overfitting |

> The deeper tree model overfit the training data and performed worse on unseen test data.

---


