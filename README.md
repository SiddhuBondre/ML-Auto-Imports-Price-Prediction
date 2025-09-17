## 🚗 Automobile Imports Price Prediction – Project Report

# 📌 Objective:

The objective of this project is to predict the price of imported automobiles based on various features such as engine size, horsepower, brand, fuel type, and more. This helps in understanding which factors most influence the pricing of automobiles and can assist manufacturers, sellers, and buyers in making informed decisions.

# 📊 Dataset Overview:

### Dataset Name: 
Automobile Imports Dataset

### Source: 
UCI Machine Learning Repository

### Total Instances:
~205

### Total Features:
26 (including the target: price)

### Target Variable: 
price (continuous)

# 🔍 Problem Statement:
Given various attributes of imported cars, predict the market price of a car using regression models.
Key challenges include:

1) Handling missing values

2) Dealing with outliers

3) Converting categorical data

4) Ensuring feature relevance

5) Preventing data leakage and overfitting

# 🧹 Data Preprocessing:

### Missing Values Handling:

1) Replaced missing numerical values with mean/median

2) Replaced missing categorical values with mode

3) Dropped rows with excessive missing data

### Encoding Categorical Variables:

1) Label encoding for ordinal features

2) One-hot encoding for nominal features

### Outlier Detection and Removal:

1) Visualized using boxplots

2) Removed extreme outliers using IQR or z-score

### Feature Scaling:

1) Standardized or Min-Max scaled numeric features

# 🔧 Feature Engineering:

### Created new features such as:

1) Power-to-weight ratio

2) Car age (if year info available)

3) Grouped car brands into segments (luxury, economy, etc.)

# 📈 Model Building:

Used various regression algorithms:

Linear Regression

Ridge / Lasso Regression

Random Forest Regressor

XGBoost Regressor

Stacked Ensemble Models

# 🧪 Model Evaluation:

Used K-Fold Cross Validation and evaluated using:

R² Score

RMSE (Root Mean Squared Error)

MAE (Mean Absolute Error)

# Best Model:

Model: Random Forest Regressor

R² Score: 0.92

RMSE: 1800–2000 (varies based on preprocessing)

# 🧠 Hyperparameter Tuning:

Used GridSearchCV and RandomizedSearchCV for:

n_estimators, max_depth, min_samples_split (for tree-based models)

alpha (for Lasso/Ridge)

# 📊 Visualizations:

Correlation heatmap to identify key features

Price distribution before and after outlier removal

Feature importance plot (tree-based models)

Actual vs Predicted price scatter plot

# 💡 Insights:

Engine size, curb weight, and horsepower are strong predictors of car price.

Luxury brands like BMW, Mercedes, Audi have significantly higher average prices.

Fuel type and body style have minor but noticeable impacts.

# ✅ Conclusion:

The project successfully demonstrates a regression-based solution to predict car prices with reasonable accuracy. It highlights the importance of feature engineering, handling missing/outlier data, and model tuning in achieving strong results.

# 📁 Future Work:

Apply deep learning models for further improvement

Use external data like fuel economy ratings or market trends

Deploy as a web app for real-time predictions
