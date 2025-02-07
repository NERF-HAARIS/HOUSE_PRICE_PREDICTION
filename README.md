# HOUSE_PRICE_PREDICTION

## Model Comparison Visualization
![Screenshot (166)](https://github.com/user-attachments/assets/3cde4b0d-15a5-44c1-89f2-d7ccd49042f7)

## Overview
This project aims to build a predictive model for house prices using machine learning techniques. The dataset undergoes preprocessing steps, including handling missing values, encoding categorical variables, standardizing numerical features, and removing multicollinearity. The final model is selected using hyperparameter tuning.

## Features and Techniques Used
1. Data Preprocessing
Loaded the dataset and performed exploratory data analysis (EDA).
Handled missing values dynamically:
Numerical: Filled with median values.
Categorical: Filled with mode values.
Dropped columns with more than 50% missing values.
2. Feature Engineering
One-hot encoding for categorical variables using OneHotEncoder.
Standardized numerical features using StandardScaler within ColumnTransformer.
Created a new feature AgeAtSale = YrSold - YearBuilt.
Dropped YrSold and YearBuilt after feature extraction.
3. Multicollinearity Handling
Calculated Variance Inflation Factor (VIF) to detect multicollinearity.
Dropped high VIF columns (VIF >= 10) to improve model performance.
4. Model Training & Selection
Split data into train and test sets.
Implemented Linear Regression, Ridge, and Lasso regression models.
Hyperparameter tuning using GridSearchCV for Ridge and Lasso.
Selected the best model based on validation R² score.
5. Model Evaluation & Visualization
Computed RMSE, MAE, and R² scores for train and test sets.
Plotted residual distributions to analyze prediction errors.
Created Predicted vs Actual SalePrice scatter plot to visualize model performance.
  
## Dataset
The dataset consists of various features describing houses, including lot size, number of rooms, construction year, and neighborhood information.




## Results & Findings
- The best-performing model was selected based on validation performance.
- Feature engineering and multicollinearity removal improved accuracy.
- Visualizations provide insights into model performance and residual analysis.



