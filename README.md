# Demand Forecasting — TransVolt Assignment

## Overview

An end-to-end demand forecasting pipeline for predicting **8-week ahead demand** across SKU–Supermarket combinations. The project includes exploratory data analysis, feature engineering, multiple machine learning models, and business recommendations to support inventory planning and reduce stock-outs and excess inventory.

## Files

- `Forecasting_demand.ipynb` — Complete analysis, EDA, feature engineering, model development, and evaluation
- `demand_forecast.pptx` — Executive summary presentation
- `demand.csv` — Historical demand dataset
- `promotions.csv` — Promotion events dataset

## Models Evaluated

| Model | MAE | RMSE | R² |
|------|----:|-----:|----:|
| **Random Forest** | **3.1054** | **15.3934** | **0.5935** |
| XGBoost | 3.5720 | 15.5423 | 0.5856 |
| LightGBM | 3.4919 | 15.4763 | 0.5891 |
| Ensemble | 3.2768 | 15.4203 | 0.5921 |

**Best Model:** Random Forest

## Key Insights

- Historical demand (lag features) was the strongest predictor of future demand.
- Demand varied primarily by SKU and supermarket.
- Weekly and monthly seasonality had limited influence.
- Promotion data was sparse, resulting in limited measurable impact.
- Tree-based ensemble models consistently produced the best forecasting performance.

## Business Impact

The proposed forecasting pipeline enables rolling **8-week demand forecasts**, helping improve production planning, reduce stock-outs, minimize inventory write-offs, and support data-driven supply chain decisions.
