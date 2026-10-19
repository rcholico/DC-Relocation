# 🚚 Distribution Center Location Optimization

**Applied Unsupervised Machine Learning for Supply Chain & Logistics Network Redesign**

An analytics and machine learning framework built for an orthopedic footwear company to optimize the geographic placement of the distribution center network reducing weighted shipping distances across North America.

---

## 🎯 Executive Summary & Problem Definition
Following the acquisition and sale of this orthopedic footwear brand, the distribution network required strategic re-evaluation. The objective was to analyze historical shipment data and apply machine learning algorithms to identify optimal warehouse locations that minimize overall transit distance and shipping zone costs.

---

## 📊 Dataset & Pipeline Overview

* **Raw Data:** 495,000+ shipment lines from FedEx Reporting across 42 data fields.
* **Data Preprocessing & Cleaning:** Filtered non-continental US states (HI, PR, AK) and cleaned data down to **378,000+ valid continental US shipment lines**.
* **Distance Calculation:** Calculated geodesic/Haversine distances from existing vs. candidate centroids.

---

## 🤖 Machine Learning & Modeling Approach

1. **Feature Engineering & Normalization:** Extracted spatial coordinates (Latitude, Longitude), normalized demand density, and scaled features.
2. **Model Selection (Unsupervised ML):** Applied **K-Means Clustering** using the **Elbow Method** to identify optimal centroid locations.
3. **Cluster Analysis & Interpretation:**
   * **1-Cluster Model (Centralized DC):** Evaluated a single centralized hub (e.g., Saint Paul / Midwest region) yielding ~483M aggregate miles.
   * **3-Cluster Model (Regional Multi-DC):** Modeled 3 regional hubs to drastically reduce average shipping zone transit.

---

## 💰 Key Impact & Financial Results
* **Distance Reduction:** Achieved a **15% reduction** in total shipping miles (from 569 Million down to 483 Million miles).
* **Freight Savings:** Identified estimated freight cost savings of **+$0.5M** through zone optimization and mileage reduction.

---

## 🛠️ Tech Stack & Methodology
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-Learn (K-Means Clustering), Matplotlib/Seaborn, Geopy
* **Domain Applications:** Supply Chain Network Design, Freight Spend Optimization, Unsupervised ML
