# Regression Techniques in Python

## Project Overview

This repository contains six regression tasks designed to develop practical knowledge of regression algorithms, model evaluation, regularization, diagnostics, and feature engineering using Python.

The project demonstrates how to implement regression models from scratch, train models using Scikit-learn, evaluate their performance, visualize results, and interpret model behavior.

## Objectives

- Understand the mathematics behind linear regression.
- Implement simple linear regression from scratch.
- Train and evaluate multiple linear regression models.
- Explore polynomial regression with different polynomial degrees.
- Apply Ridge, Lasso, and ElasticNet regularization.
- Evaluate regression assumptions using diagnostic plots and statistical methods.
- Create useful features to improve model performance.
- Compare models using standard regression evaluation metrics.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels
- Jupyter Notebook

## Project Structure

```text
regression-techniques-python/
├── README.md
├── requirements.txt
├── Task_A_Simple_Linear_Regression.ipynb
├── Task_B_Multiple_Linear_Regression.ipynb
├── Task_C_Polynomial_Regression.ipynb
├── Task_D_Regularization.ipynb
├── Task_E_Regression_Diagnostics.ipynb
├── Task_F_Feature_Engineering.ipynb
├── data/
│   └── README.md
└── plots/
    ├── regression_line.png
    ├── polynomial_curves.png
    ├── regularization_error.png
    ├── coefficient_shrinkage.png
    └── regression_diagnostics.png
```

The `data/` folder contains dataset documentation or project datasets where appropriate. The `plots/` folder stores exported visualizations.

## Task A — Simple Linear Regression From Scratch

### Description

Implement simple linear regression manually using a dataset with one independent variable and one dependent variable.

### Key Activities

- Calculate mean, variance, and covariance.
- Calculate slope and intercept.
- Implement a prediction function.
- Compare the manual implementation with Scikit-learn's `LinearRegression`.
- Plot the original observations and fitted regression line.

### Deliverables

- Jupyter Notebook
- Mathematical explanation
- Regression line plot
- Comparison of manual and Scikit-learn results

## Task B — Multiple Linear Regression

### Description

Train a regression model using multiple independent variables to predict a continuous target.

### Key Activities

- Load and inspect the dataset.
- Handle missing values.
- Encode categorical variables.
- Split the data into training and testing sets.
- Train a multiple linear regression model.
- Evaluate the model using MAE, MSE, RMSE, and R².
- Interpret the model coefficients.

### Deliverables

- Notebook with preprocessing
- Evaluation metrics
- Coefficient interpretation

## Task C — Polynomial Regression

### Description

Investigate nonlinear relationships by creating polynomial features and comparing fitted models.

### Key Activities

- Create polynomial features of degree 2 and degree 3.
- Train polynomial regression models.
- Compare them with ordinary linear regression.
- Visualize fitted curves.
- Compare model performance using a table.

### Deliverables

- Polynomial regression plots
- Performance comparison table
- Interpretation of model complexity

## Task D — Regularization Techniques

### Description

Study Ridge, Lasso, and ElasticNet to understand how regularization controls model complexity.

### Key Activities

- Train Ridge, Lasso, and ElasticNet models.
- Test multiple alpha values.
- Compare model errors across alpha values.
- Plot coefficient shrinkage.
- Explain the differences between L1 and L2 regularization.

### Deliverables

- Jupyter Notebook
- Error-versus-alpha plot
- Coefficient-versus-alpha plot
- Explanation of when to use each technique

## Task E — Regression Diagnostics

### Description

Evaluate regression assumptions and investigate potential issues that affect model reliability.

### Key Activities

- Check linearity using residuals-versus-predictions plots.
- Examine residual normality using histograms and Q-Q plots.
- Investigate homoscedasticity using residual plots and suitable statistical checks.
- Calculate Variance Inflation Factor (VIF) for multicollinearity.
- Summarize which assumptions appear reasonable and which may be violated.

### Deliverables

- Diagnostic plots
- VIF table
- Regression assumptions report
- Recommended corrective actions

## Task F — Feature Engineering for Regression

### Description

Create meaningful features and evaluate whether they improve regression performance.

### Key Activities

- Create at least five engineered features.
- Remove irrelevant or redundant features when justified.
- Investigate highly correlated predictors.
- Train and evaluate a baseline model.
- Train and evaluate a model using engineered features.
- Compare performance before and after feature engineering.

### Deliverables

- Before-and-after performance comparison
- Explanation of engineered features
- Feature selection justification
- Final interpretation

## Regression Evaluation Metrics

| Metric | Purpose |
|---|---|
| MAE | Measures average absolute prediction error. |
| MSE | Measures average squared prediction error. |
| RMSE | Expresses prediction error in the target's original units. |
| R² | Measures the proportion of target variance explained by the model. |

Lower MAE, MSE, and RMSE generally indicate smaller prediction errors. Higher R² generally indicates a better fit, but evaluation should also consider test performance, model assumptions, and overfitting.

## Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/regression-techniques-python.git
cd regression-techniques-python
```

Replace `YOUR_USERNAME` with your GitHub username.

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate on Windows:

```bash
venv\Scripts\activate
```

Activate on Linux or WSL:

```bash
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

Open the required notebook and execute the cells in order.

## Important Considerations

- Use a consistent train-test split when comparing models.
- Fit preprocessing steps only on training data to avoid data leakage.
- Standardize features when required by regularized models.
- Use cross-validation where appropriate for selecting hyperparameters.
- Evaluate polynomial models carefully because higher degrees may overfit.
- Treat diagnostic plots and statistical tests as evidence rather than absolute proof of model assumptions.
- Document dataset sources, preprocessing decisions, and model limitations.

## Conclusion

This project provides practical experience with regression algorithms and the complete modeling workflow, from data preparation and mathematical implementation to model evaluation, diagnostics, and feature engineering.

## Author

Data Science and AI/ML Portfolio Project
