#  Rainfall Prediction: Advanced Weather Forecasting

Accurately predicting rainfall is a complex classification challenge. This project leverages Machine Learning to predict rain events by analyzing meteorological data, with a specific focus on handling imbalanced datasets and hyperparameter optimization.

##  Highlights
- **Class Imbalance Management:** Recognized and addressed skewed data distributions using **Resampling techniques** (`sklearn.utils.resample`) to ensure the model doesn't favor the majority class.
- **Robust Model Tuning:** Utilized **GridSearchCV** for systematic hyperparameter tuning, optimizing the `n_estimators`, `max_depth`, and `min_samples_split` of the Random Forest Classifier.
- **Comprehensive Evaluation:** Beyond simple accuracy, the model was evaluated using **Classification Reports (Precision, Recall, F1-Score)** and **Confusion Matrices** to ensure reliability in predicting rare rain events.

## Technical Stack
- **Algorithm:** Random Forest Classifier (Optimized via Grid Search).
- **Data Engineering:** Handling missing values, feature scaling, and class balancing.
- **Model Persistence:** Used `pickle` to serialize the trained model for future deployment.
- **Libraries:** Scikit-Learn, Pandas, Numpy, Seaborn.

## Workflow & Methodology
1. **Exploratory Data Analysis (EDA):** Visualized weather patterns and feature correlations using Seaborn.
2. **Balancing Act:** Upsampled/Downsampled data to create a 50/50 distribution for "Rain" vs "No Rain" classes.
3. **Cross-Validation:** Implemented `cross_val_score` to validate model stability across different data folds.
4. **Final Prediction:** Achieved a balanced F1-score of ~0.75, making it a reliable tool for binary weather classification.

## Performance Metrics
- **Accuracy:** 74%
- **Recall (Rain):** 0.78 (Crucial for predicting when it actually rains)
- **Precision (Rain):** 0.72