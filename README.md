# 🔍 EDA of Kidney Disease Dataset

## 📂 Dataset Used
Raw dataset used during analysis:  
[🔗 Kidney_disease.csv](https://github.com/itsadil-7890/Cronic-EDA/blob/main/kidney_disease.csv)

---

## 🛠 Initial Setup

- Imported required Python libraries for EDA.
- Loaded the dataset into a Pandas DataFrame.
- Checked basic dataset info:
  - Number of rows and columns
  - Data types of all columns
  - Missing values
  - Duplicates (none found)
- Cleaned and standardized column names for readability.
- Converted object-type columns (like `Packed_Cell_Volume`, `Red_Blood_Cell_Count`, and `White_Blood_Cell_Count`) to float for analysis.
- Separated and identified categorical and numerical columns.

---

## 📊 Analysis Performed

### 🔤 Data Cleaning
- Corrected inconsistent/mistyped values in:
  - `Diabetes_Mellitus` (e.g., `' yes'`, `'\tyes'`, `'\tno'`)
  - `Coronary_Artery_Disease` (`'\tno'`)
  - `Target_Class` (`'ckd\t'`)
- Encoded `Target_Class` for binary classification.

### 📈 Exploratory Analysis
- Visualized **Age Distribution**.
- Analyzed:
  - `Hypertension`
  - `Bacteria`
  - `Appetite` (pie chart)
  - `Diabetes_Mellitus` (donut chart)
- Explored **Blood Urea** levels by CKD status:
  - Outliers in CKD group
  - Median higher in CKD group
  - Also visualized with violin plot
- Compared:
  - Average **Age** of CKD vs. non-CKD patients
  - **Blood Pressure** between CKD and non-CKD
  - **Albumin** levels vs. CKD status
  - **Hemoglobin** levels and relation with CKD
- Investigated variation of **Blood Pressure** with **Age**

---

## ✅ Conclusion

This EDA uncovered critical patterns in the dataset such as:
- CKD patients tend to have **higher blood urea**, **lower hemoglobin**, and **more outliers** in clinical measures.
- Data cleaning was crucial due to inconsistent categorical values.
- Age, blood pressure, and albumin levels appear to have strong relationships with CKD status.
- Proper data encoding and visualization techniques like violin plots and pie charts helped derive clear insights for potential health risk indicators.

---

> ✅ This project helps in identifying early signs of Chronic Kidney Disease using data-driven approaches.
