## **Python + SQL Education Data Exploration**
### 🎯 **Objective**

In this task, we combined Python and SQL to explore real-world education data.
The goal was to connect to a PostgreSQL database, query school-level information, and analyze results in a Jupyter Notebook.

### ✅ **Steps Performed**

#### 1.Database Connection

Used Python libraries (psycopg2 / SQLAlchemy) to establish a connection.

Connection setup reference: day3_sql_combined_with_creds.ipynb.

#### 2.SQL + Pandas Integration

Queried data using pandas.read_sql() and cursor-based fetching.

Displayed results in clean tabular format for analysis.

#### 3.Analysis Performed

#### 🧮 School Distribution

##### - Question: How many schools are there in each borough?

##### - Method: Queried school count grouped by borough.

#### 🎓 Language Learners

##### - Question: What is the average % of English Language Learners (ELL) per borough?

##### - Method: Aggregated borough-level averages using SQL, verified in pandas.

#### 🔗 Schools Supporting Special Needs

##### - Question: Which are the top 3 schools per borough with the highest % of special education students (sped_percent)?

##### - Method:

- Combined school demographics and high school directory data.

- Ranked schools by sped_percent.

- Selected top 3 per borough.

#### 📂 Files

day3_sql_combined_with_creds.ipynb → Database connection setup

day3_sql_analysis.ipynb → SQL queries + pandas analysis + answers

### 📊 **Key Insights**

- Distribution of schools across boroughs shows (insert your finding, e.g., Brooklyn has the highest number of schools).

- The average % of English Language Learners varies significantly by borough.

- Certain schools have disproportionately high special education enrollment, highlighting areas with specialized support.

### 🚀 **How to Run**

##### 1. Clone this repository and navigate to daily_tasks/day_3/.

##### 2. Ensure you have the following Python libraries installed:

pip install psycopg2 sqlalchemy pandas jupyter

##### 3. Open the notebooks:

jupyter notebook day3_sql_combined_with_creds.ipynb

jupyter notebook day3_sql_analysis.ipynb


##### 4. Update database credentials as needed and run cells in order.

### 📌 **Future Improvements**

- Automate query execution with reusable functions.

- Add visualizations (bar charts, heatmaps) for borough-level comparisons.

- Build a lightweight dashboard for interactive exploration.

### 📜 **License**

This project is released under the MIT License.
