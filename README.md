# Hotel Operations — SQL Data Cleaning & Service Performance Analysis

This project analyzes hotel branch operations for **LuxurStay Hotels**, an international hotel chain.  
The goal is to clean the branch dataset, validate data quality, and analyze service performance to identify slow service issues affecting customer satisfaction.

This project was completed as part of a **DataCamp SQL Associate Practical Exam**.

---

## 🔍 Business Problem

LuxurStay Hotels has received complaints about slow room service in several branches.  
Customer satisfaction has dropped below the expected **4.5 rating**, and management wants to identify:

- Which branches have data quality issues  
- Which services take the longest  
- Which regions (EMEA, LATAM, APAC, NA) are underperforming  
- Which service–branch combinations have low average ratings  

Your task was to clean the data and generate insights using SQL.

---

## 🛠️ Skills Used

- SQL Data Cleaning  
- COALESCE, CASE, REPLACE  
- Handling missing values  
- Aggregations (AVG, MAX)  
- GROUP BY and HAVING  
- JOIN operations  
- Filtering by service and region  

---

## 📂 Project Tasks

### **Task 1 — Clean the Branch Table**
Applied cleaning rules:

- Missing location → `"Unknown"`  
- Missing total_rooms → `100`  
- Missing staff_count → `total_rooms * 1.5`  
- Missing opening_date → `2023`  
- Missing target_guests → `"Leisure"`  
- Corrected typos in target_guests (e.g., `"Busniess"` → `"Business"`)

---

### **Task 2 — Service Duration Analysis**
Calculated:

- Average time taken per service per branch  
- Maximum time taken  
- Rounded values to 2 decimal places  

This helps identify slow services and problematic branches.

---

### **Task 3 — Meal & Laundry Services in EMEA and LATAM**
Filtered results to show:

- Service description  
- Branch ID  
- Location  
- Request ID  
- Rating  

These services were specifically targeted by management for improvement.

---

### **Task 4 — Low-Rating Service–Branch Combinations**
Identified combinations where:

- `AVG(rating) < 4.5`  
- Rounded to 2 decimal places  

This highlights underperforming areas requiring immediate attention.

---

## 📁 Files Included

| File | Description |
|------|-------------|
| `hotel_operations.pdf` | Original DataCamp practical exam submission |
| `sql/task1_clean_branch.sql` | SQL for Task 1 |
| `sql/task2_avg_max_time.sql` | SQL for Task 2 |
| `sql/task3_meal_laundry.sql` | SQL for Task 3 |
| `sql/task4_low_rating.sql` | SQL for Task 4 |

---

## 🧠 Key Insights

- Several branches had incorrect or missing operational data.  
- Some services consistently took longer in specific regions.  
- Meal and Laundry services in EMEA and LATAM showed notable performance issues.  
- Multiple service–branch combinations fell below the 4.5 satisfaction threshold.  

---

## 👤 Author

**Bala Akhil Rajdeep Battula**  
Data & Technology Professional → Automotive Technology (WDTC Fall 2026)
