# 🌾 Crop Yield Prediction using Machine Learning

> Predicting global crop yields based on environmental and agricultural inputs using supervised learning.

## 🎯 Objective

To build a predictive model that estimates crop yields using features such as rainfall, temperature, pesticide use, crop type, and geographic region. The aim is to support data-driven agricultural planning and highlight the most impactful factors influencing crop productivity worldwide.

---

## 📂 Project Structure

```

├── data/
│   └── yield\_df.csv                 # Raw dataset
├── notebooks/
│   └── crop\_yields\_analysis.ipynb  # Data analysis and model notebook
├── README.md                       # Project overview


---

## 📄 Dataset Overview

- Source: [Kaggle – Crop Yield Prediction](https://www.kaggle.com/code/mohsin31202/crop-yield-prediction)
- **Records**: 28,000+
- **Features**:
  - `Area`: Country or region name
  - `area_codes`: Numerical encoding of `Area`
  - `Item`: Crop type (e.g. Maize, Wheat, Rice)
  - `item_codes`: Numerical encoding of `Item`
  - `Year`: Year of data collection
  - `hg/ha_yield`: Crop yield (target variable, in hectograms per hectare)
  - `average_rain_fall_mm_per_year`: Annual average rainfall in millimeters
  - `pesticides_tonnes`: Annual pesticide usage in tonnes
  - `avg_temp`: Annual average temperature (°C)

---

## 🧰 Tools & Technologies

- Python · Pandas · NumPy · Matplotlib · Seaborn  
- Scikit-learn · Jupyter Notebook · StandardScaler · Random Forest

---

## 📊 Exploratory Data Analysis (EDA)

- Univariate and bivariate visualizations
- Correlation heatmaps and outlier detection
- Time series trends of rainfall, temperature, and pesticide use
- Yield comparison across crops and countries

---

## 🤖 Modeling

- **Baseline model**: Linear Regression  
  - *Result*: R² ~ 0.03 (poor performance due to low linear correlation)

- **Improved model**: Random Forest Regressor  
  - Evaluated using:
    - R² Score
    - Mean Squared Error (MSE)
    - Root Mean Squared Error (RMSE)
    - Mean Absolute Error (MAE)
  - Feature importance analysis to interpret influence of each variable

---

## ✅ Key Contributions

- Cleaned and encoded the dataset for machine learning.
- Built and evaluated regression models to predict crop yield.
- Identified most important yield-driving features (e.g., temperature and pesticide use).
- Proposed future model improvements using XGBoost, SVR, and neural networks.

---

## 📌 Future Improvements

- Hyperparameter tuning using GridSearchCV
- Explore more robust models (XGBoost, LightGBM)
- Add weather time-series data for temporal modeling
- Deploy as a simple web app or API

---

## 📎 License

This project is open source and available under the [MIT License](LICENSE).

---

## 🤝 Acknowledgements

- Data sourced from FAO via Kaggle.
- Inspired by sustainable agriculture and food security applications.

