# COMP90049 Assignment 2 - UK Used Car Price Prediction

**Subject:** Introduction to Machine Learning, Semester 1 2026  
**University:** The University of Melbourne

## Project Overview

This project predicts UK used-car listing prices using supervised machine learning. It compares linear, instance-based, tree-based, ensemble, and neural network models, and analyses how preprocessing choices such as missing-value imputation, categorical encoding, feature engineering, and scaling affect predictive performance.

## Dataset

**Dataset:** UK Used Car Dataset  
**Source:** https://www.kaggle.com/datasets/adityadesai13/used-car-dataset-ford-and-mercedes  
**License:** CC0 Public Domain

The dataset contains approximately 108,000 UK used-car listings across multiple brands, including Audi, BMW, Ford, Mercedes-Benz, Toyota, Vauxhall, Volkswagen, and others. The main raw features include model, year, price, transmission, mileage, fuel type, tax, mpg, and engine size.

Raw dataset files should be downloaded from Kaggle and placed in `code/data/`. The raw CSV files are not required in the submitted code package if the dataset source is provided.

## Research Questions

1. To what extent can machine learning models accurately predict used-car prices from available vehicle attributes?
2. How do different model families compare in predictive performance and generalisation?
3. How do preprocessing strategies such as scaling, missing-value handling, encoding, and feature engineering affect performance?
4. Which vehicle features contribute most strongly to price prediction?

## Project Structure

```text
IML-A2/
  README.md
  requirements.txt
  code/
    data/
      processed/
        cars_cleaned.csv
        fig*.png
    notebooks/
      01_data_preprocessing.ipynb
      02_model_training_and_comparison.ipynb
    outputs/
      model_training_comparison/
        model_metrics_train_dev_test.csv
        best_hyperparameters.csv
        scaling_comparison.csv
        cross_validation_results.csv
        random_forest_feature_importance.csv
        ridge_feature_coefficients.csv
        figures/
  report/
    main.tex
    main.pdf
    sections/
```

## How to Run

1. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

2. Download the raw dataset from Kaggle and place the CSV files in `code/data/`.

3. Run the notebooks in order:

   ```text
   code/notebooks/01_data_preprocessing.ipynb
   code/notebooks/02_model_training_and_comparison.ipynb
   ```

4. Generated cleaned data, figures, metrics, predictions, and feature-importance outputs are saved under:

   ```text
   code/data/processed/
   code/outputs/model_training_comparison/
   ```

## Models

The project evaluates:

- Ridge Regression
- KNN Regression
- Decision Tree
- Random Forest
- MLP Neural Network

## Evaluation Metrics

Model performance is reported using:

- MAE
- RMSE
- Price-scale R^2
- Supplementary 3-fold cross-validation

## Report

The final report source is in `report/`, and the compiled PDF is:

```text
report/main.pdf
```
