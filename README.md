# 📈 Sales Forecasting ML Project

This repository contains an end-to-end **retail sales forecasting pipeline** built using **XGBoost** and **Facebook Prophet**, along with a **hybrid ensemble model**.
The objective is to predict future daily sales based on historical data, seasonal trends, and domain-specific indicators.

---

## 📂 Repository Structure

```
├── Sales_Forecasting.ipynb   # Complete notebook with EDA → modeling → evaluation
├── final_forecasts.csv        # Final model predictions (XGB, Prophet, Hybrid)
├── README.md                  # Project documentation
```

---

## 🔧 Tech Stack

* **Python**
* **Pandas, NumPy**
* **XGBoost**
* **Facebook Prophet**
* **Scikit-learn**
* **Matplotlib / Seaborn**
* **Power BI** (for dashboard visualization)

---

## 🔍 Problem Statement

Retail businesses require accurate sales predictions to make informed decisions regarding:

* Inventory stocking
* Demand planning
* Marketing optimization
* Revenue forecasting

This project builds ML models to forecast daily sales and compare performance across algorithms.

---

## 🧹 Data Preprocessing & Feature Engineering

### ✔️ Steps Implemented

* Handled missing values
* Converted timestamps to proper datetime format
* Merged monthly-level data to daily granularity
* Added seasonal indicators (Winter, Summer, Monsoon, Retreating Monsoon)
* Added holiday spikes & special events
* Generated lag features (lag-1, lag-7, lag-30)
* Created moving averages (7/14/30-day windows)

---

## 📊 Exploratory Data Analysis (EDA)

Key insights:

* Identified clear **weekly** and **seasonal** patterns
* Detected sales dips during off-season periods
* Observed holiday spikes
* Visualized trends, autocorrelation, rolling windows

---

## 🤖 Models Used

### 1️⃣ **XGBoost Regressor**

* Handles complex non-linear patterns
* Engineered features boost performance
* Provides highly granular predictions

### 2️⃣ **Facebook Prophet**

* Excellent for strong seasonality
* Captures weekly, yearly trends
* Automatically models changepoints

### 3️⃣ **Hybrid Model (XGB + Prophet)**

* Weighted blend of both models
* Achieves smoother and more stable forecasts
---

## 📁 Output

### **`final_forecasts.csv` contains:**

* Date
* Actual sales (if available)
* XGBoost predictions
* Prophet predictions
* Hybrid predictions
---
## ▶️ How to Run

1. Clone the repo

   ```
   git clone https://github.com/ananyascodehq/sales-forecasting-ml.git
   ```
2. Install dependencies

   ```
   pip install -r requirements.txt
   ```
3. Run the notebook

   ```
   Sales_Forecasting.ipynb
   ```
4. Export predictions → Load `final_forecasts.csv` into Power BI.

---

## 📝 Author

**Ananya**
AI/ML Intern
GitHub: [*profile link*](https://github.com/ananyascodehq)

