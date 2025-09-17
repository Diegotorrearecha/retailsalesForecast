# Retail Sales Forecasting 🛒

This repository contains a machine learning project focused on **forecasting retail sales** using historical store data.  
It was built as part of a machine learning assignment and follows the common structure of Kaggle-style competitions (train/test datasets with a sample submission).

---

##  Repository structure
├── train.csv # Training dataset (features + target sales)

├── test.csv # Test dataset (features only, for predictions)

├── store.csv # Additional store metadata (e.g., store type, promo info)

├── sample_submission.csv # Example format for submission file

├── MLA2.ipynb # Main Jupyter notebook (data exploration, modeling, predictions)

└── README.md # Project documentation


---

##  Project overview
- **Objective:**  
  Build predictive models to forecast daily/weekly sales across different stores.

- **Datasets:**  
  - `train.csv`: contains historical sales along with features such as store ID, promotions, holidays, etc.  
  - `test.csv`: same structure but without sales, used to generate predictions.  
  - `store.csv`: descriptive metadata about each store (store type, assortment, competition).  
  - `sample_submission.csv`: template to format the final predictions for evaluation.  

- **Main steps in the notebook (`MLA2.ipynb`):**  
  1. Data loading and preprocessing (merging train/test with `store.csv`).  
  2. Feature engineering (lags, moving averages, categorical encodings).  
  3. Exploratory Data Analysis (EDA): correlations, seasonal patterns, promotions impact.  
  4. Model training and evaluation:
     - Linear Regression baseline
     - Decision Tree / Random Forest
     - Gradient Boosting (XGBoost/LightGBM, if available)
  5. Model selection and hyperparameter tuning.  
  6. Prediction generation for the `test.csv`.  
  7. Export of results in the `sample_submission.csv` format.  

---

##  Quickstart

###  Clone the repository
```bash
git clone https://github.com/Diegotorrearecha/retail-sales-forecasting.git
cd retail-sales-forecasting
