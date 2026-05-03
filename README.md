# COMP90049 Assignment 2 — UK Used Car Price Prediction

**Group Members:** Zhenyu Zhang, Xinkai Zhang, Yiming Zhang, Yifan Wu  
**Subject:** Introduction to Machine Learning, Semester 1 2026  
**University of Melbourne**

## Dataset

**UK Used Car Dataset**  
Source: https://www.kaggle.com/datasets/adityadesai13/used-car-dataset-ford-and-mercedes  
License: CC0 Public Domain

The dataset contains ~108,000 listings of used cars in the UK across 11 brands (Audi, BMW, Ford, Mercedes, VW, etc.), with features including model, year, price, transmission, mileage, fuel type, tax, mpg, and engine size.

> **Note:** Raw data files are not included in this repository. Please download the dataset from the Kaggle link above and place the CSV files in `code/data/`.

## Research Questions

1. To what extent can machine learning models accurately predict used car prices based on available features?
2. How do different types of models (linear, instance-based, tree-based, neural networks) compare in predictive performance and generalisation?
3. How do different data preprocessing strategies (scaling, missing value handling, encoding) affect model performance?
4. Which features contribute most significantly to price prediction, and how can feature importance be interpreted?

## Project Structure

```
Assignment2/
├── README.md
├── requirements.txt
├── AGENT.md                    # Assignment requirements reference
├── code/
│   ├── data/                   # Raw CSV files (not tracked by git)
│   │   └── processed/          # Cleaned dataset output
│   └── notebooks/
│       ├── 01_data_preprocessing.ipynb   # EDA, cleaning, feature engineering
│       ├── 02_baseline_models.ipynb      # Linear Regression, KNN
│       ├── 03_advanced_models.ipynb      # SVM, Random Forest, Neural Network
│       └── 04_results_analysis.ipynb     # Comparison, feature importance
└── report/
```

## How to Run

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Download the dataset from Kaggle and place all CSV files in `code/data/`
4. Run notebooks in order: `01_` → `02_` → `03_` → `04_`

## Evaluation Metrics

- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- R² (Coefficient of Determination)
- Cross-validation (5-fold)
