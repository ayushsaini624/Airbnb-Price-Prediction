# Airbnb-Price-Prediction 🏠💸

Predicting nightly Airbnb listing prices using data exploration, feature engineering, and machine learning. This project walks through the full workflow—from raw data to a trained model—so others can reproduce results and extend the work.

Project Highlights

Goal: Build a model that estimates the nightly price of an Airbnb listing.

Scope: EDA → Data Cleaning → Feature Engineering → Model Training → Evaluation → Explainability.

Tech: Python, Pandas, NumPy, scikit-learn, Matplotlib, XGBoost/LightGBM, SHAP.

Repository Structure

data/ → raw and processed datasets

notebooks/ → main end-to-end Jupyter notebook

src/ → Python scripts for preprocessing, feature engineering, training, and utilities

models/ → trained model artifacts (ignored in git by default)

requirements.txt and environment.yml → dependencies

README.md and LICENSE

Problem Statement

Given listing metadata (location, property type, room type, amenities, host attributes, reviews, etc.), predict the nightly price.
Applications include:

Helping hosts set competitive prices

Supporting platforms in dynamic pricing or quality checks

Providing price estimates for new listings with limited history

Data

Source: Public Airbnb listing data (Inside Airbnb, Kaggle, or curated datasets)

Target variable: price

Example features:

Categorical: room_type, property_type, neighbourhood, cancellation_policy

Numerical: accommodates, bathrooms, bedrooms, beds, minimum_nights, availability_365, number_of_reviews, review_scores_rating

Derived: amenities count, host experience, seasonal features, geospatial distance to city center

Methodology

Exploratory Data Analysis: distributions, missing values, outliers, correlations

Preprocessing: imputation, encoding categorical variables, scaling, log-transforming price

Modeling: Linear Regression, Ridge/Lasso, Random Forest, Gradient Boosting, XGBoost/LightGBM

Evaluation: RMSE, MAE, R² with cross-validation, plus residual analysis

Explainability: Feature importance and SHAP values

Results (example)

Linear Regression: RMSE 35.2, MAE 22.9, R² 0.58

Random Forest: RMSE 28.4, MAE 18.3, R² 0.72

XGBoost: RMSE 26.9, MAE 17.4, R² 0.75 (best)

Reproducibility

Notebook runs end-to-end on Google Colab with uploaded dataset.

Environment files provided for local setup (requirements.txt or environment.yml).

Feature Engineering Ideas

Amenity richness score

Host reliability signals (response rate, superhost status)

Seasonal and calendar features

Geospatial features (distance to landmarks/city center)

Explainability

Global: Feature importance and permutation importance

Local: SHAP values to explain individual predictions

Model Card (Quick Summary)

Intended use: Educational and exploratory pricing insights

Not intended for: Financial decision-making without expert review

Limitations: Biases from dataset, missing seasonal trends, sensitive to incorrect or incomplete data

Future Work

Build city-specific or hierarchical models

Add time-series and seasonal effects

Use advanced NLP for amenities


Acknowledgements

Open datasets from Inside Airbnb and Kaggle

Libraries: scikit-learn, XGBoost/LightGBM, SHAP

Contact

Author: Ayush Saini
Email: ayushsaini624@gmail.com
