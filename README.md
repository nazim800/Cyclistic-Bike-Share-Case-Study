# 🚲 Cyclistic Bike Share Case Study using Spreadsheet, SQL, and Power BI  
* *How Does a Bike-Share Navigate Speedy Success?* *  
![image](https://github.com/user-attachments/assets/a9149887-8d0d-4d6b-91ad-2b43592f6fa0)

---

## 📌 Introduction  
In this case study, I analyze historical data from a **Chicago-based bike-share company** to identify trends in how customers use bikes differently.  

### 🔍 **Objective**  
To answer the key business questions, I follow the **Google Data Analytics** process:  
**Ask → Prepare → Process → Analyze → Share → Act**.  

### 🛠 **Tools Used**  
- **Microsoft Excel** – Data structuring & analysis  
- **SQL (MySQL / PostgreSQL)** – Data processing  
- **Power BI** – Data visualization  

---

## 🔹 Quick Links  

📂 **Data Source**: [Divvy Trip Data](https://divvy-tripdata)  

📝 **SQL Queries**:  
1. [Prepare Data](#)  
2. [Process Data](#)  

📊 **Data Visualizations**: [Power BI Dashboard](#)  

📄 **Full Case Study Report**: [View PDF](#)  

---

## 📖 Scenario  

As a **junior data analyst** on the marketing team at **Cyclistic**, my role is to uncover insights that drive business growth.  

The **Director of Marketing** believes that the key to Cyclistic’s future success lies in **increasing annual memberships**. My team is focused on analyzing how **casual riders** and **annual members** differ in their bike usage patterns.  

The ultimate goal is to develop an effective marketing strategy that **converts casual riders into annual members**.  

### 🌟 **Key Business Insights**  
✅ **Cyclistic operates** over **5,800 bicycles** across **600 docking stations**.  
✅ **Casual riders** use bikes for **leisure** (weekend peaks), while **annual members** use them for **commuting** (weekday consistency).  
✅ **Annual members** are **more profitable** than casual riders.  
✅ Converting **existing casual riders** into annual members is a **key growth opportunity**.  

---

## 🔎 **Phase 1: Ask - Defining the Problem**  

### 🎯 **Business Task**  
✅ Devise **marketing strategies** to convert **casual riders into members**.  

### 🏢 **Key Stakeholders**  
- **Director of Marketing** – Needs insights to shape campaigns.  
- **Executive Team** – Requires **data-backed recommendations** to approve funding.  
- **Marketing Analytics Team** – Supports analysis & implements findings.  

### ❓ **Analysis Questions**  
1. **How do annual members and casual riders use Cyclistic bikes differently?**  
2. **Why would casual riders buy Cyclistic annual memberships?**  
3. **How can digital media influence casual riders to become members?**  

📌 **Assigned Question:**  
**How do annual members and casual riders use Cyclistic bikes differently?**  

---

## 📊 **Phase 2: Prepare - Gathering & Organizing Data**  

### 📂 **Data Source**  
Cyclistic’s **historical trip data** (Jan 2024 – Dec 2024) from [Divvy Trip Data](https://divvy-tripdata).  

🔹 **Data Privacy**: No personally identifiable information is included.  

### 📑 **Data Organization**  
The dataset consists of **12 monthly CSV files** with columns such as:  
- `ride_id`, `rideable_type`, `started_at`, `ended_at`, `start_station_name`, `end_station_name`, `member_casual`.  

### 📋 **Steps to Prepare Data**  
1. **Download Data** – Obtain **12 months of trip data**.  
2. **Organize Files** – Store in structured folders (`raw_data`, `processed_data`).  
3. **Inspect Data** – Open in **Excel** to understand structure.  
4. **Verify Credibility** – Ensure accuracy and licensing compliance.  

### 🔗 **Combining Data Tables**  
To merge all 12 months of data, I used **SQL (`UNION ALL`)** to consolidate them into one dataset.  

---

## 🛠 **Phase 3: Process - Cleaning & Transforming Data**  

### 🖥 **Data Cleaning in SQL Server (SSMS)**  
✅ **Removed duplicate rows** to prevent skewed analysis.  
✅ **Handled missing values** appropriately.  
✅ **Validated data types** to ensure consistency.  
✅ **Checked primary & foreign keys** for relational integrity.  

### 📝 **Documenting Data Cleaning**  
- **Issues Identified:** Null values, duplicates, inconsistent formats.  
- **SQL Queries Used:** Cleaning, filtering, and transforming data.  
- **Final Validation:** Ensuring **data integrity** before analysis.  

🔹 **Final Output**: Cleaned dataset exported to **CSV** for visualization.  

---

## 📈 **Phase 4: Analyze - Identifying Trends**  

📊 **Data imported into Power BI** for calculations & visualization.  

### 🔢 **Key Calculations**  
- **Average Ride Length**  
- **Max Ride Length**  
- **Most Frequent Ride Day (Mode Calculation - DAX Query)**  

### 📋 **Key Findings**  

1️⃣ **Ride Duration**  
   - **Casual Riders**: 🚲 **25 min avg. ride** (Leisure-focused).  
   - **Members**: 🚴‍♂️ **13 min avg. ride** (Commute-focused).  

2️⃣ **Usage by Weekdays**  
   - **Casual Riders**: Peak on **weekends** (Sat/Sun).  
   - **Annual Members**: Consistent **weekday usage**.  

3️⃣ **Total Rides by Weekday**  
   - **Highest:** 🚴‍♂️ **Saturday (~0.94M rides)**.  
   - **Lowest:** 🚲 **Monday (~0.78M rides)**.  

4️⃣ **Usage by Rideable Type**  
   - **Classic Bikes**: 🚴‍♂️ **23 min avg.** (Longer trips).  
   - **Electric Bikes & Scooters**: ⚡ **12-14 min avg.** (Quick commutes).  

---

## 📊 **Phase 5: Share - Visualizing Report**  

### 📌 **Power BI Dashboard Insights**  

📊 **Visualizations show clear differences between user types:**  
✅ **Casual riders = leisure-focused** (weekend usage).  
✅ **Annual members = commuter-focused** (weekday consistency).  
✅ **Classic bikes dominate longer rides**, while **electric bikes/scooters = quick trips**.  

🔹 **Data-Backed Implications**  
- **Casual riders = weekend users** → Target **weekend promotions**.  
- **Annual members = commuters** → Optimize **bike availability on weekdays**.  
- **Electric bikes for quick trips** → Expand fleet in **urban commuter areas**.  

---

## 🎯 **Phase 6: Act - Recommendations & Conclusion**  

### 🔥 **Top 3 Recommendations for Cyclistic**  

1️⃣ **Introduce a "Weekend Membership Plan"**  
   - Casual riders **prefer weekends** → Offer **weekend-based membership plans**.  

2️⃣ **Enhance Bike Availability Based on Demand**  
   - Increase **classic bikes on weekends** (high leisure demand).  
   - Deploy **more electric bikes in commuter areas**.  

3️⃣ **Targeted Digital Marketing for Conversion**  
   - **Push notifications** to casual riders with **membership perks**.  
   - **Offer discounts** for **first-time membership sign-ups**.  

---

## 📌 **Conclusion**  

🔹 **Casual riders represent a key conversion opportunity.**  
🔹 **Targeted marketing & optimized pricing plans** can **boost memberships**.  
🔹 **Cyclistic should focus on incentives** that align with **riding habits**.  

🚀 **With data-driven insights, Cyclistic can increase revenue & user engagement!**  

---

Let me know if you need any refinements! 🚴‍♂️✨  
