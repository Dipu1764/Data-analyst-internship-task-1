# Data-analyst-internship-task-1

**🩺 Medical Appointment No-Show – Data Cleaning Summary Report**
Objective:
To clean and standardize the medical appointment dataset by addressing missing values, duplicates, inconsistent formatting, and incorrect data types.

**1. Column Renaming:**

All column headers converted to lowercase with underscores.

Example: "Appointment Date" → appointment_date.

**2. Duplicate Removal:**

Removed 2,921 duplicate rows.

Before: 49,593 rows → After: 46,672 rows.

**3. Handling Missing Values:**

age: Filled with median.

gender, city: Replaced with 'Unknown'.

appointment_date, date_of_birth, entry_service_date: Converted to datetime, forward-filled; dropped rows with critical missing dates.

**4. Text Standardization:**

gender: Standardized to 'MALE', 'FEMALE', 'UNKNOWN'.

city: Converted to title case.

no_show: Mapped 'Yes' → 1, 'No' → 0.

**5. Date Format Conversion:**

Columns appointment_date, date_of_birth, and entry_service_date converted to datetime64[ns].

**6. Data Type Fixes:**

age: Converted to int.

Other numeric columns (if any): Converted to appropriate float type.

**Result:**
The dataset is now cleaned, standardized, and ready for exploratory data analysis or machine learning workflows.
