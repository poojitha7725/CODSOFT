# 🎬 Movie Rating Prediction

## 📌 Project Overview
This project focuses on building a machine learning model to predict movie ratings based on various factors such as **Genre**, **Director**, and **Lead Actors**. The analysis is performed using a structured modular workflow in Python.

### 👤 Developer Info
- **Developer:** POOJITHA
- **Domain:** Data Science
- **Objective:** Predict IMDb ratings using regression techniques.

---

## 🚀 Features
- **Data Cleaning:** Robust handling of missing values for both numerical (Year, Duration, Votes) and categorical features.
- **Exploratory Data Analysis (EDA):** Visual insights into top genres, prolific directors, and year-wise trends using Matplotlib, Seaborn, and Plotly.
- **Feature Engineering:** Automated label encoding for categorical variables.
- **Model Comparison:** Evaluates multiple regression models:
  - Linear Regression
  - Random Forest Regressor
  - Gradient Boosting Regressor

---

## 🛠️ Tech Stack
- **Language:** Python 3.x
- **Libraries:**
  - `pandas`, `numpy`: Data manipulation
  - `matplotlib`, `seaborn`, `plotly`: Data visualization
  - `scikit-learn`: Machine learning & preprocessing

---

## 📊 Dataset
The model uses `imdb_data (1).csv` which contains information about:
- Movie Name
- Release Year
- Duration
- Genre
- Rating (Target Variable)
- Votes
- Director & Lead Actors (Actor 1, 2, 3)

---

## 📈 Model Performance
The current pipeline evaluates models based on **R² Score** and **Mean Squared Error (MSE)**.

| Model | Status |
| :--- | :--- |
| **Linear Regression** | Baseline |
| **Random Forest** | Performance-Optimized |
| **Gradient Boosting** | High Precision |

---

## ⚙️ How to Run
1. Ensure you have the required libraries installed:
   ```bash
   pip install pandas numpy matplotlib seaborn plotly scikit-learn
   ```
2. Open `Task-2(Movies).ipynb` in Jupyter Notebook or VS Code.
3. Ensure the dataset `imdb_data (1).csv` is in the same directory.
4. Run all cells to execute the pipeline.
