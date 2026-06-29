# Mining--quality-prediction
ML model to predict % silica concentrate in mining flotation process using Random forest((R²=0.9999)

## Overview
ML project to predict % Silica Concentrate (impurity) in iron ore from a real industrial flotation plant dataset using Random Forest and Linear Regression.

## Problem Statement
Predicting silica impurity in iron ore concentrate helps mining engineers take early corrective actions, improving efficiency and reducing environmental waste.

## Dataset
** Source: UCT internship dataset (Mining Process Flotation Plant)
** 50,000 rows × 24 columns
 ** Features: Iron Feed, Silica Feed, Starch Flow, Amina Flow, Ore Pulp Flow, Flotation Column Air Flows and Levels
 ** Target: % Silica Concentrate (last column)

## Approach
1. Loaded 50,000 rows from large industrial dataset
2. Dropped date column, handled missing values
3. Trained Linear Regression and Random Forest Regressor
4. Evaluated using RMSE and R² Score
5. Generated 4 visualizations (Actual vs Predicted, Feature Importance, Correlation Heatmap, Target Distribution)

## Results
| Model | RMSE | R² Score |
|-------|------|----------|
| Linear Regression | 0.5313 | 0.7974 |
| Random Forest | 0.0141 | 0.9999 |

Random Forest achieved near-perfect prediction accuracy (R² = 0.9999).

## Tech Stack
* Python
* Pandas
* Scikit-learn
* Matplotlib
* Seaborn

## Learnings
- Real industrial datasets require careful handling of decimal formats
- Random Forest drastically outperforms Linear Regression on complex process data
- Feature importance analysis reveals which flotation parameters most influence silica concentration
