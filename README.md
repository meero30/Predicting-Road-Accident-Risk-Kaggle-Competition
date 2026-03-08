# 2025 Predicting Road Risk - Kaggle Competition

This repository contains the solution for the 2025 Kaggle "Predicting Road Risk" competition. The goal is to predict the `accident_risk` score for various road segments based on environmental, structural, and historical data.

## Project Overview
The pipeline involves extensive Exploratory Data Analysis (EDA) and the implementation of automated machine learning (AutoML) to generate high-accuracy risk predictions.

## Key Features
- **Data Source:** Kaggle 2025 Predicting Road Risk Dataset (~517k training samples).
- **Target Variable:** `accident_risk` (Continuous score).
- **Features:** Road type, curvature, speed limits, lighting, weather conditions, and historical accident counts.

## Methodology
1. **EDA:** Analyzed distributions of categorical variables (weather, lighting, road type) and correlations between physical road attributes and risk.
2. **Automated ML:** Leveraged the `mljar-supervised` AutoML framework to benchmark multiple algorithms including LightGBM and Linear Regression.
3. **Ensembling:** Utilized an ensemble of models to optimize the final risk score.
4. **Post-Processing:** Applied prediction clipping to ensure results remained within the valid 0.0 to 1.0 range.

## Libraries Used
- `pandas`, `numpy` (Data manipulation)
- `matplotlib`, `seaborn` (Visualization)
- `scikit-learn` (Preprocessing and Pipelines)
- `mljar-supervised` (AutoML)
