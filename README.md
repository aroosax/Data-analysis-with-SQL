# 📉 Layoff Analysis Project (2020–2023)

This project focuses on analyzing employee layoffs from various companies around the world between 2020 and 2023. The goal was to clean and analyze the dataset to uncover trends and insights related to layoffs during this period.

---

## 🗂️ Dataset Overview

- **Source:** Layoffs dataset containing information on company name, industry, location, number of employees laid off, total staff, percentage laid off, stage, funding, and date of layoff.
- **Time Period:** 2020 to 2023
- **Rows:** ~2,300
- **Columns:** Company, Industry, Location, Total Laid Off, Percentage Laid Off, Date, etc.

---

## 🧹 Data Cleaning Process

The following steps were performed to clean and prepare the data for analysis using SQL:

1. **Removed Duplicates:**  
   Identified and removed duplicate rows using `ROW_NUMBER()` and `DELETE`.

2. **Standardized Data:**  
   Cleaned inconsistent formats in columns such as:
   - Converted all text to lowercase
   - Trimmed spaces
   - Fixed inconsistent company/industry names

3. **Handled NULL and Blank Values:**  
   - Replaced blank strings with `NULL`
   - Removed rows where important columns (like company or industry) were missing

4. **Removed Unnecessary Columns:**  
   Dropped irrelevant or empty columns to streamline the dataset

5. **Converted Data Types:**  
   Converted date strings to proper `DATE` format using `STR_TO_DATE()`

---

## 📊 Exploratory Data Analysis (EDA)

Using SQL queries, I performed EDA on the cleaned dataset to answer questions like:

- 📌 Which companies had the highest number of layoffs?
- 🏭 What industries were affected the most?
- 🌍 Which countries or cities saw the most layoffs?
- 📈 How did layoffs change over time from 2020 to 2023?
- 🔄 What percentage of employees were laid off by each company?

---

## 🛠️ Tools & Skills Used

- **SQL** (MySQL Workbench)
- `ROW_NUMBER()`, CTEs, Joins, Aggregates
- Data Cleaning Techniques
- EDA using SQL queries
- Git & GitHub

---

## 📁 Folder Structure

```bash
├── README.md
├── layoffs.csv                          # Raw data table
├── Data Cleaning.sql                    # Cleaned data queries
├── Exploratory Data Analysis.sql        # EDA queries
