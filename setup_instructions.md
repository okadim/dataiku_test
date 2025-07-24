# Setup Instructions

## Quick Start

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

## Project Files

### Input Data
- `analysis.ipynb` - Main analysis notebook
- `census_income_learn.csv` / `census_income_test.csv` - Datasets
- `census_income_metadata.txt` - Dataset information
- `requirements.txt` - Dependencies

### Model Outputs (generated after running analysis)
- `catboost_income.model` - Trained CatBoost model (saved using joblib)
- `threshold.json` - Optimal classification threshold for the model
- `catboost_info/` - CatBoost training logs, cross-validation results, and diagnostics

*Requires Python 3.8+* 