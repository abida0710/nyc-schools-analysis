# 🧠 SAT Data Integration into PostgreSQL

This project demonstrates how to clean and integrate real-world SAT results data into a **PostgreSQL database** using Python. The dataset is intentionally messy and requires thoughtful preprocessing, cleaning, and schema mapping to ensure relational integrity.

---

## 🎯 Objective

- Analyze and understand the structure of a raw SAT dataset  
- Identify meaningful and relational columns  
- Clean and preprocess messy and inconsistent data  
- Write a script to connect to a PostgreSQL database  
- Insert the cleaned data into an existing schema using Python

---

## 📁 Files in This Repository

| File | Description |
|------|-------------|
| `sat_modeling.ipynb` | Main notebook containing data cleaning, inspection, and database integration logic |
| `sat-results.csv` | Raw, unprocessed SAT results dataset |
| `cleaned_sat_results.csv` | Cleaned version, ready for database insertion |

---

## 🧪 Project Workflow

### 🔍 1. Inspect the Dataset
- Loaded the dataset using `pandas.read_csv()`
- Explored column types, sample values, and row counts
- Verified compatibility with existing database schema

### 🧹 2. Clean & Preprocess Data
- Removed **duplicates** using `drop_duplicates()`  
- Replaced or dropped missing values using `fillna()` and `dropna()`  
- Standardized text fields and column formats  
- Selected only **relational and meaningful columns** (e.g. DBN, school name, borough, SAT scores)

### 🛢️ 3. Prepare for Database Insertion
- Matched column names and types to existing database schema  
- Mapped fields using `dtype` and ensured format compatibility  
- Removed invalid records and normalized data where needed

### 🔌 4. Connect to PostgreSQL
- Connected using `SQLAlchemy` and `create_engine()`  
- Established secure credentials for insertion  
- Ensured connection stability before pushing records

### 📤 5. Insert into Database
- Used `to_sql()` or `engine.execute()` to append data  
- Verified successful insertion through manual inspection or SELECT queries  
- Ensured **no duplicates** or schema violations occurred  

---

## ✅ Key Accomplishments

- ✅ Cleaned a messy real-world CSV into a usable relational format  
- ✅ Connected Python to PostgreSQL using SQLAlchemy  
- ✅ Inserted records using script-based workflow (no manual work)  
- ✅ Ensured data quality through duplicate removal and null handling  

---

## 🧰 Tech Stack

- Python 3.x  
- Pandas  
- SQLAlchemy  
- PostgreSQL  
- Jupyter Notebook  

---

## 📌 Future Improvements

- Add logging and error handling to the database pipeline  
- Build automated scripts (`.py`) for cron or CI/CD scheduling  
- Validate schema before pushing using `pydantic` or custom checks  
- Expand to visualizations and SAT score trends by borough or district

---

## 📝 License

MIT License – Free to use and modify.
