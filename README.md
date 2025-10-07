
---

# Real-Estate-Price-Prediction-with-Ensemble-Features 🏡💰

[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-1.3.0-orange)](https://scikit-learn.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-1.7.6-green)](https://xgboost.readthedocs.io/)
[![LightGBM](https://img.shields.io/badge/LightGBM-4.2.0-blueviolet)](https://lightgbm.readthedocs.io/)

Optimized **ensemble approach for real estate price prediction** using machine learning. This project includes **data preprocessing, feature selection, model training, hyperparameter tuning**, and **evaluation** using multiple regression models and ensemble techniques.

---

## Project Overview

This project predicts **house sale prices** using the **Ames Housing dataset**. The dataset contains **2930 records** with **81 features** describing residential properties, including lot size, neighborhood, construction quality, year built, basement details, and garage specifications.

**Goal:** Build an optimized machine learning model to accurately predict house prices.

---

## Dataset Preprocessing

* **Handling missing values:** Remove features with extensive nulls.
* **Encoding:** Categorical variables using **Label Encoding**.
* **Scaling:** Numeric features using **MinMaxScaler**.

---

## Feature Selection

* **Forward feature selection** based on **p-values** to retain only statistically significant features.
* Reduces dimensionality while keeping the strongest predictors of house prices.

---

## Modeling Approach

Models used:

| Model             | Description                                                     |
| ----------------- | --------------------------------------------------------------- |
| XGBoost           | Gradient boosting for high performance regression               |
| LightGBM          | Efficient gradient boosting with low memory usage               |
| CatBoost          | Gradient boosting that handles categorical features efficiently |
| SVR               | Support Vector Regression for non-linear prediction             |
| Stacking Ensemble | Combines XGBoost and LightGBM for robust predictions            |

* **Hyperparameter tuning:** `RandomizedSearchCV`
* **Pipelines:** Streamlined scaling, encoding, and modeling processes

---

## Evaluation Metrics

| Metric        | Description                                     |
| ------------- | ----------------------------------------------- |
| R²            | Percentage of variance explained by the model   |
| MAE           | Average absolute prediction error               |
| RMSE          | Root mean squared error, penalizes large errors |
| Training Time | Time taken to train each model                  |

---

## Results & Insights

* Comparison of individual and ensemble models identifies the **best-performing model**.
* Visualizations include:

  * **Predicted vs Actual Prices**
  * **Residual Errors**

**Sample Visualization:**
*(Add your plots here using GitHub markdown, e.g., `![Predicted vs Actual](path_to_plot.png)`)*

---

## Installation & Usage

```bash
git clone https://github.com/your-username/Real-Estate-Price-Prediction-with-Ensemble-Features.git
cd Real-Estate-Price-Prediction-with-Ensemble-Features
pip install -r requirements.txt
python main.py
```

---

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve models, visualizations, or documentation.

---

