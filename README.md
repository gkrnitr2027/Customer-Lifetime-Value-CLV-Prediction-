# Customer Lifetime Value (CLV) Predictor

<<<<<<< HEAD
Predicts customer lifetime value from purchase data using RFM (Recency, Frequency, Monetary) analysis and
regression models, with a Streamlit dashboard for predictions and analytics.
=======
Predicts customer lifetime value from purchase data using a trained Random Forest model, with a Streamlit dashboard for predictions and analytics.
>>>>>>> 5f93856c156dbce088d83ef1791b2b006964c236

## Project Structure

|── streamlit_app.py          # Streamlit dashboard (prediction + analytics)
├── data/
│   └── customer_transactions.csv # Sample transaction data
├── notebooks/
<<<<<<< HEAD
│   ├── data_preprocessing_feature_engineering.ipynb   # Cleaning, feature engineering, preprocessing pipeline
│   └── rfm_analysis_and_modeling.ipynb                # RFM segmentation + regression model comparison
├── artifacts/
|   |
|___├── clv_features.csv           # Preprocessed data
│   ├── rfm_customer_segments.csv  # Customer-level RFM table with segment labels
│   ├── model.pkl                  # Trained model
│   └── preprocessor.pkl           # Fitted preprocessor
=======
│   └── data_preprocessing_feature_engineering.ipynb
├── artifacts/
|   |
|___├── clv_features.csv          # Preprocessed data
│   ├── model.pkl                 # Trained model
│   └── preprocessor.pkl          # Fitted preprocessor
>>>>>>> 5f93856c156dbce088d83ef1791b2b006964c236
└── requirements.txt

## Setup

pip install -r requirements.txt

## Run the app

streamlit run streamlit_app.py

Opens at http://localhost:8501

<<<<<<< HEAD
## Notebooks

- `notebooks/data_preprocessing_feature_engineering.ipynb` walks through data cleaning, feature engineering,
  and preprocessing on the raw CSV.
- `notebooks/rfm_analysis_and_modeling.ipynb` performs RFM (Recency, Frequency, Monetary) analysis to segment
  customers into tiers (Champions, Loyal Customers, Potential Loyalists, At Risk, Lost), trains and compares
  Linear Regression and Random Forest regression models to predict customer lifetime value, and visualizes
  segment behavior and feature importance to support marketing strategy.

## Key Results

- RFM segmentation cleanly separates customers by value: **Champions** average ~3.4x the total spend of
  **Lost** customers, based on recency, frequency, and monetary quartile scoring.
- A Random Forest regressor outperforms a simple Linear Regression baseline for predicting customer lifetime
  value (higher R², lower error), with purchase frequency and average order value as the strongest predictors.

## Tech Stack

Python, Pandas, NumPy, Scikit-learn, Matplotlib, Streamlit, Altair
=======
## Notebook

notebooks/data_preprocessing_feature_engineering.ipynb walks through data cleaning, feature engineering, and preprocessing on the raw CSV.

## Tech Stack

Python, Streamlit, scikit-learn, pandas, Altair
>>>>>>> 5f93856c156dbce088d83ef1791b2b006964c236
