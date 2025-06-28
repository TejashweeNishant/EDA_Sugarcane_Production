# 🌾 Sugarcane Production Analysis 📊

## 📌 Overview
This project is a comprehensive data analysis of global sugarcane production across various countries and continents. The aim is to extract meaningful insights regarding production volume, land usage, yield efficiency, and regional trends.

The dataset includes:
- Total sugarcane production (in tons)
- Production per person (in kilograms)
- Cultivated acreage (in hectares)
- Yield per hectare (Kg/Ha)
- Country and continent information

---

## 🎯 Objective
- Identify top sugarcane-producing countries
- Analyze the efficiency of production (Yield per hectare)
- Understand distribution across continents
- Detect outliers and anomalies
- Visualize patterns and relationships using charts

---

## 🗂 Dataset Information
- **Source:** Manually cleaned and preprocessed dataset
- **Total Records:** 103 countries
- **Attributes:**
  - `Country`
  - `Continent`
  - `Production(Tons)`
  - `Production_per_person(Kg)`
  - `Acreage(Hectare)`
  - `Yield(Kg/Hectare)`

---

## 🧹 Data Cleaning Steps
- Removed European-style number formatting (`.` as thousand separator, `,` as decimal point)
- Converted all numeric columns to proper float types
- Dropped rows with missing values in key numeric columns
- Removed unnecessary columns (like unnamed index)

---

## 📈 EDA & Visualizations

### 🌍 Distribution by Continent
```python
df['Continent'].value_counts().plot(kind='bar')
