# 🚦 Traffic Demand Forecasting System

A Machine Learning project to predict traffic demand using temporal, geographical, road network, and weather-related features. The solution was developed for a traffic demand prediction competition using Python, CatBoost, and Scikit-Learn.

---

## 📌 Overview

Urban traffic congestion is a growing challenge that affects transportation efficiency and economic productivity. This project builds a machine learning pipeline to forecast traffic demand by leveraging historical traffic data and feature engineering techniques.

The solution was trained using **77,299** records and generated predictions for **41,778** unseen samples.

---

## 🎯 Problem Statement

Develop a machine learning model capable of predicting traffic demand using:

- Geographic location (Geohash)
- Road characteristics
- Weather conditions
- Temperature
- Timestamp
- Number of lanes
- Large vehicle information
- Nearby landmarks

Evaluation Metric:

**Score = max(0, 100 × R² Score)**

---

## 📊 Dataset

### Training Dataset

- 77,299 rows
- 11 Features

### Test Dataset

- 41,778 rows
- 10 Features

### Features Used

- Geohash
- Day
- Timestamp
- RoadType
- NumberOfLanes
- LargeVehicles
- Landmarks
- Temperature
- Weather

Target Variable:

- Demand

---

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- CatBoost
- Scikit-Learn
- Matplotlib
- PyGeoHash
- Jupyter Notebook

---

## ⚙️ Feature Engineering

The project includes several feature engineering techniques:

- Hour extraction
- Minute extraction
- Peak hour detection
- Time slot creation
- Geohash decomposition
- Latitude & Longitude extraction
- Frequency encoding
- Interaction features
- Missing value handling

---

## 🤖 Model

The final solution uses:

**CatBoostRegressor**

Key Parameters:

- Iterations: 2000
- Depth: 8
- Learning Rate: 0.05

---

## 📈 Results

### Validation Performance

- Validation **R² ≈ 0.957**

### Competition Submission

- Final Competition Score: **91.12190**

The model achieved strong predictive performance through feature engineering and CatBoost optimization.

---

## 📁 Repository Structure

```
traffic-demand-forecasting/
│
├── traffic_demand_forecasting.ipynb
├── requirements.txt
├── submission_v2.csv
└── README.md
```

---

## 🚀 How to Run

1. Clone the repository

```bash
git clone https://github.com/bhanukiran29/traffic-demand-forecasting.git
```

2. Install dependencies

```bash
pip install -r requirements.txt
```

3. Open

```
traffic_demand_forecasting.ipynb
```

4. Execute all notebook cells.

---

## 📌 Future Improvements

- Hyperparameter tuning using Optuna
- Ensemble learning
- LightGBM/XGBoost comparison
- Automated feature selection
- Model deployment using FastAPI

---

## 👨‍💻 Author

**Madisetty Bhanu Kiran**

- LinkedIn: https://linkedin.com/in/madisetty-bhanu-kiran
- GitHub: https://github.com/bhanukiran29
