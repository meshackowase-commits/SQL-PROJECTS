# SQL-Data-cleaning-
### SQL Project: Tech Layoffs Data Cleaning and Standardization

### 📌 Project Overview

This project focuses on data cleaning and standardization of a raw layoffs dataset using SQL. Unclean data with duplicates, inconsistent formatting, and missing records can heavily compromise downstream data analysis. The goal of this script is to transform messy raw data into a structured, accurate, and reliable dataset ready for executive insights and visualization.

* * *

### 🛠️ Key Data Cleaning Steps

The SQL script executes four main stages to ensure maximum data integrity:

1.  **Duplicate Removal**
    *   Identified duplicate rows using window functions (`ROW_NUMBER()`).
    *   Safely removed redundant observations without corrupting unique entries.
2.  **Data Standardization**
    *   Trimmed white spaces from text fields.
    *   Unified inconsistent naming conventions (e.g., standardizing industry names and country typos).
3.  **Date Format Conversion**
    *   Converted raw text date columns into a standardized `DATE` format (`YYYY-MM-DD`).
4.  **Handling Null Values & Structural Fixes**
    *   Populated missing fields where corresponding historical data was available.
    *   Removed entirely blank rows and dropped unneeded diagnostic columns to reduce storage size.

* * *

### 💻 Tech Stack

*   **Database Engine:** MySQL / PostgreSQL *(Update to match your dialect)*
*   **Concepts Used:** CTEs, Window Functions, String Operations, Type Casting, DDL & DML Commands

* * *

### 🚀 How to Run the Script

1.  Clone this repository to your local machine.
2.  Ensure you have a database instance initialized.
3.  Run the setup queries inside `1_data_cleaning.sql` sequentially.

* * *

### 📈 Next Steps

Now that the dataset is thoroughly cleaned, the next phase of this project involves conducting Exploratory Data Analysis (EDA) to uncover trends regarding which industries, locations, and funding stages were hit hardest by global layoffs.
