# HTX_Test – HDB Resale Price Prediction Model

This repository contains the data, code, and insights for a predictive model developed to analyze and estimate resale prices of HDB flats in Singapore. The goal is to uncover key drivers of housing prices and support data-driven strategies for housing affordability and policy evaluation.

---

## 🏠 Project Objective

Build a machine learning model that predicts the resale price of an HDB flat based on features such as:

- Town / location
- Flat type and floor area
- Lease remaining
- Distance to nearest MRT station
- Distance to CBD
- Temporal trend (month of transaction)
- Other engineered features

The model is designed to help planners and policymakers understand what factors most influence price — and explore potential strategies to curb price inflation.

---
## 📦 Repository Structure
-Datasets folder 
-Models and Codes folder
-Report Folder
---

## 📊 Data Sources

- HDB Resale Price data: [Data.gov.sg](https://data.gov.sg/dataset/resale-flat-prices)
- MRT exit locations: [LTA OneMap GeoJSON API]
- Geocoding: [OneMap Singapore API](https://www.onemap.gov.sg/docs/)

---

## ⚙️ Models Used

- 🔍 **Linear Regression** – interpretable baseline model
- 🌲 **Random Forest** – captures non-linear interactions
- 🚀 **XGBoost** – best predictive accuracy across multiple folds

We also engineered features like:
- Distance to MRT (using KDTree)
- Distance to CBD
- Month index (`month_numeric`) to capture time trend
- Town (one-hot encoded or target encoded)

---

## 📈 Insights

- Remaining lease, floor area, and town are strong predictors of price
- Flats closer to MRT and CBD tend to command higher prices
- Policy interventions (like SSD in 1996) caused noticeable inflection points in pricing trends

---

