# Employee Salary Prediction Using Machine Learning

## 1. Project Overview
This project uses machine learning regression models to predict employee salaries based on experience, skill score, job level, and department.

The objective is to build, evaluate, and compare different regression models and identify a suitable model for salary prediction.

**Note:** The dataset contains 100 synthetic employee records and is intended for learning and demonstration purposes.

## 2. Technologies Used
- Python
- Pandas and NumPy
- Scikit-learn
- Matplotlib
- Linear Regression
- Decision Tree Regressor
- GridSearchCV and cross-validation

## 3. Dataset Features

| Feature | Description |
|---|---|
| Experience | Employee's years of experience |
| Skill_Score | Employee skill score |
| Job_Level | Employee's job level |
| Department | Employee's department |
| Salary | Target variable to predict |

## 4. Project Workflow
1. Load and inspect the dataset.
2. Separate input features and target variable.
3. Split the data into training and testing sets.
4. Preprocess numerical and categorical features using a pipeline.
5. Train Linear Regression and Decision Tree models.
6. Tune Decision Tree depth using GridSearchCV.
7. Evaluate the models using MAE, RMSE, and R².
8. Analyze residuals, feature importance, and model predictions.

## 5. Model Evaluation

### Linear Regression

| Dataset | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Training | ₹3,780.61 | ₹4,786.07 | 0.923 |
| Test | ₹3,419.06 | ₹3,786.55 | 0.958 |

### Decision Tree Regressor
The tuned Decision Tree selected a maximum depth of 3.

| Metric | Test Result |
|---|---:|
| MAE | ₹6,866.99 |
| RMSE | ₹8,776.16 |
| R² Score | 0.776 |

**Model selection:** Linear Regression performed better than the Decision Tree on this test set.

## 6. Key Findings
- Linear Regression achieved a test R² score of 0.958.
- The test MAE was approximately ₹3,419.
- Experience was the most important feature in the Decision Tree model, with an importance score of approximately 0.847.
- Residual analysis was used to examine prediction errors.
- Predictions from different models varied for some employee profiles.

## 7. Limitations
- The dataset is small and synthetic.
- Results may not reflect real-world salary patterns.
- The test set contains only 20 records.
- Real-world use would require representative salary data, further validation, and appropriate checks for bias and fairness.

## 8. How to Run the Project
1. Clone or download this repository.
2. Install the required Python libraries.
3. Open the Jupyter Notebook.
4. Run the notebook cells in order.
5. Review the model metrics, residual plot, and predictions.

Install dependencies with:

```bash
pip install pandas numpy scikit-learn matplotlib jupyter
```

## 9. Conclusion
This project demonstrates an end-to-end regression workflow, including preprocessing, model training, hyperparameter tuning, evaluation, interpretation, and prediction.

It provides a foundation for further learning in data analytics and machine learning.
