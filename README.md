**Objective**

To apply regression modeling techniques on real-world datasets by performing data preprocessing, feature engineering, model training, evaluation, visualization, and regularization, and to interpret model behavior using appropriate statistical metrics.

**Scenario 1: Student Academic Performance Prediction**
**Dataset:**

Kaggle – Students Performance in Exams Dataset

**Problem Type:**

Multilinear Regression

**Tasks Performed**

Imported essential libraries such as NumPy, Pandas, Matplotlib, and Scikit-learn.

Loaded the student performance dataset into a Pandas DataFrame.

Created the target variable as the average of Math, Reading, and Writing scores.

Generated additional numerical features such as:

Study hours per day

Attendance percentage

Sleep hours

Encoded categorical features (parental education level and test preparation course) using Label Encoding.

Handled missing values using median imputation.

Applied StandardScaler for feature scaling to ensure numerical stability.

Split the dataset into training and testing sets.

Trained a Multilinear Regression model using Ordinary Least Squares.

**Evaluated model performance using:**

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

R² Score

**Visualized:**

Predicted vs Actual Scores

Residual Distribution

Coefficient magnitude comparison

**Improved model performance using:**

Feature elimination

Ridge Regression (L2 regularization)

Lasso Regression (L1 regularization)

**Observations & Inferences**

Study hours and test preparation course showed strong positive influence on final exam scores.

Feature scaling improved numerical stability and helped regularization perform effectively.

Some correlation between features indicated mild multicollinearity.

Ridge regression stabilized coefficients and reduced variance in predictions.

Lasso regression reduced the impact of less significant features.

Residual plots showed approximately random distribution, supporting linear model assumptions.

**Scenario 2: Vehicle Fuel Efficiency Prediction**
**Dataset:**

Kaggle – Auto MPG Dataset

**Problem Type:**

Polynomial Regression

**Tasks Performed**

Imported required libraries for regression modeling and visualization.

Loaded the Auto MPG dataset into Pandas.

Selected horsepower as the independent variable and MPG as the target variable.

**Cleaned the dataset by:**

Replacing '?' with NaN

Converting horsepower to float

Filling missing values using median imputation

Generated polynomial features for degrees:

1

2

8

Applied StandardScaler after polynomial expansion.

Split the dataset into training and testing sets.

Trained Polynomial Regression models for different degrees.

**Evaluated performance using:**

MSE

RMSE

R² Score

Compared training and testing errors to analyze overfitting.

Applied Ridge regression to reduce overfitting.

**Visualized:**

Polynomial curve fitting

Training vs Testing error comparison

Residual distribution

**Observations & Inferences**

The relationship between horsepower and MPG was non-linear.

Degree 2 provided improved fit compared to linear regression.

Higher polynomial degrees reduced training error but increased test error, indicating overfitting.

Ridge regression smoothed the polynomial curve and reduced coefficient explosion.

Test error increased at higher degrees due to high variance.

The experiment clearly demonstrated the bias–variance tradeoff.

**Conclusion**

These experiments demonstrate the practical application of regression techniques in different domains:

Multilinear regression effectively models linear relationships with multiple influencing factors.

Polynomial regression captures non-linear patterns but requires careful control of complexity.

Regularization techniques such as Ridge and Lasso are essential to ensure model stability and generalization.

Proper preprocessing, feature scaling, evaluation metrics, and residual diagnostics are critical in building reliable machine learning models.
