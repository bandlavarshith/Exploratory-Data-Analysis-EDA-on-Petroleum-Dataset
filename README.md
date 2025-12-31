# 📊 Exploratory Data Analysis (EDA) on Petroleum Dataset

## 📌 Project Overview

This project focuses on performing **Exploratory Data Analysis (EDA)** on a petroleum refinery dataset to understand operational patterns, shipment consistency, and refinery-level insights. The analysis uses statistical methods and visualizations to uncover trends, correlations, and anomalies in petroleum production and transportation data.

The goal is to transform raw operational data into **meaningful business insights** that can support better decision-making.

---

## 🎯 Objectives

* Understand the structure and quality of the petroleum dataset
* Identify key patterns and trends in refinery operations
* Analyze relationships between origin and destination shipment weights
* Detect anomalies, duplicates, and data quality issues
* Generate insights using univariate and bivariate analysis

---

## 📂 Dataset Description

The dataset contains **265 records and 7 columns**, capturing petroleum shipment details across different refineries and shifts.

### Key Columns:

* **Work Shift** – Day / Evening / Night shift
* **Type** – Product type (VB, C5+, Condensate, Iso-Recycle)
* **Refinery** – Refinery location (Tehran, Shiraz, South Pars, Pars Petrochemical)
* **Origin Departure Date** – Shipment departure date
* **Origin Net Weight** – Net weight at origin
* **Destination Arrival Date** – Shipment arrival date
* **Destination Net Weight** – Net weight at destination

---

## 🧹 Data Cleaning & Preprocessing

* Verified dataset size and structure using `df.shape` and `df.info()`
* Confirmed **no missing values**, ensuring high data completeness
* Identified and removed **one duplicate record**
* Converted dates from **Jalali format to Gregorian (YYYY-MM-DD)** for accurate analysis

---

## 📈 Exploratory Data Analysis

### 🔹 Univariate Analysis

* Analyzed distribution of work shifts and product types
* Observed that **VB is the dominant product type**
* Origin Net Weight values mostly range between **22,000 and 26,000**, with a few outliers

### 🔹 Bivariate Analysis

* Found a **very strong positive correlation (~0.998)** between Origin Net Weight and Destination Net Weight
* Identified refinery-wise variations in shipment volumes
* Observed operational specialization, where certain product types are processed by specific refineries

---

## 🔍 Key Insights

* Shipment weights are highly consistent between origin and destination, indicating minimal loss
* **Tehran and Shiraz refineries** handle higher shipment volumes
* VB is predominantly processed at Shiraz and Tehran
* Other product types show strong refinery-specific specialization
* Data shows stable and predictable shipment behavior

---

## ⚠️ Challenges

* Date conversion from Jalali to Gregorian format required additional preprocessing
* Highly imbalanced product categories limited comparative analysis
* Strong correlation between weights introduced redundancy
* Some refinery–product combinations had limited data

---

## 🛠️ Tools & Technologies Used

* **Python**
* **Pandas, NumPy** – Data manipulation
* **Matplotlib, Seaborn** – Data visualization
* **Jupyter Notebook** – Analysis environment

---

## 📌 Conclusion

This EDA project successfully revealed operational trends, refinery specialization, and shipment consistency within the petroleum dataset. Despite challenges like date conversion and category imbalance, the analysis produced **reliable and actionable insights** that can support operational and business decisions.
  
