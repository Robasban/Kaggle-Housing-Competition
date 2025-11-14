# Kaggle Housing Competition

A comprehensive machine learning pipeline for predicting house prices using XGBoost, scikit-learn, and advanced feature engineering. This project demonstrates end-to-end model development with GridSearchCV optimization and cross-validation evaluation.

## Overview

This repository contains a complete solution for the Kaggle House Prices competition, featuring:
- **Advanced preprocessing** with ordinal and one-hot encoding strategies
- **Feature engineering** creating derived features (TotalSF, TotalBath, SellAge, OverallRating)
- **Hyperparameter tuning** via GridSearchCV with 5-fold cross-validation
- **XGBoost regression model** with optimized parameters (n_estimators=621, max_depth=2, learning_rate=0.125)
- **Model evaluation** with RMSE and R² metrics

## Project Structure

```
.
├── int-adv-ml-xgboost-gridcv-pipeline-housing.ipynb  # Main analysis notebook
├── train.csv                                           # Training data
├── test.csv                                            # Test data
├── requirements.txt                                    # Python dependencies
├── .gitignore                                          # Git ignore rules
├── README.md                                           # This file
└── LICENSE                                             # MIT License
```

## Results

- **Best Local CV RMSE:** ~0.118 (slight variance due to environment differences)
- **Kaggle Submission RMSE:** 0.1164
- **Average R²:** 0.915

## Getting Started

### Prerequisites
- Python 3.7+
- pip

### Installation

1. **Clone the repository:**
```bash
git clone https://github.com/Robasban/Kaggle-Housing-Competition.git
cd Kaggle-Housing-Competition
```

2. **Create and activate a virtual environment:**
```bash
python3 -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

3. **Install dependencies:**
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### Running the Notebook

Launch Jupyter Lab or Notebook:
```bash
jupyter lab
# or
jupyter notebook
```

Open `int-adv-ml-xgboost-gridcv-pipeline-housing.ipynb` and select the kernel `kaggle-housing-venv` when prompted.

## Notebook Walkthrough

1. **Data Loading & Exploration** — Load train/test data and examine shape/structure
2. **Feature Identification** — Categorize columns into ordinal, one-hot, and numerical
3. **Feature Engineering** — Create derived features and handle missing values
4. **Pipeline Construction** — Build preprocessing and modeling pipeline
5. **Hyperparameter Tuning** — GridSearchCV to optimize XGBoost parameters
6. **Model Evaluation** — Cross-validation RMSE and R² scoring
7. **Feature Importance** — Permutation importance analysis
8. **Prediction & Submission** — Generate predictions on test set

## Key Libraries

- **scikit-learn** — Preprocessing, pipelines, model selection
- **xgboost** — Gradient boosting regressor
- **pandas** — Data manipulation and analysis
- **numpy** — Numerical computing

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Feel free to open issues or submit pull requests to improve the analysis or model performance.

## Acknowledgments

- Kaggle for the House Prices dataset
- scikit-learn and XGBoost communities for excellent ML libraries
