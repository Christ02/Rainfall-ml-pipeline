# AustralianWeather

A scikit-learn machine learning pipeline contained within a Jupyter Notebook (`AustralianWeather.ipynb`) that predicts whether it will rain today in the Melbourne area using historical weather data and rigorous model evaluation.

## Overview

This project focuses on building and tuning a reproducible ML workflow—all within a single notebook—to answer the question: **Will it rain today?** You’ll find:

1. **Data Loading & Selection**: Import historical weather records for Melbourne, Watsonia, and Melbourne Airport stations.
2. **Exploratory Data Analysis**: Check class balance, visualize rain frequency, and identify potential data leakage.
3. **Feature Engineering**:

   * Derive a `Season` column from dates to capture seasonality.
   * Group nearby stations and retain `Location` as a categorical feature.
   * Optionally create lagged features or aggregate statistics.
4. **Preprocessing Pipeline**:

   * Automatic numeric/categorical handling with `ColumnTransformer`.
   * One-hot encoding for categories and scaling or imputation for numerics.
5. **Model Training & Tuning**:

   * Integrate preprocessing and model in a single `Pipeline`.
   * Compare **Random Forest** and **Logistic Regression** using `GridSearchCV` for hyperparameter optimization.
6. **Evaluation**:

   * Metrics: accuracy, recall (true positive rate), F1 score, ROC–AUC.
   * Confusion matrix to assess false positives/negatives.
   * Feature importances to understand key predictors.

## Getting Started

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/rainfall-ml-pipeline.git
   cd rainfall-ml-pipeline
   ```

2. **Launch the notebook**:

   ```bash
   jupyter lab AustralianWeather.ipynb
   ```

3. **Run all cells** and explore the step-by-step workflow. You can tweak parameters, add features, or switch models as you like.

## File Structure

```
rainfall-ml-pipeline/
├── AustralianWeather.ipynb   # Main notebook with full pipeline
└── README.md                 
```

## License

MIT © 2025 Christian Alejandro Barrios Rodriguez
