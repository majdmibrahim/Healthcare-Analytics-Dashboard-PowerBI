# 🏥 Healthcare Analytics Dashboard (Power BI)

This project presents an **interactive Power BI dashboard** for healthcare data analytics — designed to transform raw patient records into meaningful insights that support operational and financial decisions in hospitals and clinics.

---

## 📊 Project Overview

The **Healthcare Analytics Dashboard** provides a complete analytical view of patient visits, treatment costs, insurance coverage, and satisfaction levels.  
It helps identify trends, optimize resource allocation, and understand financial performance across departments and service types.

---

## ⚙️ Data Model

The data model consists of four key tables:

- **Visit Table**: Core transactional data including admission/discharge dates, costs, and procedures.  
- **Providers Table**: Information about healthcare providers and departments.  
- **Date Table (Custom)**: Created using DAX `CALENDARAUTO()` for flexible time-based analysis.  
- **DAX Calculation Table**: Disconnected table for storing measures and KPIs.

---

## 🧮 Key DAX Measures

Some of the main KPIs and measures include:

- **Total Billing Amount** = `[Total Medication Cost] + [Total Room Charges] + [Total Treatment Cost]`  
- **Out of Pocket** = `[Total Billing Amount] - [Total Insurance Covered]`  
- **Average Billing per Patient** = `DIVIDE([Total Billing Amount], [Total Patients])`  
- **Length of Stay** = `DATEDIFF([Admitted Date], [Discharged Date], DAY)`  
- **Patient Satisfaction Score (Avg)** = `AVERAGE([Satisfaction Score])`

---

## 🎨 Dashboard Design

- Designed dual-mode views: **Light Mode** and **Dark Mode**.
- Custom backgrounds created using **PowerPoint**.
- Interactive **slicers** for patient race, time filters, and departments.
- Dynamic **page navigation** to switch between themes.

---

## 🗺️ Key Visuals

- **Azure Map**: Displays Total Billing by City/State.  
- **Clustered Bar/Column Charts**: Analyze billing by procedure, department, and diagnosis.  
- **Cards**: Highlight key KPIs like Total Billing, Insurance Covered, and Out of Pocket.  
- **Slicers**: Allow filtering by race, month, quarter, and year.

---

## 💡 Insights Generated

- Clear visibility of top-performing departments and costly procedures.  
- Comparative view of insured vs. out-of-pocket costs.  
- Trends in patient satisfaction correlated with treatment costs.  
- Temporal patterns in admissions and discharges.

---

## 🧠 Technologies Used

- **Power BI Desktop**  
- **DAX (Data Analysis Expressions)**  
- **Power Query**  
- **Microsoft PowerPoint (for background design)**  

---

## 📷 Dashboard Previews

Light Mode  
![1](https://github.com/user-attachments/assets/f11c1b32-b888-43b5-921f-e67251e40a44)

Dark Mode  
![2](https://github.com/user-attachments/assets/34f3ed8e-1b3c-480a-bd60-aa2465a15caa)

With Slicers
![3](https://github.com/user-attachments/assets/9cb12ec3-6022-4d1c-b252-bed92565c083)

---

## 🚀 How to Use

1. Download the `.pbix` file.  
2. Open it in **Power BI Desktop**.  
3. Click **Refresh** to load or update data.  
4. Interact with slicers and visuals to explore the insights.  

---

## 📈 Future Enhancements

- Add patient-level prediction models using Power BI + Python integration.  
- Include automated report export (PDF/Email).  
- Expand dataset with demographic and performance metrics.

---

## 👤 Author

**Majd Ibrahim**  
[LinkedIn Profile](https://linkedin.com/in/majd-ibrahim-6a02bb200/)
📂 Project File: `Healthcare_Analytics_Dashboard_PowerBI_by_MajdIbrahim.pbix`  
📅 Year: 2025  

---

## 📎 License

This project is open for educational and portfolio purposes. Please give credit if you reuse or modify the design.





