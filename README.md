# 🏥 Insurance Charges Prediction

This project explores a health insurance dataset to understand the factors influencing medical charges and build predictive models.

A logarithmic transformation was applied to the target variable (charges) to handle skewness and reduce the effect of outliers, leading to improved model performance.

📌 Dataset Description

age → Age of the individual

sex → Male/Female

bmi → Body Mass Index (health/obesity measure)

children → Number of dependents

smoker → Smoking status (yes/no)

region → Residential area (northeast, northwest, southeast, southwest)

charges → Medical insurance cost (target, log-transformed for modeling)

🎯 Purpose of Analysis

Predict medical insurance charges using regression models.

Compare Linear Regression, Ridge, Lasso, and Polynomial Regression after applying log transformation.

Evaluate models using R², MAE, MSE, and RMSE.

📊 Results Summary After Log Transformation

Linear Regression

R²: 0.803 → Explains ~80% variance

MAE: 0.275

MSE: 0.177

Ridge Regression

R²: 0.803

MAE: 0.28

RMSE: 0.42

Lasso Regression

R²: 0.803

MAE: 0.27

RMSE: 0.42

Polynomial Regression

R²: 0.861 → Higher than Linear, Ridge, and Lasso

Captures non-linear relationships between features and the target

More flexible but less interpretable, with potential risk of overfitting if polynomial degree is too high

📌 Key Insights

Log transformation improved stability and reduced the impact of extreme high-cost outliers.

Linear, Ridge, and Lasso perform very similarly, with Lasso offering slight feature selection benefits.

Polynomial Regression outperforms all linear-based models, showing that non-linear patterns exist in the data.

However, interpretability decreases and careful degree selection is important to avoid overfitting.

MAE ≈ 0.27 (log scale) → When exponentiated, this corresponds to exp(0.27) ≈ 1.30.

**This means that on average, the Polynomial regression model’s predictions are about 22 % higher or lower than the actual insurance charges.**

📈 Visualizations

Predicted vs Actual (log-charges)

Shows closer alignment with the perfect-fit line in Polynomial Regression compared to Linear Regression.

🚀 Next Steps

Explore advanced non-linear models (Random Forest, XGBoost) for further improvement.

Compare them with Polynomial Regression to check trade-offs between accuracy and interpretability.

👩‍💻 Author

Project by Sonia Firdous.

Special thanks to my teacher Aqsa Moiz for guidance 🙏
