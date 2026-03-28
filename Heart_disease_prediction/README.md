#  Heart Disease Prediction: Smart Model Selection

Can we predict heart disease before it strikes? This project implements a machine learning solution to analyze cardiovascular data and uses an automated benchmarking approach to find the most accurate prediction model.

##  Why This Project is Unique
Instead of just training one model, I developed a custom **ModelSelection function** that automates:
- **Benchmarking:** Running multiple algorithms (Logistic Regression, SVC, KNN, Random Forest) side-by-side.
- **Hyperparameter Tuning:** Integrating `GridSearchCV` to find the "Best Parameters" for each model automatically.
- **Data-Driven Decisions:** The system identifies and selects the **Best Model** based on the highest cross-validation score.

##  Technical Toolkit
- **Algorithms:** Logistic Regression, Support Vector Machine (SVM), K-Nearest Neighbors (KNN), Random Forest Classifier.
- **Optimization:** GridSearchCV, RandomizedSearchCV, and Cross-Validation.
- **Visualization:** Seaborn and Matplotlib for Exploratory Data Analysis (EDA).
- **Libraries:** Scikit-Learn, Pandas, Numpy.

##  Feature Analysis
The model analyzes critical health indicators:
- **Age & Gender**
- **Chest Pain Type (cp)**
- **Resting Blood Pressure (trestbps)**
- **Cholesterol Levels (chol)**
- **Maximum Heart Rate (thalach)**

##  Key Achievements
- **Automation:** Reduced manual effort by building a reusable model evaluation framework.
- **Accuracy:** Fine-tuned the models to achieve optimal performance for medical binary classification.