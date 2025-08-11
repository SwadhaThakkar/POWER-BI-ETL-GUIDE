# 📊 Power BI Learning Repository

This repository documents my journey of learning **Power BI**, focusing on **Extract, Transform, and Load (ETL)** processes using **Power Query**.  
It includes detailed notes, key concepts, and the final project where multiple datasets are cleaned, transformed, and combined.

---

## 📂 Course Structure

### 1️⃣ Power BI Fundamentals
- What is Power BI?
- Importance of ETL in Power BI
- Power BI Interface and Workflow Overview

### 2️⃣ Connecting to Data Sources
- Supported Data Sources in Power BI
- Local vs. Shared Datasets
- Power BI Connectors
- Connecting to Excel, Databases, and Cloud Sources

### 3️⃣ Storage Modes in Power BI
- Import Mode
- Direct Query Mode
- Dual Mode
- Choosing the right mode for your scenario

### 4️⃣ Data Types in Power BI
- Numeric
- Text (Unicode)
- Date/Time
- Logical (True/False)
- Binary

### 5️⃣ Data Transformation in Power Query
- Applied Steps Pane
- Removing / Renaming Columns
- Filtering Rows
- Handling Empty or Error Values
- Data Type Conversion
- Removing Duplicates
- Merging & Splitting Columns
- Pivot and Unpivot

### 6️⃣ Data Loading in Power BI
- Load vs. Load To
- Loading to the Data Model
- Performance considerations

### 7️⃣ Data Profiling in Power BI
- Column Quality (Valid, Empty, Error)
- Column Distribution (Distinct, Unique values)
- Column Profile (Min, Max, Average, Mode)
- Identifying and removing anomalies/outliers

### 8️⃣ Combining Tables: Append & Merge
- Append Queries
- Merge Queries
- Join Types in Power BI (Inner, Left Outer, Full Outer)

#### 8.1 Append Queries
#### 8.2 Merge Queries
#### 8.3 Join Types in Power BI
#### 8.4 Best Practices

---

### 9️⃣ Reference Queries & Dataflows in Power BI
- Reusing queries
- Creating consistent transformations
- Using Dataflows for ETL in Power BI Service

### 🔟 Data Profiling in Power BI (Advanced)
- Deeper profiling for anomaly detection
- Using profiling to clean large datasets

### 1️⃣1️⃣ Combining Queries (Append & Merge) in Practice
#### A. Append Queries – Combining multiple years of sales data  
#### B. Merge Queries – Adding additional columns from related tables

### 1️⃣2️⃣ Advanced ETL Features in Power BI
- Parameters
- Conditional Columns
- Custom Columns using M language
- Staging Queries

### 1️⃣4️⃣ Common Data Errors in Power BI
- Missing / Null values
- Duplicate Rows
- Inconsistent Data Types
- Extreme values (outliers)

### 1️⃣5️⃣ Dataset Endorsement & Governance in Power BI
- Promotion vs. Certification
- Privacy Levels (Private, Organizational, Public)
- Security considerations

### 1️⃣6️⃣ Best Practices for ETL in Power BI
- Filter early, reduce data at source
- Use numeric join keys
- Avoid unnecessary columns
- Profile before loading

---

## 🏆 1️⃣7️⃣ Final Project – Transforming Multiple Data Sources

**Case Study**: Adventure Works sales data for 2022 & 2023, with detailed order information.

**Steps performed**:
1. **Import Data**
   - Order2022.xlsx  
   - Order2023.xlsx  
   - OrderDetails.xlsx  

2. **Clean OrderDetails Table**
   - Kept only: SalesOrderID, ProductID, OrderQty, UnitPrice
   - Removed unnecessary columns
   - Checked Column Quality for valid/error/empty values

3. **Detect & Remove Anomalies**
   - Used Column Profile to check min, max, average for UnitPrice
   - Removed 3 extreme outlier values

4. **Append Tables**
   - Combined Order2022 & Order2023 into one `Orders` table

5. **Merge Tables**
   - Merged `OrderDetails` with `Orders` on `SalesOrderID`
   - Selected **Inner Join**
   - Expanded only the `OrderDate` column

6. **Rename & Finalize**
   - Renamed `Orders.OrderDate` to `OrderDate`
   - Ensured final cleaned dataset is ready for reporting

---

## 📌 Repository Contents
- 📁 `/notes` → Detailed topic-wise notes in Markdown / Jupyter Notebook
- 📁 `/datasets` → Sample datasets used (Adventure Works)
- 📁 `/projects` → Final project Power BI file (`.pbix`)
- 📄 `README.md` → This file

---

## 🚀 Learning Outcome
- Gained hands-on experience with **end-to-end ETL in Power BI**
- Learned to **profile, clean, and combine multiple data sources**
- Applied **best practices for efficient data modeling**
- Understood the role of **data governance and dataset endorsement**

---

📅 **Course Completion Date**: *August 2025*  
✍️ **Author**: *[Your Name]*  
