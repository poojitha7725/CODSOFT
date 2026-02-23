# Titanic Survival Prediction Project

## Overview
This project focuses on building a machine learning model to predict the survival status of passengers on the Titanic using various features from the dataset.

## Dataset
- **Name:** Titanic Passenger Data
- **Target:** Survival (0 = Did Not Survive, 1 = Survived)
- **Features Used:** 7 features after preprocessing (Age, Sex, Pclass, Fare, Embarked, etc.)

## Project Workflow
1. **Data Exploration & Cleaning:**
   - Handled missing values in 'Age' (filled with median) and 'Embarked' (filled with mode).
   - Removed irrelevant columns: 'Cabin', 'PassengerId', 'Name', 'Ticket'.
   - Mapped categorical variables ('Sex', 'Embarked') to numerical values.
2. **Exploratory Data Analysis (EDA):**
   - Visualized distributions of Age and Fare.
   - Analyzed survival rates by Passenger Class (Pclass) and Gender (Sex) through count plots.
3. **Model Training:**
   - Split data into training (80%) and testing (20%) sets.
   - Trained a Random Forest Classifier.
4. **Evaluation:**
   - Achieved a Test Accuracy of approximately **61.45%**.
   - F1 Score: **0.5036**.
   - Cross-Validation Mean: **70.15% (+/- 2.52%)**.
   - Analyzed Feature Importance, with **Fare** identified as the top predictive feature.
5. **Deployment:**
   - Saved the trained Random Forest model as `random_forest_model.pkl`.
   - Generated a `model_summary.json` for production integration.

## Key Insights
- **Fare** was found to be the most significant feature for predicting survival.
- The model shows strong consistency across cross-validation folds.

## Deliverables
- `Task-1(titanic).ipynb`: Comprehensive Jupyter Notebook documenting the analysis.
- `titanic_models/random_forest_model.pkl`: Serialized production-ready model.
- `titanic_models/model_summary.json`: JSON metadata and metrics for the model.

## Implementation Details
To load the model in production:
```python
import joblib
loaded_model = joblib.load('titanic_models/random_forest_model.pkl')
```

## Project Status
**Status:** ✅ COMPLETE & READY FOR DEPLOYMENT
