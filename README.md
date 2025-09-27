  # HR Analytics Dashboard – Demo Company

This project is inspired by an HR analytics dashboard exercise, reimagined with a fully **synthetic dataset**.  
Instead of relying on the widely reused IBM HR dataset, every column here has been **randomised and modified** from a public example to create a more realistic, anonymised version.  

The goal is to build a structured, reproducible pipeline that prepares the data for **employee attrition analysis and dashboard visualisation**. With the cleaned dataset, we can explore insights such as:  

- 📊 **Attrition patterns** by department, job role, and age group  
- 👥 Workforce composition across education, gender, and marital status  
- ⏳ Career dynamics: years at company, promotions, and manager changes   

🛠️ **Status**: Dasboard in Progress
🔮 **Next Step**: Add reasoning notes, consistency checks, and first dashboard draft 
🔒 **Repo**: Private 

---

## 📌 Project Goals

- Build a **synthetic HR dataset** for portfolio use (randomised & anonymised from a public base)  
- Prepare a **clean data pipeline** for analysis and dashboarding  
- Explore **attrition patterns** by department, role, and demographics  
- Analyse **career dynamics**: years at company, promotions, manager changes  
- Develop a **dashboard** showcasing workforce and attrition insights  

---

## 📂 Project Structure


- [README.md](README.md) – Overview & docs  
- [notebooks/](notebooks/) – Jupyter notebooks  
  - [01. data preparation.ipynb](notebooks/01.%20data%20preparation.ipynb) – HR data cleaning  
- [data/](data/) – Datasets  
  - [original/](data/original/) – Raw HR data  
    - [HR Data.xlsx](data/original/HR%20Data.xlsx)  
  - [modified/](data/modified/) – Synthetic HR data  
    - [HRDataset_Synthetic_2025-09-27_19-18.xlsx](data/modified/HRDataset_Synthetic_2025-09-27_19-18.xlsx)  
- [dashboard/](dashboard/) – Dashboard (WIP)  
- [.gitignore](.gitignore) – Ignore raw/temp files  

---

### 🗂️ Folder Tree

```
root/
├── README.md
├── .gitignore
├── data/
│   ├── original/
│       └── HR Data.xlsx
│   └── modified/
│       └── HRDataset_Synthetic_2025-09-27_19-18.xlsx
├── notebooks/
│   └── 01. data preparation.ipynb
└── dashboard/
    └── soon
```
---


---

## 📊 Dataset Overview

- **Source**: Based on an HR dataset from the *Data Tutorials* YouTube channel  
- **Modification**: All 39 columns have been **randomised and anonymised** to ensure uniqueness and realism  
- **Coverage**: 1,470 employee records across multiple departments and roles  
- **Variables**: Demographics, job details, compensation, satisfaction, and attrition indicators  
- **Format**: Excel (.xlsx), prepared for cleaning, analysis, and dashboard visualisation  

---

## 🧹 Cleaning & Processing Summary

- **Preserved original schema**: all columns retained with same labels.  
- **Randomised contents** while keeping similar ratios to original distributions.  
- **Applied rules for realism**:  
  - Dept ↔ Job Role / Education Field  
  - Job Role ↔ Overtime  
  - Job Level ↔ Income & Stock Options  
  - Age ↔ Age Band ↔ Marital Status  
- **Career timeline checks**:  
  - `TotalWorkingYears` ≤ Age – 18  
  - `YearsAtCompany` ≤ TotalWorkingYears  
  - Other tenure fields capped and biased by Job Level.  
- **Adjusted imbalances**:  
  - All `Over18` = "Y"  
  - Balanced education levels  
  - Reduced excessive “0 years” in tenure-related fields  
- **Exported** final randomised dataset to `modified/` with timestamped filenames.

---

## ✨ Outputs

The project produces a **modified HR dataset** based on the IBM HR Analytics schema.  
- All columns from the original dataset are preserved.  
- Values are **randomised and rebalanced** with realistic business rules (e.g., JobRole ↔ Department, JobLevel ↔ Income, Tenure constraints).  
- This ensures the data remains **anonymised** but still **credible for analysis and dashboarding**.  

Currently, a **modified version of the dataset is ready** and can be directly used to build dashboards and visualisations.  


---

## 🛡️ Disclaimer 

- This project is based on an HR dataset originally provided in a tutorial by the **Data Tutorials** YouTube channel.  
- All 39 columns have been **randomised and anonymised** to create a synthetic dataset suitable for portfolio and educational use.  
- The dataset is not identical to the one shared in the tutorial and does not contain any real employee records.  
- Original reference:  
  - [Data Tutorials YouTube Channel](https://www.youtube.com/@data_tutorials)  
