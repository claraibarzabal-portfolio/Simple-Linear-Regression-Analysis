# Simple-Linear-Regression-Analysis
A detailed exploration and analysis of a dataset containing SAT and GPA scores to understand the relationship between these two variables. The goal is to apply simple linear regression, handle outliers, perform various data transformations, and explore polynomial regression to predict a student's GPA based on their SAT score.

## Dataset

The dataset used in this project is sourced from Kaggle: [101 Simple Linear Regression.csv](https://www.kaggle.com/datasets/luddarell/101-simple-linear-regressioncsv?resource=download). It consists of observations on two variables:
- **SAT**: Student's SAT scores.
- **GPA**: Student's GPA.

## Files Description

- `data_101_simple_linear_regression.csv`: The original dataset file.
- `Simple_Linear_Regression_with_Outliers_and_Transformations.ipynb`: Jupyter notebook for simple linear regression analysis.
- `Different_Transformations_for_Linear_Regression.ipynb`: This Jupyter notebook delves into various data transformations to enhance the performance of linear regression models. It examines the effects of transformations such as logarithmic, square root, inverse, Box-Cox, and Yeo-Johnson on the model's Mean Squared Error (MSE) and R-squared (R^2) values. The analysis seeks to identify which transformation(s) lead to more accurate and reliable predictive outcomes. It's an insightful exploration for those looking to deepen their understanding of preprocessing techniques in linear regression analysis.
- `Polynomial_Regression.ipynb`: Jupyter notebook for polynomial regression analysis.

## How to Run

1. Clone this repository to your local machine.
2. Ensure you have Jupyter Notebook installed or use Google Colab to open the `.ipynb` files.
3. Run each notebook cell to see the analysis process and results.

## Results and Conclusions

### Key Findings:
- The exploration of data transformations and polynomial regression models has led to insightful discoveries regarding the relationship between SAT scores and GPA.
- Different transformations and model complexities were experimented with to optimize model performance.

### Statistical Metrics and Visualizations:
- **Original Model Performance:** MSE: 6413.13, R^2: 0.406. The initial analysis indicated room for improvement in both prediction accuracy and variability explanation.
- **Logarithmic Transformation:** Significantly reduced MSE to 0.00188 while slightly improving R^2 to 0.409. This highlights an increase in prediction accuracy.
- **6th-degree Polynomial Model:** Presented a better balance between MSE (6071.66) and R^2 (0.438), suggesting an enhanced model fit.

### Conclusions:
Upon reviewing the Mean Squared Error (MSE) and the Coefficient of Determination (R^2), it became clear that each transformation and model adjustment uniquely impacted the prediction accuracy and fit.

- **Logarithmic Transformation** emerged as a powerful method for minimizing MSE, which suggests a high precision in predictions. However, its impact on R^2 was marginal, indicating only a slight improvement in explaining the variability within the dependent variable.
- **6th-degree Polynomial Model** did not achieve the lowest MSE but demonstrated a considerable enhancement in R^2. This suggests a superior overall model fit, providing a more comprehensive explanation of the data variability without a significant compromise on prediction accuracy.

Given these observations, the choice between minimizing prediction error through logarithmic transformation and enhancing the explanation of variability via a 6th-degree polynomial model hinges on the specific objectives of the analysis and the practical application of the models. Therefore, both approaches offer valuable insights, with the final selection tailored to the aims of the study and its implications in practice.

## Technologies Used

This project was developed using Python and a variety of libraries that are part of the data science ecosystem in Python. Here's a breakdown of the main tools and libraries used:

- **Python:** The core programming language of the project, providing a versatile environment for data manipulation, analysis, and visualization.

- **Pandas:** A powerful library for data manipulation and analysis, used for reading and manipulating the dataset.

- **NumPy:** Essential for numerical operations, especially useful for handling arrays and performing a wide array of mathematical operations.

- **Matplotlib:** One of the primary libraries for creating static, interactive, and animated visualizations in Python. Used extensively for plotting graphs and charts.

- **Seaborn:** Built on top of Matplotlib, Seaborn provides a high-level interface for drawing attractive and informative statistical graphics. It's used to enhance the visualization aspect of the analysis.

- **scikit-learn:** A leading machine learning library that provides simple and efficient tools for data analysis and modeling. It was used for:
  - Implementing linear regression and polynomial regression models.
  - Generating polynomial features.
  - Computing mean squared error (MSE) and the coefficient of determination (R²) to evaluate model performance.

- **SciPy (stats):** A library used for scientific and technical computing. Within this project, the `stats` module from SciPy was utilized for more advanced statistical functions and transformations.

- **Math (sqrt):** Part of Python's standard library, the `sqrt` function from the `math` module was used to calculate the square root, specifically for computing the root mean square error (RMSE).

These tools collectively supported the exploration, analysis, and modeling phases of the project, enabling the detailed investigation of the relationship between SAT scores and GPA.


## Acknowledgements

- Dataset provided by [Kaggle](https://www.kaggle.com/).

