CUSTOMER LIFETIME VALUE (CLV) PREDICTOR
========================================

Predicts customer lifetime value from purchase data using RFM (Recency,
Frequency, Monetary) analysis and regression models, with a Streamlit
dashboard for predictions and analytics.


PROJECT STRUCTURE
------------------

app.py                 - Streamlit dashboard (prediction + analytics)

customer_transactions.csv      - Sample transaction data

notebooks/
  data_preprocessing_feature_engineering.ipynb
      Cleaning, feature engineering, preprocessing pipeline
  rfm_analysis_and_modeling.ipynb
      RFM segmentation + regression model comparison

artifacts/
  clv_features.csv               - Preprocessed data
  rfm_customer_segments.csv      - Customer-level RFM table with segment labels
  model.pkl                      - Trained model
  preprocessor.pkl               - Fitted preprocessor

requirements.txt


SETUP
-----

pip install -r requirements.txt


RUN THE APP
-----------

streamlit run app.py

Opens at http://localhost:8501


NOTEBOOKS
---------

1. notebooks/data_preprocessing_feature_engineering.ipynb
   Walks through data cleaning, feature engineering, and preprocessing
   on the raw CSV.

2. notebooks/rfm_analysis_and_modeling.ipynb
   Performs RFM (Recency, Frequency, Monetary) analysis to segment
   customers into tiers (Champions, Loyal Customers, Potential
   Loyalists, At Risk, Lost), trains and compares Linear Regression
   and Random Forest regression models to predict customer lifetime
   value, and visualizes segment behavior and feature importance to
   support marketing strategy.


KEY RESULTS
-----------

- RFM segmentation cleanly separates customers by value: Champions
  average about 3.4x the total spend of Lost customers, based on
  recency, frequency, and monetary quartile scoring.

- A Random Forest regressor outperforms a simple Linear Regression
  baseline for predicting customer lifetime value (higher R-squared,
  lower error), with purchase frequency and average order value as
  the strongest predictors.


TECH STACK
----------

Python, Pandas, NumPy, Scikit-learn, Matplotlib, Streamlit, Altair
