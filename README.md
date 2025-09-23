# 🏫 NYC Education Data Analysis & Database Integration

## 📌 Overview
This repository contains a collection of projects focused on cleaning, analyzing, and integrating datasets from the **New York City public school system**.  
It combines work across multiple tasks:  
1. **School Safety Report Exploration (Google Sheets)**  
2. **Python + SQL Analysis of School Demographics**  
3. **SAT Results Cleaning & Database Integration**  
4. **High School Directory & SPED/ELL Analysis**  

The goal is to produce **clean datasets**, perform **relational queries**, and practice building pipelines that load real-world data into **PostgreSQL databases**.

---

## 📂 Datasets
- `school-safety-report.csv` → NYC incident-level safety data  
- `School_Safety_Report_Data_Dictionary.xlsx` → Reference for safety dataset  
- `high-school-directory.csv` → Attributes of NYC high schools  
- `sat-results.csv` → Raw SAT performance data  
- `cleaned_sat_results.csv` → Cleaned dataset prepared for database integration  

---

## 🎯 Objectives
- Explore dataset structures and identify meaningful columns  
- Clean and preprocess messy or inconsistent data  
- Analyze borough-level differences in incidents, ELL, and SPED support  
- Write SQL queries to aggregate and rank schools  
- Connect Python to PostgreSQL and insert cleaned datasets  

---

## 🛠️ Tools Used
- **Google Sheets** → initial cleaning, formulas, quick analysis  
- **Python (Pandas, SQLAlchemy, Psycopg2)** → preprocessing, queries, database loading  
- **PostgreSQL** → relational schema and storage  
- **Jupyter Notebook** → interactive workflows  

---

## 📊 Key Insights

### School Safety Report (Day 1)
- Total rows: ~1000+  
- Unique schools: ~322  
- Most frequent incident type: **non-criminal incidents**  
- Bronx accounts for ~28% of incidents  

### Python + SQL Analysis (Day 3)
- Schools by borough: Brooklyn (121), Bronx (118), Manhattan (106), Queens (80), Staten Island (10)  
- Avg ELL % in Manhattan: ~7.6%  
- East Side Community School (Manhattan) has >28% SPED students  

### SAT Data Integration
- Cleaned messy CSV into `cleaned_sat_results.csv`  
- Removed duplicates and standardized formats  
- Inserted into PostgreSQL using SQLAlchemy  
- Schema mapped DBN → `school_id`, SAT scores → subject fields  

---

## 📌 Future Improvements
- Expand SQL queries to cover all boroughs for ELL & SPED  
- Add charts and visualizations for borough comparisons  
- Automate data cleaning and ETL pipeline with scripts  
- Build dashboards with **Looker Studio** or **Streamlit**  

---

## 📜 License
MIT License – free to use and adapt.  
