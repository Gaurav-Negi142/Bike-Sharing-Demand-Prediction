# Bike-Sharing-Demand-Prediction
# 🚲 ML Regression Capstone Project – Bike Sharing Demand Prediction

## 📖 Project Overview
This project aims to **predict bike sharing demand** using a dataset containing hourly rental information along with environmental and temporal features. Accurate demand forecasting is crucial for optimizing bike distribution, managing inventory, and improving service efficiency in bike sharing systems.

---

## 🗂 Dataset
- **Rows:** 8,760 (hourly records for one year)
- **Columns:** 14 features including:
  - Date, Hour, Rented Bike Count (target)
  - Weather metrics: Temperature, Humidity, Wind Speed, Visibility, Dew Point, Solar Radiation, Rainfall, Snowfall
  - Categorical features: Seasons, Holiday, Functioning Day

The dataset contained **no missing values or duplicates**, simplifying preprocessing.

---

## 🔧 Methodology
1. **Data Exploration & Cleaning**
   - Converted `Date` to datetime
   - Extracted temporal features (Year, Month, Day, Weekday)
   - Converted categorical variables to `category` type

2. **Data Visualization**
   - Histograms, scatter plots, box plots, and correlation heatmaps
   - Insights: rentals peak during rush hours, higher in warmer temperatures, vary by season and holidays

3. **Hypothesis Testing**
   - T-tests confirmed significant differences in rentals based on temperature, holidays, and functioning days

4. **Feature Engineering**
   - Outlier capping (IQR method)
   - Log transformations for skewed features
   - Label Encoding & One-Hot Encoding
   - Cyclical features for Hour/Month
   - Interaction features (e.g., Temp × Solar Radiation)

5. **Model Implementation**
   - Linear Regression
   - Random Forest Regressor
   - Gradient Boosting Regressor
   - Hyperparameter tuning with `RandomizedSearchCV`

---

## 📊 Results
- **Best Model:** Tuned Gradient Boosting Regressor
- **Performance Metrics:** Achieved highest accuracy and lowest error on test data
- **Key Insights:** Temperature, hour of day, and season strongly influence demand

---

## 🏆 Learning Outcomes
- End-to-end ML workflow: data wrangling → visualization → hypothesis testing → feature engineering → model building
- Practical application of regression techniques for demand forecasting
- Improved understanding of feature importance and model interpretability

---

## 📜 License
This project is licensed under the MIT License – feel free to use and adapt for learning purposes.
