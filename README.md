📌 Overview

This project predicts Airbnb listing prices using machine learning models. The aim is to help hosts and guests better understand pricing dynamics based on features like location, room type, reviews, and host behavior.

The dataset was provided by Internshala platform during my Data Science training internship.

🎯 Objectives

Perform Exploratory Data Analysis (EDA) to understand Airbnb listings.

Handle outliers and preprocess data effectively.

Build and evaluate multiple regression models.

Use hyperparameter tuning (GridSearchCV) to improve performance.

Compare models and select the best-performing algorithm.

🛠️ Technologies & Tools Used

Python 🐍

Libraries: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, XGBoost

Jupyter Notebook

📊 Dataset

Source: Internshala (provided for training purposes)

Features include:

accommodates, bathrooms, bedrooms, beds

host_response_rate, number_of_reviews, review_scores_rating

latitude, longitude

Target variable: price

🔎 Exploratory Data Analysis (EDA)

Identified outliers in key features

Visualized distributions and relationships between variables

📷 Example (Outlier Detection):


🤖 Model Building & Evaluation

Models used:

Initial Random Forest

Initial XGBoost

Tuned Random Forest (GridSearchCV)

Tuned XGBoost (GridSearchCV)

📷 Model Comparison:


📈 Performance Summary

Initial XGBoost → RMSE: 0.3763, MAE: 0.2732, R²: 0.5812

Initial Random Forest → RMSE: 0.3795, MAE: 0.2719, R²: 0.5740

Tuned XGBoost → Best performance with GridSearchCV

Tuned Random Forest → Improved but not better than XGBoost

✅ Final Model Selected: Tuned XGBoost
