# ✈️ Flight Price Prediction – EDA & Feature Engineering

This project focuses on **Exploratory Data Analysis (EDA)** and **feature engineering** on flight ticket data to prepare it for machine learning-based price prediction.

---

## 📊 Dataset

- **Source**: [Kaggle - Flight Price Prediction](https://www.kaggle.com/datasets/shubhambathwal/flight-price-prediction)
- **Rows**: 10,683
- **Target Variable**: `Price` (flight ticket cost)

### Main Features:
- `Airline`: Airline operating the flight
- `Source` / `Destination`: Cities of departure and arrival
- `Route`: Flight path with stops
- `Total_Stops`: Number of stops
- `Dep_Time` / `Arrival_Time`: Departure and arrival timestamps
- `Duration`: Total flight time
- `Additional_Info`: Extra details (e.g. meal, baggage)
- `Date_of_Journey`: Flight date

---

## 🔧 Feature Engineering Highlights

- Converted `Duration` into `Duration_in_minutes` (integer)
- Extracted day, month, and year from `Date_of_Journey`
- Parsed hours and minutes from `Dep_Time` and `Arrival_Time`
- Mapped `Total_Stops` to numerical values (0–4)
- Filled missing values using appropriate strategies
- Dropped redundant columns (`Route`, `Dep_Time`, `Arrival_Time`, etc.)
- Applied **One-Hot Encoding** on categorical columns:
  - `Airline`
  - `Source`
  - `Destination`

✅ Final dataset shape: **10,683 rows × 34 columns**  
✅ All features are **numerical**, suitable for modeling

---

## 📁 Output

A fully cleaned and feature-engineered dataset ready for building regression models to predict flight ticket prices.

---

## 🚀 Next Steps

- Train regression models (e.g., Linear Regression, Random Forest, XGBoost)
- Evaluate performance (RMSE, MAE, R²)
- Tune hyperparameters
- Optionally deploy the model for real-time predictions

---

## 📦 Requirements

pandas
numpy
matplotlib
seaborn
scikit-learn
