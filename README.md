# F1 Data Science Analyses with FastF1

This repository contains multiple Jupyter notebooks applying **data science and machine learning** techniques to Formula 1 data via [FastF1](https://theoehrly.github.io/Fast-F1/).

Each notebook demonstrates a different analysis approach:
- 📊 **Performance Metrics (Engine Stress Index)**  
- 🤖 **Machine Learning Lap Time Prediction**

---

## 📂 Notebooks

### 1. Engine Stress Index (ESI) Analysis
- Introduces a custom **Engine Stress Index (ESI)** combining RPM, throttle, and positive acceleration.  
- Produces lap visualisations, track maps colored by ESI, and top-5 demanding corners/straights.  
- **Goal:** quantify where the power unit is most stressed around a circuit.

### 2. Lap Time Prediction with ML
- Uses **tyre compound, tyre life, stint progression, and driver info** to predict lap times.  
- Trains a **Gradient Boosting Regressor** with leakage-aware `GroupKFold` validation by driver.  
- Achieves ~**1.0s MAE** and ~**0.90 R²** on race data (e.g., 2024 British GP).  
- Provides **feature importance analysis** (tyre compound dominates), and plots of **actual vs predicted lap times**.  
- **Goal:** showcase machine learning applied to race strategy/tyre modelling.

---

## 🚧 Project Status
This project is currently **a work in progress**.  
Expect frequent changes and incomplete features while development is ongoing.

---

## ✨ Features
- **ESI notebook**: stress index computation, corner/straight aggregation, visualisations.  
- **Lap Time notebook**: regression modelling, permutation importance, tyre degradation curves.  

---

## 📦 Requirements
- Python 3.10+
- Dependencies:
  - `numpy`, `pandas`, `matplotlib`
  - `fastf1`
  - `scikit-learn`

Install via:
```bash
pip install fastf1 matplotlib pandas numpy scikit-learn
