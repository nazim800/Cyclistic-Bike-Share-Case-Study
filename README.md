# 🚲 Cyclistic Bike Share Case Study using Microsoft Excel, SQL, and Power BI  
* *How does a bike-share navigate speedy success?*

![images](https://github.com/user-attachments/assets/9c8ff41c-dfe2-4715-bf8c-4a5f2c36da87)

## Introduction  
In this case study, I analyze historical data from a Chicago-based bike-share company to identify trends in how their customers use bikes differently. To answer the key business questions, I will follow the steps of the data analysis process: **Ask, Prepare, Process, Analyze, Share, and Act**.  

The main tools I used are **Microsoft Excel, SQL, and Power BI**.  

### Quick Links  
- **Data Source:** [divvy_tripdata](https://divvy-tripdata.s3.amazonaws.com/index.html)  
- **SQL Queries:**  
  1. [Prepare Data](https://github.com/nazim800/Cyclistic-Bike-Share-Case-Study/blob/main/Prepare%20Data%3A%20Gathering%20and%20Organizing%20Data.sql)  
  2. [Process Data](https://github.com/nazim800/Cyclistic-Bike-Share-Case-Study/blob/main/Process%20Data%3A%20Cleaning%20%26%20Transforming%20Data.sql)
- **Data Visualizations:** [Power BI Report](https://drive.google.com/file/d/1vEsGIJ5vIzH1VwP7J3JDYidcm2CKx2ck/view?usp=share_link) 

A more in-depth breakdown of the case study scenario is included below, followed by my [full report](https://drive.google.com/file/d/1yYHBa_VInSxs_rqUEXbVHXBBjIZR_ujW/view?usp=sharing).  

---

## Scenario  
As a junior data analyst on the marketing analyst team at Cyclistic, a bike-share company in Chicago, my role is to help uncover insights that drive business growth. The **Director of Marketing** believes that the key to the company’s future success lies in increasing the number of annual memberships.  

To support this goal, my team is focused on analyzing how **casual riders and annual members** differ in their usage of Cyclistic bikes. By identifying key trends and patterns, we aim to develop an effective marketing strategy that encourages casual riders to become annual members.  

Before implementing any strategy, our recommendations must be reviewed and approved by **Cyclistic’s executives**. To ensure a strong case, we will support our findings with **data-driven insights and professional visualizations** that clearly communicate the value of our proposed approach.  

---

## Background  
Cyclistic is a bike-share program that operates **5,800+ bicycles across 600 docking stations**. What sets Cyclistic apart is its commitment to inclusivity, offering:  
- Traditional bikes  
- Reclining bikes  
- Hand tricycles  
- Cargo bikes (for riders with disabilities)  

While **most users prefer traditional bikes**, about **8% opt for assistive options**. The majority of riders use Cyclistic for **leisure**, though **30% rely on it for commuting** to work.  

### Pricing Model  
Cyclistic offers **three pricing plans**:  
- **Single-ride passes**  
- **Full-day passes**  
- **Annual memberships**  

Customers using **single-ride or full-day passes** are classified as **casual riders**, while those who purchase **annual memberships** are considered **Cyclistic members**.  

### Business Challenge  
Financial analysis has shown that **annual members** are significantly **more profitable** than casual riders. Instead of attracting **new customers**, the Director of Marketing believes that **converting casual riders into annual members** will be crucial for Cyclistic’s long-term success.  

To achieve this goal, we need a **deeper understanding** of:  
- How **casual riders** and **annual members** differ in their bike usage  
- Why casual riders **might** buy a membership  
- How **digital marketing strategies** could influence their decision  

---

# Data Analysis Process  

## Phase 1: Ask – Defining the Problem  

### **Business Task**  
**Devise marketing strategies to convert casual riders to members.**  

### **Key Stakeholders**  
- **Director of Marketing** – Needs actionable insights to shape marketing campaigns.  
- **Executive Team** – Requires data-backed recommendations to approve funding.  
- **Marketing Analytics Team** – Supports your analysis and implements findings.  

### **Analysis Questions**  
Three key questions guide the marketing strategy:  
1. **How do annual members and casual riders use Cyclistic bikes differently?**  
2. **Why would casual riders buy Cyclistic annual memberships?**  
3. **How can Cyclistic use digital media to influence casual riders to become members?**  

**My assigned task:** Answer question #1 – How do annual members and casual riders use Cyclistic bikes differently?  

---

## Phase 2: Prepare – Gather and Organize Data  

### **Data Source**  
I used **Cyclistic’s historical trip data** (Jan 2024 - Dec 2024), which can be downloaded from **divvy_tripdata**. The data is publicly available under a **Motivate International Inc.** license.  

### **Data Organization**  
There are **12 files** (one per month) with the naming convention: `YYYYMM-divvy-tripdata`. Each file contains:  
- `ride_id` (Primary Key)  
- `rideable_type`  
- `started_at`, `ended_at`  
- `start_station_name`, `end_station_name`  
- `start_lat`, `start_lng`, `end_lat`, `end_lng`  
- `member_casual`
<img width="245" alt="image" src="https://github.com/user-attachments/assets/8a7efaf5-288b-48fe-b96c-d4bff3778e7c" />


### **Steps Taken**  
✅ **Download & Organize Data**  
✅ **Inspect Data** in Excel (structure, missing values, key columns)  
✅ **Verify Data Credibility** (privacy, accuracy, consistency)  

---

## Phase 3: Process – Cleaning & Transforming Data  

### **Data Cleaning Process**  
🔹 I used **SQL Server Management Studio (SSMS)** for efficient data cleaning and transformation.  

✅ **Removed Duplicate Rows** 

  <img width="218" alt="image" src="https://github.com/user-attachments/assets/0cc7e9d2-b517-4a0e-ac85-f34750571220" />

✅ **Checked for Missing Values**  

  <img width="237" alt="image" src="https://github.com/user-attachments/assets/9bcfa921-2842-49d4-932a-c15acf8b6fd8" />

✅ **Validated Data Types**  
✅ **Verified Primary & Foreign Keys**  

### **Combining Data Tables**  
I used the **UNION ALL** function in SQL to merge 12 months of trip data into one comprehensive table.  
  <img width="232" alt="image" src="https://github.com/user-attachments/assets/b20d83c0-1a8d-427d-b442-3e91d609f6ce" />

✅ **Documented Every SQL Query**  
✅ **Saved Cleaned Data as CSV**  

---

## Phase 4: Analyze – Identifying Trends  

1. **Imported Cleaned CSV into Power BI**  
  <img width="470" alt="image" src="https://github.com/user-attachments/assets/4c7e0623-e362-4229-85f6-340ce65f6e43" />

2. **Performed Calculations** (Ride Length, Day of the Week, Month, etc.)
  <img width="455" alt="image" src="https://github.com/user-attachments/assets/f9f3c139-8aa1-4e23-bf44-3687fc05b167" />

3. **DAX Query for Mode of Day**  
  <img width="282" alt="image" src="https://github.com/user-attachments/assets/e985a60a-cfe7-4995-9dcf-d95819a6a198" />


4. **Created Visual Tables:**  
   - **Average Ride Length** (Members vs. Casual Riders)
     <img width="171" alt="image" src="https://github.com/user-attachments/assets/cc59943d-169d-4681-a026-ce13c23f40d2" />
   
   - **Rides by Day of Week**
     <img width="216" alt="image" src="https://github.com/user-attachments/assets/49edccc9-7647-4062-986b-5d4459cb2671" />
   
   - **Total Rides by Weekday**
     <img width="113" alt="image" src="https://github.com/user-attachments/assets/398b5f56-bfc2-4418-bdd9-6bec4792a8a9" />

---

## Phase 5: Share – Insights & Visualizing Report  

### **Power BI Dashboard Highlights**  
  <img width="411" alt="image" src="https://github.com/user-attachments/assets/ab5ce59c-86b7-4cf7-90d5-0fc8bc9ef363" />

📊 **Ride Duration:**  

  <img width="318" alt="image" src="https://github.com/user-attachments/assets/55dcf95f-6848-410c-97ad-8c4d3454e1cb" />

- Casual Riders: **25 min avg. ride**  
- Members: **13 min avg. ride**  

📊 **Usage by Weekdays:**  

  <img width="374" alt="image" src="https://github.com/user-attachments/assets/b690b27c-b9ea-40b9-a10c-33ea788ca20d" />

- Casual riders prefer **weekend rides** (Sat & Sun)  
- Members maintain **consistent** weekday usage  

📊 **Total Rides by Weekday:**  

  <img width="383" alt="image" src="https://github.com/user-attachments/assets/93108b14-67e4-4a0d-97a8-9f2683673be5" />

- **Peak:** Saturday (~0.94M rides)  
- **Lowest:** Monday (~0.78M rides)  

📊 **Usage by Ride Type:**

  <img width="383" alt="image" src="https://github.com/user-attachments/assets/664867fd-4073-46e9-81da-71eb733cbfa5" />

- **Classic Bikes:** 23 min avg.  
- **Electric Bikes:** 12.4 min avg.  
- **Scooters:** 10.4 min avg.  

📊 **Bike Type Preference:**  

  <img width="354" alt="image" src="https://github.com/user-attachments/assets/b4dda527-3745-43bf-836e-a93b2207652d" />

- **Classic Bikes:** 50%  
- **Electric Bikes:** 46.7%  
- **Scooters:** 2.5%  

---

## Phase 6: Act – Recommendations & Conclusion  

### **Top 3 Recommendations**  
1️⃣ **Introduce a "Weekend Membership Plan"**  
   - Casual riders primarily ride on weekends.  
   - Offer **weekend-specific discounts** or a **limited-time membership**.  

2️⃣ **Enhance Bike Availability Based on Demand**  
   - **More classic bikes** at high-demand stations (weekends).  
   - **More electric bikes** in commuter-heavy areas (weekdays).  

3️⃣ **Targeted Digital Marketing to Convert Casual Riders**  
   - **App notifications & email offers** after casual rides.  
   - **"First-month free" or seasonal discounts** to encourage sign-ups.  
---
### **Conclusion**  
Casual riders represent a **significant conversion opportunity**.  
📢 **Targeted marketing efforts should focus on incentives that match their riding habits!** 🚴  
