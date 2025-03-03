# 🏆 Kaggle Playground Series: Backpack Price Prediction

This repository contains my solution for the **Kaggle Playground Series - Predicting Backpack Prices** competition.

## Link of Competition: https://www.kaggle.com/competitions/playground-series-s5e2


## 🚀 Competition Overview  
- **Task**: Predict the price of backpacks based on various attributes.
- **Evaluation Metric**: Root Mean Squared Error (RMSE)
- **Final Rank**: `1828`
- **Best RMSE Score**: `38.93292`

## 📊 Approach

### 🔹 Data Preprocessing
- Handled missing values
- Converted categorical variables using **Label Encoding** and **One-Hot Encoding**
- Feature Engineering (New features based on domain knowledge)

### 🔹 Models Used
- `RandomForestRegressor`
- `LightGBM`
- `XGBoost`
- `CatBoost`
- `Stacking` (LGBM, XGB, CatBoost)
- `Optuna` Hyperparameter Tuning
- `Ensemble` (Weighted combination of best models)

## 🏆 Final Submission Results
| Submission | Model | RMSE |
|------------|----------------|----------|
| **Featured_CatBoost_submission.csv** | Feature Engineered CatBoost | `38.93292` |
| final_ensemble_submission.csv | Ensemble (CatBoost, XGB, LGBM) | `38.94040` |
| stacking_submission.csv | Stacked Model (CatBoost, XGB, LGBM) | `38.94582` |
| Optuna_CatBoost_submission.csv | Optuna Tuned CatBoost | `38.95744` |
| submission4.csv | CatBoost | `38.96010` |
| submission3.csv | XGBoost | `39.09539` |
| submission2.csv | LGBMRegressor | `39.02232` |
| submission.csv | RandomForestRegressor | `40.09732` |

## 🔥 Challenges Faced
- Handling categorical features effectively for tree-based models.
- Finding the right hyperparameters using **Optuna**.
- Balancing bias and variance while ensembling models.
- Avoiding **overfitting** due to small dataset size.

## 📌 How to Reproduce
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/kaggle-backpack-price-prediction.git
   cd kaggle-backpack-price-prediction
