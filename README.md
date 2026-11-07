# Predicting Red Wine Quality

**Individual Machine Learning Project | R**

An individual data science project exploring how the chemical properties of red wine relate to its quality score. The project uses statistical analysis and machine learning to compare regression approaches and evaluate their ability to predict wine quality on unseen data.

## Project Overview

The analysis uses the red wine quality dataset, containing 1,599 observations and 11 physicochemical predictor variables. The objective is to predict wine quality scores using chemical measurements and compare the performance of different regression models.

## Models Compared

- **Mean Baseline:** Establishes a reference prediction using the average quality score.
- **Ordinary Least Squares (OLS):** Fits a linear regression model.
- **Ridge Regression:** Applies regularization to reduce the influence of less stable coefficients.
- **k-Nearest Neighbors (kNN):** Predicts quality based on neighboring observations.

## Methodology

The project includes:

1. Exploratory data analysis and predictor correlation analysis.
2. Examination of the distribution of wine quality scores.
3. Comparison of OLS and ridge regression coefficients.
4. Hyperparameter tuning for ridge regression and kNN.
5. Grouped cross-validation to account for repeated chemical profiles.
6. Training-fold standardization to avoid information leakage.
7. Held-out test evaluation and residual diagnostics.

## Model Performance

The reported held-out test results are:

| Model | Test RMSE |
|---|---:|
| Mean baseline | 0.813 |
| OLS | 0.681 |
| Ridge regression | 0.680 |
| kNN | 0.677 |

Lower RMSE indicates lower prediction error. All three fitted models outperform the mean baseline. kNN achieves the lowest reported test RMSE, although its improvement over OLS and ridge regression is small.

## Visualizations

The project includes visual analysis of:

- Predictor correlations and quality-score distribution
- OLS versus ridge regression coefficients
- Ridge penalty and kNN neighborhood-size tuning
- Held-out model performance
- Observed versus predicted quality
- Residual patterns on unseen observations

## Tools and Technologies

- **Language:** R
- **Analysis:** Statistical modeling and exploratory data analysis
- **Machine Learning:** OLS, ridge regression, kNN
- **Validation:** Grouped cross-validation and held-out testing
- **Reporting:** R Markdown and HTML
- **Visualization:** R-generated statistical plots

## Repository Contents

- `wine_quality_report.Rmd` — Reproducible R Markdown analysis
- `winequality-red.csv` — Dataset
- `report/` — Rendered HTML report
- `figures/` — Generated visualizations
- `results/` — Additional model outputs, if available

## Key Learning Outcomes

- Applying regression techniques to a real-world dataset
- Comparing linear and neighborhood-based prediction methods
- Understanding regularization and hyperparameter tuning
- Designing validation procedures that reduce data leakage
- Evaluating predictive models using RMSE and residual analysis
- Communicating analytical
