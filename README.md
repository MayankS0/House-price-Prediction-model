🏠 House Price Prediction & Analysis
📌 Overview

This project focuses on building a machine learning model to predict house prices and analyzing the key factors that influence pricing.
The goal is not just prediction, but also deriving data-driven insights from real estate data.

🚀 Problem Statement

Accurately predicting house prices is challenging due to multiple influencing factors such as location, size, and property features.
This project aims to:

Build a reliable prediction model
Identify the most important factors affecting prices
Validate model performance on unseen data
📊 Dataset
Real-world housing dataset (structured data)
Features include:
Property size (SQFT)
Location (Latitude, Longitude)
Number of BHK
City category
Seller type (Dealer/Owner)
RERA compliance
⚙️ Tech Stack
Python
Pandas, NumPy → Data manipulation
Matplotlib, Seaborn → Visualization
Scikit-learn → Machine Learning
🔍 Workflow
1. Data Preprocessing
Handled missing values
Applied log transformation (LOG_SQFT)
One-hot encoding for categorical features
Feature scaling using StandardScaler
2. Exploratory Data Analysis (EDA)
Analyzed price distribution
Identified relationships between features
Visualized correlations
3. Model Building

Trained and compared multiple models:

Ridge Regression
Random Forest ✅ (Best)
Gradient Boosting
4. Model Evaluation
Model	MAE	RMSE	R²
Ridge Regression	78.39	39616.24	0.18
Random Forest	26.31	9970.97	0.79
Gradient Boosting	29.82	10096.92	0.79

👉 Best Model: Random Forest

📈 Key Insights
Property Size (LOG_SQFT) → ~53% importance (strongest driver)
Location (Lat + Long) → ~25% combined impact
Resale factor also plays a significant role
City tier and seller type have comparatively lower influence
📉 Model Validation
Compared training data distribution vs test predictions
Both distributions show a similar right-skewed pattern
Confirms that the model generalizes well and avoids overfitting

💡 Learnings
Importance of feature engineering in improving model performance
Tree-based models outperform linear models for non-linear data
Model evaluation should go beyond accuracy → distribution & insights matter
🔗 Future Improvements
Hyperparameter tuning (GridSearchCV)
Model deployment (Flask/Streamlit)
Integration with a dashboard (Power BI / Tableau)
🤝 Connect With Me

If you have feedback or opportunities in Data Analytics / Data Science, feel free to connect!

⭐ If you found this useful

Give this repo a star ⭐
