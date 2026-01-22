# Student Performance Prediction

This project implements **Linear Regression** and **Logistic Regression** models to predict student performance using academic and lifestyle-related features.

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

---

## Workflow
1. Load the dataset from Kaggle.
2. Perform exploratory data analysis (head, describe, info, missing values, duplicates).
3. Encode categorical features (Extracurricular Activities → 1/0).
4. Split dataset into training and testing sets.
5. Scale features using training data only.
6. Train models:
   - Linear Regression → Predict Performance Index
   - Logistic Regression → Predict Pass/Fail
7. Evaluate model performance using appropriate metrics.
8. Visualize results:
   - Linear Regression: Predicted vs Actual Performance Index
   - Logistic Regression: Predicted probabilities histogram

---

## Evaluation Metrics

### Linear Regression
- R² Score
- Root Mean Squared Error (RMSE)

### Logistic Regression
- Accuracy Score
- Confusion Matrix
- Classification Report

---

## Visualization
- Scatter plot comparing **actual vs predicted performance index** (Linear Regression)
- Histogram of **predicted passing probabilities** (Logistic Regression)

---

## Conclusion
- Linear Regression effectively predicts student **performance scores** using academic and lifestyle data.
- Logistic Regression effectively predicts **pass/fail outcomes** based on the same features.
- Both academic effort and lifestyle habits are important predictors of student performance.

---

## Future Work
- Apply Ridge, Lasso, and Polynomial Regression for improved predictions.
- Perform feature importance analysis.
- Compare Logistic Regression with other classification models (SVM, Random Forest, etc.).
- Explore converting performance scores to categories for enhanced classification.

---

## Author
Created as part of a Machine Learning learning project.
