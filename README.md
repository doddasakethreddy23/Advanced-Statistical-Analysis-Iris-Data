# Statistical Analysis of Iris Data

This project explores the statistical relationships in the Iris dataset, a classic dataset in machine learning and statistics. The analysis focuses on identifying key predictors of petal width and validating their significance using various statistical methods.

## Table of Contents
1. [Introduction](#introduction)
2. [Data Description](#data-description)
3. [Research Question](#research-question)
4. [Analysis Steps](#analysis-steps)
5. [Results](#results)
6. [Conclusions](#conclusions)
7. [Future Work](#future-work)
8. [References](#references)

---

## Introduction
The Iris dataset provides measurements for 150 iris flowers from three species: Setosa, Versicolor, and Virginica. This project aims to uncover the relationships between structural features (sepal and petal dimensions) and their influence on petal width. By applying statistical methods, we seek to understand which features strongly predict petal width and validate their significance.

---

## Data Description
The Iris dataset includes the following variables:
- **Sepal.Length**: Length of the sepals in centimeters.
- **Sepal.Width**: Width of the sepals in centimeters.
- **Petal.Length**: Length of the petals in centimeters.
- **Petal.Width**: Width of the petals in centimeters.
- **Species**: Species of the iris flower (Setosa, Versicolor, Virginica).

---

## Research Question
**How do structural features correlate with petal width, and can we statistically validate the significance of these relationships? Specifically, which features strongly predict petal width?**

---

## Analysis Steps
1. **Exploratory Data Analysis (EDA)**:
   - Visualized distributions of sepal and petal dimensions using histograms, density plots, and boxplots.
   - Identified potential patterns and differences between iris species.

2. **Linear Regression**:
   - Performed regression analysis to predict petal width.
   - Evaluated the model using Mean Squared Prediction Error (MSPE) and diagnostic checks.

3. **Model Selection**:
   - Used AIC, BIC, and Adjusted R² criteria to identify the best model.
   - Applied Best Subset Regression to evaluate predictor combinations.

4. **Generalized Linear Modeling (GLM)**:
   - Addressed non-normality and non-linearity by applying a GLM with a Gamma family and log link.

5. **Diagnostics**:
   - Assessed residuals for violations of linear regression assumptions, including normality, independence, and constant variance.

6. **ANOVA**:
   - Compared multiple models to evaluate the statistical significance of predictors.

---

## Results
- **Linear Regression**:
  - Best model included Sepal.Length, Sepal.Width, and Petal.Length.
  - High predictive accuracy with an MSPE of 0.09499934 and Adjusted R² of 95.33%.
  - Petal.Length emerged as the strongest predictor of Petal.Width.

- **Diagnostics**:
  - Detected violations in normality, independence, and homoscedasticity.
  - Highlighted limitations in the linear regression model.

- **GLM**:
  - Applied Gamma family and log link.
  - Higher MSPE (0.3253174) than the linear model, indicating less effective performance.

- **Model Selection**:
  - Models with Sepal.Length, Sepal.Width, and Petal.Length consistently identified as the best across AIC, BIC, and Adjusted R² criteria.

---

## Conclusions
- Linear regression effectively predicted petal width but showed some diagnostic violations.
- The GLM approach, while addressing diagnostic issues, did not outperform linear regression in prediction accuracy.
- Sepal.Length, Sepal.Width, and Petal.Length are key predictors of Petal.Width.

---

## Future Work
1. Integrate interaction terms in regression models to assess combined effects of predictors.
2. Explore species-specific variations through expanded ANOVA analyses.
3. Experiment with polynomial regression to evaluate non-linear relationships.

---

## References
1. [Cecilia Lee's Analysis on RPubs](https://rpubs.com/cecilialee/iris)
2. [Exploratory Analysis with R](https://xiaorui.site/Data-Mining-R/lecture/2.A_ExploratoryAnalyses.html)
3. Diagnostic_plots.ipynb file from Professor
4. Homework-5 (submitted as part of coursework)
5. [Medium Post: Statistical Analysis of Iris Dataset](https://medium.com/@elsasaji02/an-exploration-of-the-iris-dataset-through-fundamental-statistical-analysis-with-r-programming-9e0ed52f2acd)

---

## How to Use
1. Clone this repository:
   ```bash
   git clone <repository_url>
   cd Statistical-Analysis-Iris-Data
