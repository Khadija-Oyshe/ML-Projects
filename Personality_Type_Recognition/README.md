# Personality Type Prediction (Introvert vs. Extrovert)

This project aims to predict an individual's personality type based on various behavioral and demographic features using Machine Learning. It demonstrates a complete end-to-end ML workflow, from raw data preprocessing to model serialization.

## Highlights
- **End-to-End Pipeline:** Implemented `ColumnTransformer` and `Pipeline` to automate imputation, scaling, and encoding, ensuring zero data leakage.
- **Model Benchmarking:** Compared multiple classifiers including Logistic Regression, SVM, KNN, and Random Forest using `GridSearchCV` for hyperparameter tuning.
- **Production Ready:** Exported the final model and preprocessor using `joblib` for seamless deployment in production environments.

## Technical Stack
- **Algorithms:** Random Forest (Best Model), SVM, Logistic Regression, KNN.
- **Preprocessing:** `OneHotEncoder`, `OrdinalEncoder`, `SimpleImputer`, `StandardScaler`.
- **Libraries:** Scikit-Learn, Pandas, Numpy, Joblib.

## Feature Engineering
The model handles a mix of numerical and categorical data:
- **Categorical:** Gender, Occupation, Education Level, etc. (Handled via OneHot/Ordinal Encoding).
- **Numerical:** Age and other behavioral scores (Handled via Scaling).

## Results
- **Optimization:** Used `GridSearchCV` to find the optimal parameters for the Random Forest Classifier.
- **Outcome:** The model successfully classifies users into "Introvert" or "Extrovert" with high reliability.

## Project Structure
- `Personality_Type_.ipynb`: Full data analysis and model training.
- `personality_model.joblib`: The trained model.
- `preprocessor.joblib`: Saved preprocessing pipeline.