# Student Performance Prediction

This project implements **Linear Regression**, **Logistic Regression**, and **K-Nearest Neighbors (KNN)** models to predict student performance using academic and lifestyle-related features.

---

## Dataset
- Source: Kaggle (`neurocipher/student-performance`)
- Rows: 10,000
- Columns: 6

### Features
- Hours Studied
- Previous Scores
- Extracurricular Activities (Yes/No encoded as 1/0)
- Sleep Hours
- Sample Question Papers Practiced

### Targets
- **Linear Regression**: Performance Index (continuous)
- **Logistic Regression**: Pass/Fail outcome (binary; Performance Index ≥ 40 → Pass)
- **KNN Classification**: Pass/Fail outcome (binary; Performance Index ≥ 40 → Pass)

---

## Models Implemented

### Linear Regression
- Predicts the **Performance Index**.
- Features are normalized using **StandardScaler**.
- Evaluation metrics:
  - R² Score
  - Root Mean Squared Error (RMSE)

### Logistic Regression
- Predicts whether a student will **Pass or Fail**.
- Features are normalized using **StandardScaler**.
- Evaluation metrics:
  - Accuracy Score
  - Confusion Matrix
  - Classification Report
- Probability histogram shows predicted likelihood of passing.

### K-Nearest Neighbors (KNN)
- Predicts whether a student will **Pass or Fail**.
- Distance-based classifier using nearest neighbors.
- Features are normalized using **StandardScaler** (critical for KNN performance).
- Evaluation metrics:
  - Accuracy Score
  - Confusion Matrix
  - Classification Report
- Confusion matrix heatmap visualizes classification performance.
- `k` value chosen as 5 (can be optimized for best performance).

---

## Workflow
1. Load the dataset from Kaggle.
2. Perform exploratory data analysis (head, describe, info, missing values, duplicates).
3. Encode categorical features (Extracurricular Activities → 1/0).
4. Create target variable for Pass/Fail (Performance Index ≥ 40 → 1, else 0).
5. Split dataset into training and testing sets.
6. Scale features using training data only.
7. Train models:
   - Linear Regression → Predict Performance Index
   - Logistic Regression → Predict Pass/Fail
   - KNN → Predict Pass/Fail
8. Evaluate model performance using appropriate metrics.
9. Visualize results:
   - Linear Regression: Predicted vs Actual Performance Index
   - Logistic Regression: Predicted probabilities histogram
   - KNN: Confusion matrix heatmap

---

## Evaluation Metrics

### Linear Regression
- R² Score
- Root Mean Squared Error (RMSE)

### Logistic Regression
- Accuracy Score
- Confusion Matrix
- Classification Report

### K-Nearest Neighbors (KNN)
- Accuracy Score
- Confusion Matrix
- Classification Report

---

## Visualization
- Scatter plot comparing **actual vs predicted performance index** (Linear Regression)
- Histogram of **predicted passing probabilities** (Logistic Regression)
- Confusion matrix heatmap (KNN)

---

## Conclusion
- Linear Regression effectively predicts student **performance scores** using academic and lifestyle data.
- Logistic Regression effectively predicts **pass/fail outcomes** based on the same features.
- KNN also predicts **pass/fail outcomes** and provides an alternative distance-based classification method.
- Both academic effort and lifestyle habits are important predictors of student performance.
- Comparing Logistic Regression and KNN allows evaluation of different classification approaches on the same dataset.

---

## Future Work
- Apply Ridge, Lasso, and Polynomial Regression for improved predictions.
- Perform feature importance analysis.
- Compare Logistic Regression, KNN, and other classification models (SVM, Random Forest, etc.).
- Explore converting performance scores to categories for enhanced classification.
- Optimize KNN `k` value using cross-validation for best results.

---

## Author
Created as part of a Machine Learning learning project.
