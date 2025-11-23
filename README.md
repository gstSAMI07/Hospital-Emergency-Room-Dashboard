# 🏥 Hospital Emergency Room Dashboard

## 📌 Project Overview
This project is an interactive **Power BI dashboard** that analyzes Emergency Room (ER) performance metrics using real-world hospital data.  
The dashboard helps in understanding key trends such as:

- Patient arrival patterns  
- Waiting times and service times  
- Department referrals  
- Admission vs discharge trends  
- Overall ER efficiency  

The goal is to provide hospital management with clear, actionable insights to improve patient care and operational performance.

---

## 📁 Project Files
| File Name | Description |
|----------|-------------|
| `Hospital ER_Data.csv` | Raw dataset containing ER patient logs and details. |
| `Project hospital Room.pbix` | Power BI report file for the dashboard. |

---

## 📊 Dashboard Features

### **1. Patient Overview**
- Total number of patients
- Average waiting time
- Peak hour analysis

### **2. Department Referral Analysis**
- Count of patients referred to each department  
- Patients with “None” referral  
- Visual referral trends

### **3. Admission & Discharge Metrics**
- Number of admitted vs discharged patients  
- Reason for visit analysis  

### **4. Time-Based Insights**
- Hourly patient load  
- Daily/Monthly patterns  
- ER congestion times  

---

## 🛠️ Tools & Technologies
- **Power BI**
- **Microsoft Excel / CSV**
- **Data Cleaning & Modelling**
- **DAX (Data Analysis Expressions)**

---

## 📌 How to Use
1. Download the `.pbix` file from this repository.
2. Open it in **Power BI Desktop**.
3. Make sure the data source path of `Hospital ER_Data.csv` is correct.
4. Refresh the dataset to view the dashboard.

---

## 📈 Data Model
The data model is based on a single dataset with transformations applied using:
- Power Query
- DAX measures  
Examples include:  
```DAX
Patients Referred = CALCULATE(COUNTROWS('Hospital ER_Data'), 'Hospital ER_Data'[Department Referral] <> "None")
