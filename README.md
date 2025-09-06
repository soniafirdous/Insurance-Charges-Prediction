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

Compare Linear Regression, Ridge, and Lasso after applying log transformation.

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

📌 Key Insight: Log transformation improved stability and reduced the impact of extreme high-cost outliers. All three models perform very similarly, with Lasso offering slight feature selection benefits.

MAE ≈ 0.27 (log scale) → When exponentiated, this corresponds to exp(0.27) ≈ 1.30.

This means that on average, the model’s predictions are about 30% higher or lower than the actual insurance charges.

📈 Visualizations

Predicted vs Actual (log-charges) scatter plot shows better alignment with the perfect fit line compared to the untransformed version.

Distribution of residuals is more normal after transformation.

🚀 Next Steps

Explore non-linear models (Random Forest, XGBoost) for further improvement.

👩‍💻 Author

Project by Sonia Firdous.

Special thanks to my teacher Aqsa Moiz for guidance 🙏
