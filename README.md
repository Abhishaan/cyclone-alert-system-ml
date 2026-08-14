# Cyclone Alert System for Weather Forecasting using Machine Learning

## 📌 Project Overview

The **Cyclone Alert System** is a machine learning-based system developed to analyze tropical cyclone data and classify cyclone intensity levels. The project aims to support early warning and disaster preparedness by using historical cyclone observations and machine learning techniques.

The system uses **IBTrACS (International Best Track Archive for Climate Stewardship)** data containing parameters such as wind speed, atmospheric pressure, latitude, longitude, storm movement, and temporal information.

## 🎯 Objectives

* Analyze historical tropical cyclone data using machine learning.
* Classify cyclones according to their intensity levels.
* Identify important factors influencing cyclone intensity.
* Generate graduated threat alerts for tropical storms, hurricanes, and major hurricanes.
* Compare multiple machine learning algorithms.
* Provide visual and geospatial analysis of cyclone activity.

## 📊 Dataset

The project uses the **IBTrACS v04r01** dataset covering cyclone observations from **2022–2025**.

The processed dataset contains approximately **22,891 observations** and 32 initial features, covering 409 distinct storms across multiple basins.

Important parameters include:

* Wind Speed
* Atmospheric Pressure
* Latitude
* Longitude
* Storm Speed
* Storm Direction
* Date and Time
* Storm Movement
* Cyclone Structure

## ⚙️ Feature Engineering

The project performs extensive feature engineering, including:

* Temporal features such as year, month, day and hour
* Day of year and week of year
* Cyclone category
* Wind and pressure changes
* Latitude and longitude movement
* Storm duration
* Rolling wind and pressure averages
* Hemisphere and seasonal features

The feature space was expanded from **32 to 54 predictive features**.

## 🤖 Machine Learning Algorithms

Four supervised machine learning algorithms were evaluated:

1. **Random Forest**
2. **XGBoost**
3. **LightGBM**
4. **CatBoost**

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* AUC-ROC

### 🏆 Best Performing Model

**XGBoost** achieved the best overall performance:

* Accuracy: **94.2%**
* AUC-ROC: **0.97**
* F1-Score: **0.925**

For major hurricane detection, the system achieved **96.8% accuracy**.

## 🚨 Alert Classification

The system defines three important threat levels:

* **Tropical Storm:** Wind speed ≥ 34 knots
* **Hurricane:** Wind speed ≥ 64 knots
* **Major Hurricane:** Wind speed ≥ 96 knots

These classifications can support graduated cyclone alert generation.

## 🔍 Important Predictors

The feature importance analysis identified the following major predictors:

1. Pressure
2. Pressure Change
3. Wind Change
4. Latitude
5. Hours Since Storm Start

The study also found a strong negative correlation between wind speed and central pressure (**r = -0.89**).

## 🗺️ Visualization

The project includes data visualization and interactive geospatial analysis for examining:

* Cyclone tracks
* Wind-speed distributions
* Pressure and wind relationships
* Feature correlations
* Cyclone intensity patterns

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Scikit-learn**
* **XGBoost**
* **LightGBM**
* **CatBoost**
* **Matplotlib**
* **Seaborn**
* **Plotly**
* **Folium**
* **Google Colab**
* **Jupyter Notebook**

## 📁 Project Files

```text
cyclone-alert-system-ml/
│
├── Cyclone_Alert_System.ipynb
└── README.md
```

## ▶️ How to Run

1. Open `Cyclone_Alert_System.ipynb`.
2. Open the notebook in Google Colab.
3. Upload/provide the required IBTrACS dataset.
4. Run the notebook cells sequentially.
5. Perform data preprocessing and feature engineering.
6. Train and evaluate the machine learning models.
7. Compare model performance and visualize cyclone patterns.

## 📄 Research Publication

This project has been published as:

**Cyclone Alert System for Weather Forecasting using Machine Learning**

**Journal:** Journal of Emerging Technologies and Innovative Research (JETIR)

**Volume:** 13, Issue 4

**Publication Date:** April 18, 2026

**Paper ID:** JETIR2604564

**Authors:** Abhijeet Panigrahi, Anjali Patnaik, Sanghamitra Samantara, B. Ujalesh Subudhi

**Publication:** http://www.jetir.org/view?paper=JETIR2604564

## 🔮 Future Work

Future improvements include:

* Integration of satellite-derived environmental data.
* 6, 12, 24 and 48-hour intensity forecasting.
* Ensemble machine learning methods.
* CNN-based satellite image analysis.
* LSTM-based cyclone trajectory prediction.
* Real-time API-based cyclone alerts.
* Explainable AI using SHAP.

## 👨‍💻 Author

**Abhijeet Panigrahi**

B.Tech – Computer Science and Engineering
NIST University, Berhampur, Odisha
