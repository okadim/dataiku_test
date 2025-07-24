# Census Income Analysis - Dataiku Assessment

This repository contains my solution to the Dataiku Data Scientist Technical Assessment, which focuses on predicting income levels (>$50K vs ≤$50K) using US Census data.

## 📋 Project Overview

The project involves building a machine learning pipeline to identify characteristics associated with earning more or less than $50,000 per year using a dataset of ~300,000 anonymized individuals from the US Census archive.

## 🎯 Key Components

- **Exploratory Data Analysis**: Comprehensive analysis of demographic and economic patterns
- **Data Preprocessing**: Advanced cleaning, feature engineering, and missing value handling  
- **Machine Learning Models**: CatBoost gradient boosting with hyperparameter optimization
- **Model Interpretability**: SHAP analysis for feature importance and prediction explanations
- **Performance Evaluation**: Detailed metrics, calibration, and threshold optimization

## 📊 Presentation

The complete presentation and findings can be found in:
**`Dataiku - Predicting Income Levels Using US Census Data (2).pdf`**

## 🚀 Quick Start

1. **Create and activate virtual environment:**
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate  # macOS/Linux
   # .venv\Scripts\activate   # Windows
   ```

2. **Install dependencies and start Jupyter:**
   ```bash
   pip install -r requirements.txt
   jupyter notebook
   ```

3. **Open `analysis.ipynb` in your browser**

## 📁 Project Files

### Input Data
- `analysis.ipynb` - Main analysis notebook
- `census_income_learn.csv` / `census_income_test.csv` - Datasets
- `census_income_metadata.txt` - Dataset information
- `requirements.txt` - Dependencies

### Model Outputs (generated after running analysis)
- `catboost_income.model` - Trained CatBoost model (saved using joblib)
- `threshold.json` - Optimal classification threshold for the model
- `catboost_info/` - CatBoost training logs, cross-validation results, and diagnostics

### Documentation
- `Dataiku - Predicting Income Levels Using US Census Data (2).pdf` - Complete presentation
- `setup_instructions.md` - Detailed setup guide

## 🔧 Requirements

*Requires Python 3.8+*

## 📈 Key Results

- **AUC-ROC**: 0.956 on test set
- **Optimal F1-Score**: 0.63 with balanced precision/recall
- **Top Features**: Age, Education, Weeks Worked, Occupation, Capital Gains

The final model demonstrates strong predictive performance while maintaining interpretability through SHAP analysis.
