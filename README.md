# monsoon_diseases_cases_dashboard
# 🌧️ Health Under the Clouds: Monsoon Impact on Disease Outbreaks (2024)

## 📌 Project Overview
This Power BI project analyzes the **relationship between monsoon rainfall patterns and mosquito-borne diseases** (Malaria, Dengue) across Indian cities during 2024.  
By integrating **rainfall/weather datasets** with **disease case records**, the dashboard provides **actionable insights** on outbreak patterns, vulnerable regions, and effectiveness of preventive measures.  

This project was developed as part of **ThunderByte 2025 Hackathon** under the theme *“Tech for a Rainy Day – Building Solutions for the Monsoon Season.”*

---

## 🎯 Objectives
- Identify **trends and correlations** between rainfall and disease outbreaks.
- Track **seasonal variations** in Malaria and Dengue cases.
- Highlight **high-risk regions** and demographic groups.
- Measure the **impact of preventive measures** such as spraying campaigns and awareness drives.
- Provide **predictive signals** for outbreak preparedness.

---

## 🗂️ Dataset Details
Two datasets were used for this project:

### 1️⃣ Rainfall Dataset (4800 records)
- **Columns**:  
  - Date  
  - Region  
  - City  
  - Rainfall_mm  
  - Rainfall_Type (Light, Moderate, Heavy)  
  - Temperature_C  
  - Humidity_%  
  - Rainfall_Impact_Score  
  - Wind_Speed  
  - Cloud_Cover  

### 2️⃣ Disease Dataset (4800 records)
- **Columns**:  
  - Date  
  - Region  
  - City  
  - Disease_Type (Malaria/Dengue)  
  - Cases_Reported  
  - Hospitalizations  
  - Deaths  
  - Age_Group  
  - Gender  
  - Preventive_Measures (Spraying, Medical Camp, Awareness Drive)  
  - Risk_Factor (High/Medium/Low)  

📌 Both datasets share a **common `Date` column** for merging inside Power BI ETL.

---

## 🔑 Key KPIs
- **Total Rainfall (mm)**  
- **Total Cases Reported**  
- **Hospitalizations**  
- **Fatalities**  
- **Mosquito Index** (calculated: `(Rainfall_mm × Humidity %) ÷ 100`)  
- **Case Fatality Rate (CFR)** = `(Deaths ÷ Cases_Reported) × 100`  
- **Preventive Impact %** = `(Cases_Prevented ÷ Total_Cases) × 100`

---

## 📊 Dashboard Features
The Power BI dashboard includes the following visualizations:

1. **KPI Cards** – Quick insights (Rainfall, Cases, Hospitalizations, Deaths, Risk Index).  
2. **Dual-Axis Line Chart** – Rainfall vs Disease cases trend over time.  
3. **Clustered Bar Chart** – Cases by region for comparison.  
4. **Donut Chart** – Distribution of cases by disease type (Malaria vs Dengue).  
5. **Stacked Column Chart** – Disease cases segmented by Rainfall Type (Light/Moderate/Heavy).  
6. **Heatmap (Matrix)** – Regional cases across months to highlight hotspots.  
7. **Scatter Plot** – Rainfall vs Cases with bubble size = Hospitalizations.  
8. **Gauge Chart** – Real-time Mosquito Risk Index indicator.  
9. **TreeMap** – Effectiveness of Preventive Measures.  
10. **Slicers** – Filters for Date, City, Region, Disease Type.  

---

## 🛠️ Tools & Technologies
- **Power BI** → Data visualization & dashboard creation.  
- **Power Query (M Language)** → ETL process, handling blanks/NA values, merging datasets.  
- **DAX (Data Analysis Expressions)** → Calculated fields & KPIs.  
- **Excel** → Data preparation and formatting.  
- **Python (optional)** → Initial cleaning and validation (Pandas, NumPy).  

---

## 🚀 Project Workflow
1. **Data Import**  
   - Loaded both datasets into Power BI.  
2. **Data Cleaning**  
   - Handled missing/NA values, corrected data types, and standardized city names.  
3. **Data Transformation**  
   - Merged datasets on `Date` and `City`.  
   - Created calculated columns (Mosquito Index, Fatality Rate, Preventive Impact).  
4. **Modeling**  
   - Built relationships between tables (Rainfall ↔ Disease).  
5. **Visualization**  
   - Designed interactive dashboard with charts, filters, and KPIs.  
6. **Insights**  
   - Heavy rainfall correlated with a spike in cases (10–14 day lag).  
   - Certain regions showed consistently high mosquito index and higher hospitalization rates.  
   - Preventive measures reduced case growth by ~15–20% in treated areas.  

---

## 🌍 Impact
- **Public Health Officials** → Prepare resources for outbreaks.  
- **Urban Planners** → Identify high-risk zones needing better drainage & spraying.  
- **Communities** → Awareness campaigns for at-risk populations.  
- **Researchers** → Use data for predictive outbreak modeling.  

---

## 📂 Project Structure
