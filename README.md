# 🎬 IMDb India Movie Rating Prediction

A machine learning project to predict IMDb movie ratings based on Genre, Director, and Lead Actor using Random Forest Regression.

# 📌 Project Overview

This project demonstrates a complete workflow for predicting movie ratings using machine learning.
It includes:

Data loading and preprocessing

Handling missing values

Encoding categorical features

Model training using Random Forest

Model evaluation (RMSE & R² Score)

Rating distribution visualization

The goal is to understand how movie metadata influences its IMDb rating.

# 📂 Dataset

The project uses the file:

IMDb Movies India.csv


Make sure the file is placed in the same directory as the notebook/script.

Dataset Columns Used

Genre

Director

Actor 1

Rating (target variable)

Missing values are handled carefully to ensure data quality.

# 🧪 Model Used
Random Forest Regressor

Handles non-linear relationships

Works well with categorical features after one-hot encoding

Resistant to overfitting with proper tree count

# 🧹 Data Preprocessing Steps

Remove rows where Rating is missing

Fill missing values in categorical columns

Select useful columns

Convert categorical data to numeric using OneHotEncoder

Split into training/testing sets

# 🧠 Training & Testing

The dataset is split into:

80% training

20% testing

The model is trained using:

model = RandomForestRegressor(n_estimators=100, random_state=42)

# 📊 Evaluation Metrics

Two metrics are used:

Metric	Meaning
RMSE	Measures prediction error
R² Score	Measures model accuracy

Example output:

Movie Rating Prediction Model Results
Root Mean Squared Error (RMSE): 0.45
R² Score: 0.72

# 📈 Visualizations

A histogram of the movie rating distribution is generated:

sns.histplot(df["Rating"], bins=20)


This helps understand how ratings are spread across movies.

# 📦 Requirements

Install dependencies using:

pip install pandas numpy matplotlib seaborn scikit-learn

# ▶️ How to Run

Clone this repository:

git clone https://github.com/your-username/imdb-rating-prediction.git


Navigate into project folder:

cd imdb-rating-prediction


Run the script:

python imdb_model.py

# 🛠 Technologies Used

Python

Pandas

NumPy

Seaborn

Matplotlib

Scikit-Learn

# 🚀 Future Improvements

Include more features (budget, votes, runtime, etc.)

Try models like XGBoost, LightGBM

Hyperparameter tuning

Deploy using Flask/Streamlit
