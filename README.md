# Student Performance Prediction using Linear Regression

This project implements a Linear Regression model to predict a student's Performance Index based on academic and lifestyle-related features.

---

## Dataset
The dataset is sourced from Kaggle:
- neurocipher/student-performance
- 10,000 rows, 6 columns

### Features
- Hours Studied
- Previous Scores
- Extracurricular Activities (Yes/No encoded as 1/0)
- Sleep Hours
- Sample Question Papers Practiced

### Target
- Performance Index (continuous)

---

## Model
- Linear Regression
- StandardScaler for feature normalization
- Evaluation using R² Score and RMSE

---

## Workflow
1. Load dataset using kagglehub
2. Perform exploratory data analysis
3. Encode categorical features
4. Split dataset into train and test sets
5. Scale features using training data only
6. Train Linear Regression model
7. Evaluate model performance
8. Visualize actual vs predicted values

---

## Evaluation Metrics
- R² Score
- Root Mean Squared Error (RMSE)

---

## Visualization
A scatter plot comparing actual and predicted performance index values.

---

## Conclusion
The model shows that student performance can be effectively predicted using a combination of academic effort and lifestyle habits.

---

## Future Work
- Add Ridge and Lasso regression
- Polynomial regression
- Feature importance analysis
- Convert to classification problem

---

## Author
Created as part of a Machine Learning learning project.
