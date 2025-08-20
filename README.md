# F1 Engine Stress Index (ESI) Analysis

This repository provides tools to analyze Formula 1 telemetry data using [FastF1](https://theoehrly.github.io/Fast-F1/).  
It introduces a custom **Engine Stress Index (ESI)**, which combines RPM, throttle, and positive acceleration signals into a single metric.  
The code produces lap visualisations, track maps colored by ESI, and tables summarizing the most demanding corners and straights.

---

## ✨ Features
- **ESI computation per lap**  
  Robust scaling of RPM, throttle, and acceleration with configurable weights.  
- **Corner & straight aggregation**  
  Identify top stress corners and straights using telemetry and circuit map data.  
- **Visualization**  
  - ESI vs. distance with corner markers  
  - Track map heatmap (colored by ESI) with corner labels  
  - Top-5 tables for stressful corners/straights  

---

## 📦 Requirements
- Python 3.10+
- Dependencies:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `fastf1`

Install via:
```bash
pip install fastf1 matplotlib pandas numpy
```
