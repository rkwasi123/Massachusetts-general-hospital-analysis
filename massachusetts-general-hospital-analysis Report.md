# 🏥 Healthcare Analytics – massachusetts-general-hospital-analysis
 

## 📑 Table of Contents  
- [📌 Project Overview](#-project-overview)  
- [📂 Dataset](#-dataset)  
- [🛠 Tools & Technologies](#-tools--technologies)  
- [📈 Dashboards & Insights](#-dashboards--insights)  
  - [🔹 1. Overview Dashboard](#-1-overview-dashboard)  
  - [🔹 2. Cost & Coverage Insights Dashboard](#-2-cost--coverage-insights-dashboard)  
  - [🔹 3. Patient Behavior Dashboard](#-3-patient-behavior-dashboard)  
- [📊 Project Workflow](#-project-workflow)  
- [📌 Key Takeaways](#-key-takeaways)  
- [🚀 How to Run This Project](#-how-to-run-this-project)  
- [📬 Contact](#-contact)  

---

## 📌 Project Overview
This project analyzes synthetic hospital patient records (Massachusetts General Hospital, 2011–2022) to uncover insights into:  
- Patient encounters and hospital utilization  
- Cost and insurance coverage trends  
- Procedure frequency and cost drivers  
- Patient behavior and readmissions  

The project was completed as part of the **STC 6-Week Data Analyst Mentorship Program**, with a focus on SQL, Power BI, and Data Storytelling.  

---

## 📂 Dataset
- **Patients Table** → demographics, marital status, race, gender  
- **Encounters Table** → admissions, discharge, class of encounter, costs, readmissions  
- **Payers Table** → insurance and coverage  
- **Procedures Table** → medical procedures performed  
- **Dictionary Table** → metadata reference  

---

## 🛠 Tools & Technologies
- **SQL (MySQL)** → cleaning & transformation  
- **Power BI** → dashboarding & storytelling  
- **Excel** → exploration and quick validation  

---

## 📈 Dashboards & Insights

### 🔹 1. Overview Dashboard  
![Overview Dashboard](Overview page.png)  

**Key Insights**  
- 27,891 total encounters, 974 unique patients  
- Ambulatory encounters = **44.95%**, followed by Outpatient (22.59%) and Urgent Care (13.14%)  
- YoY encounters increased by **40.13%**, MoM growth was modest at 1.64%  
- Peak encounters: **2014 (3,885)**; peak patients: **2014 Q1 (269)**, over 300% higher than 2011 Q1 (67)  

---

### 🔹 2. Cost & Coverage Insights Dashboard  
![Cost Dashboard](Cost Insight.png)  

**Key Insights**  
- Avg base cost per procedure = **$2,092**  
- Highest avg base cost procedure = **$21,111**  
- No-insurance patients have the **highest avg claim cost** ($4,920); dual-eligible patients the lowest ($1,551)  
- Payer coverage: **48.23%**; Self-pay encounters: **1,460**  
- Coronary artery bypass grafting = most expensive procedure (**$56,169**)  

---

### 🔹 3. Patient Behavior Dashboard  
![Patient Behavior](patients_behavior.png)  

**Key Insights**  
- Repeat encounter rate: **28.64%**  
- Readmissions within 30 days: **13,138**  
- Top readmitted patient (Collier Collier) accounted for **3.63%** of all encounters  
- Patient volumes peaked in **2014 Q1**; variability observed across years  
- Subset of patients drive disproportionate encounters → opportunity for **targeted care management**  

---

## 📊 Project Workflow
1. **Week 1 – Understanding the Problem**  
   - Defined business challenge & stakeholders  
   - Drafted business questions  

2. **Week 2 – Data Cleaning**  
   - Imported raw CSVs → staging tables in MySQL  
   - Cleaned patient names, standardized gender/marital status  
   - Converted text-based dates → proper datetime  
   - Removed duplicates, blanks, unnecessary fields  

3. **Week 3 – Data Analysis**  
   - SQL queries answered business questions (encounters per year, class %, >24hr encounters, procedures, readmissions)  

4. **Week 4 – Visualization**  
   - Built Power BI dashboards  
   - Designed KPIs with conditional formatting  
   - Storytelling structure: Overview → Cost → Patient Behavior  

---

## 📌 Key Takeaways
- **Operational:** Ambulatory & Outpatient dominate hospital visits  
- **Financial:** Inpatient = most costly; uninsured patients face highest costs  
- **Clinical:** Seasonal patient trends, 6%+ readmissions highlight care gaps  
- **Strategic:** Patient concentration suggests care management programs could reduce repeat admissions  

---

## 🚀 How to Run This Project
1. Clone the repository  
2. Load `patients.csv`, `encounters.csv`, `payers.csv`, `procedures.csv` into MySQL  
3. Run SQL scripts (`/sql` folder) to clean & transform  
4. Connect Power BI to curated MySQL schema  
5. Use DAX measures in `/measures` to replicate dashboards  

---

## 📬 Contact
👤 [Your Full Name]  
📧 [Your Email]  
🔗 [Your LinkedIn]  
