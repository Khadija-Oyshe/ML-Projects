# Calorie Burn Prediction using XGBoost

This project predicts the number of calories burned during physical activity based on various personal and exercise-related factors. It utilizes machine learning to provide an estimate that can help users track their fitness goals more accurately.

## Key Highlights
- **Model Used:** XGBoost Regressor.
- **Objective:** To estimate calories burned based on exercise duration, heart rate, and body metrics.
- **Prediction result:** Successfully predicts calories for custom user input (e.g., predicted ~47.45 kcal for a 10-year-old male with 20 mins duration).

## Features Used
The model considers the following features for prediction:
- **Gender:** (Male/Female)
- **Age:** User's age
- **Height & Weight:** Used to determine body metrics
- **Duration:** Time spent exercising (in minutes)
- **Heart Rate:** Average heart rate during the activity
- **Body Temperature:** Internal body temperature during exercise

## Tech Stack
- **Language:** Python
- **Machine Learning Library:** XGBoost
- **Data Manipulation:** Pandas, Numpy
- **Visualization:** Matplotlib, Seaborn (used during EDA)

## Workflow
1. **Data Preprocessing:** Handling categorical data (Gender) using encoding.
2. **Model Training:** Training the XGBoost Regressor on the training dataset.
3. **Evaluation:** Checking the model's performance on test data.
4. **Custom Prediction:** A dedicated script/cell to input personal data and get an instant calorie burn estimate.
