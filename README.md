# 📊 Customer Behaviour Analysis

This project analyzes customer shopping behavior using Python, stores processed data in PostgreSQL, and visualizes insights using Power BI.

---

## 🚀 Project Workflow

1. Data Collection (CSV file)
2. Data Cleaning & Preprocessing (Python - Pandas)
3. Database Storage (PostgreSQL)
4. Data Visualization (Power BI)

---

## 📁 Dataset

- File: `customer_shopping_behavior.csv`
- Contains:
  - Age
  - Category
  - Purchase Amount
  - Review Rating
  - Purchase Frequency
  - Discounts

---

## 🐍 Data Processing (Python)

### ✔️ Data Exploration
- `df.head()` → Preview data  
- `df.info()` → Structure of dataset  
- `df.describe()` → Statistical summary  

### ✔️ Handling Missing Values
- Checked using `df.isnull().sum()`
- Filled missing **Review Rating** using median per category

### ✔️ Data Cleaning
- Converted column names to snake_case  
- Renamed columns for better readability  

### ✔️ Feature Engineering
- Created `age_group` column using quartiles  
- Converted purchase frequency into numeric days  
- Removed unnecessary columns  

---

## 🗄️ PostgreSQL Integration

### 🔌 Connection Details
- Host: `localhost`
- Port: `5432`
- Database: `customer_behaviour`
- User: `postgres`

## 📊 Power BI Integration

### 🔗 Steps

1. Open Power BI Desktop  
2. Select **PostgreSQL connector**  
3. Enter:
   - **Server:** `localhost:5432`  
   - **Database:** `customer_behaviour`  
4. Enter your PostgreSQL credentials  

➡️ Data will be automatically loaded into Power BI.

---

## 📈 Dashboard Insights

- Customer segmentation (age groups)  
- Purchase trends  
- Category-wise sales  
- Discount impact  
- Frequency-based behavior  

---

## 🛠️ Tech Stack

- Python  
- Pandas  
- PostgreSQL  
- SQLAlchemy  
- Power BI  

---

## ⚡ How to Run

1. Clone the repository  
2. Add the dataset (`customer_shopping_behavior.csv`)  
3. Run the Jupyter Notebook  
4. Ensure PostgreSQL is running on `localhost:5432`  
5. Push data to the database  
6. Connect Power BI to PostgreSQL  
7. Build dashboards  

---

## 🎯 Conclusion

This project demonstrates an **end-to-end data pipeline**, from raw data processing to database storage and interactive dashboard visualization.
