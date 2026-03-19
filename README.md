# 📦 K.M Logistics & E-Commerce Sales Analytics (End-to-End Excel Project)

## 📊 Executive Summary
In the high-volume e-commerce sector, logistics and marketplace performance dictate profitability. This project executes an end-to-end data analysis pipeline on 31,000+ raw transactional records from K.M Logistics Pvt. Ltd. (2022 data).

The objective was to transform fragmented, corrupted raw data into a dynamic, interactive executive dashboard. By engineering new demographic features and standardizing logistics states, this analysis provides immediate visibility into **Marketplace Dependency, Demographic Purchasing Trends, and Regional Fulfillment Success.**

---

## 🛠️ Technical Stack & Skills Demonstrated
* **Tool:** Advanced Microsoft Excel (Office 365)
* **Data Engineering (Power Query/Native Excel):** Date restoration, Null-handling, Text normalization, Duplicate removal.
* **Feature Engineering (Formulas):** Nested `IF` statements, `VLOOKUP`/`XLOOKUP`, custom binning (Age/Demographics).
* **Data Visualization & BI:** Pivot Tables, Pivot Charts, Interactive Slicers, Dashboard UI/UX Design.

---

## 🗄️ Phase 1: The Raw Data Landscape
The initial dataset consisted of unstructured transactional logs tracking individual parcels across major Indian marketplaces.

* **Order Identifiers:** Unique Order IDs and SKU codes mapping to specific inventory units.
* **Logistics Status:** Real-time shipment states (e.g., Delivered, Cancelled, Refunded, RTO).
* **Sales Channels:** Attribution across Amazon, Flipkart, Myntra, Ajio, and Nalli.
* **Geographic Data:** Destination mapping via City, State, and Pincode.
* **Financials:** Order valuation standardized in INR.

<img width="1918" height="1008" alt="Raw Data Preview" src="https://github.com/user-attachments/assets/fd4ea198-b2cf-48b6-8863-6f46b5864e78" />

---

## 🧹 Phase 2: Data Transformation & "Dirty Data" Resolution
Real-world logistics data is notoriously messy. A significant portion of this project focused on ETL (Extract, Transform, Load) principles to convert 31,000+ records into a verified, analysis-ready dataset.

### 1. Structural Repair & Normalization
* **Date Restoration:** Resolved widespread "########" overflow errors in the raw timestamp column. Standardized dates into a strict `DD-MM-YYYY` format and extracted a separate **Month** dimension to enable seasonality and trend forecasting.
* **Categorical Unification:** Cleaned the 'Gender' column, using conditional logic to merge inconsistent manual entries (e.g., "M", "Men", "Male") into strict binary categories (**Men** / **Women**).
* **Status Verification:** Standardized fulfillment statuses to ensure "Delivered," "Cancelled," and "Refunded" orders were mutually exclusive, preventing the double-counting of recognized revenue.

### 2. Feature Engineering for Business Intelligence
To generate deeper insights beyond surface-level metrics, I engineered new analytical dimensions:
* **Demographic Segmentation:** Created custom logic to bucket customers into specific age cohorts (**Teen, Adult, Senior**). This enables highly targeted marketing analysis (e.g., *Isolating the Adult cohort's preference for Sarees vs. Western Wear*).
* **Channel Grouping:** Standardized vendor inputs to accurately attribute market share across Amazon, Flipkart, Myntra, and Ajio.

### 3. Quality Assurance (QA)
* **Data Cleansing:** Identified and purged redundant transaction IDs to prevent the overstatement of critical Sales KPIs. Addressed missing values in geographic fields to ensure regional heatmaps were comprehensive.

<img width="1920" height="1003" alt="Cleaned Data Preview" src="https://github.com/user-attachments/assets/07da7a1c-0808-4a08-bce6-e6275e4959c6" />

---

## 📈 Phase 3: E-Commerce Apparel Sales Performance Dashboard

## 📌 Project Overview
This project is an end-to-end data analysis of an e-commerce apparel retailer. The objective of this project is to analyze raw sales data, uncover purchasing trends, and build an interactive dashboard using Microsoft Excel to help stakeholders make data-driven decisions regarding inventory, marketing channels, and target demographics.

## ⚠️ Data Disclaimer
**Please Note:** The dataset used for this project is strictly for **educational and portfolio demonstration purposes**. 
* The data is synthetic/mocked and does not represent the actual proprietary sales, revenue, or customer data of any real-world companies or platforms mentioned (e.g., Amazon, Myntra, Flipkart, Ajio). 
* Any resemblance to real company figures or demographic behavior is purely coincidental. 
* This project is a proof-of-concept to demonstrate data cleaning, aggregation, and visualization skills in a simulated business environment.

## 🛠️ Tools & Technologies Used
* **Microsoft Excel:** Data Cleaning, Data Processing, Pivot Tables, Pivot Charts, Dashboard Creation.

## 📊 Key Metrics & Insights Analyzed
The dashboard provides a macro-level view of business performance across several key dimensions:

1. **Monthly Sales Trends (`Month-Wise Sales`):**
   * Analyzed a full calendar year of sales across 8 apparel categories (Blouse, Bottom, Ethnic Dress, Kurta, Saree, Set, Top, Western Dress).
   * **Insight:** Identified peak purchasing months to help optimize future inventory stocking and seasonal marketing campaigns. (Note: Kurta and Sets consistently drive the highest volume).

2. **Channel Performance (`Channel-Wise Sales`):**
   * Evaluated revenue streams across 7 primary e-commerce platforms.
   * **Insight:** Amazon (35%) and Myntra (23%) dominate the sales channels, accounting for nearly 60% of total revenue. Resources should be heavily allocated to maintaining these platform relationships.

3. **Demographic Breakdown (`Gender & Age Category`):**
   * **Gender:** Women represent the overwhelming majority of the customer base, driving 69% of total sales compared to Men (31%).
   * **Age:** Adults constitute the primary purchasing segment (63%), followed by Old Adults (20%) and Teens (17%).
   * **Actionable Takeaway:** Marketing spend and product development should remain hyper-focused on Adult Women, as they are the core revenue drivers.

4. **Geographic Distribution (`Top 5 Sales by State`):**
   * Pinpointed the highest-performing regions.
   * **Insight:** Maharashtra and Karnataka are the top two states for gross revenue. Regionalized targeted ad campaigns and localized supply chain hubs should prioritize these areas to reduce shipping times and increase market penetration.

## ⚙️ Methodology & Steps Taken
1. **Data Cleaning:** Standardized text formatting, handled missing values, and ensured data types (currency, dates) were accurate.
2. **Data Aggregation:** Utilized Excel Pivot Tables to summarize hundreds of thousands of rows of transactional data into digestible metrics.
3. **Data Visualization:** Built dynamic charts tied to the pivot tables to represent the data visually, ensuring stakeholders can understand performance at a glance.
4. **Dashboard Assembly:** Designed a clean, centralized layout placing the most critical KPIs (Sales by Channel, Demographics, and Time) into a single viewport.

## 🚀 How to Use This Repository
1. Download the `.xlsx` file included in this repository.
2. Open in Microsoft Excel (2016 or newer recommended for full chart compatibility).
3. Navigate to the `Dashboard` tab to view the visual summary.
4. Raw data and pivot calculations are located in their respective, labeled sheets for deep-dive analysis.

<img width="1919" height="1010" alt="Analytical Charts" src="https://github.com/user-attachments/assets/2c1be1c0-65e7-4956-91ba-131df36d6afa" />

---

## 🎯 Phase 4:  E-Commerce Apparel Sales: Aggregation & Insights Report

## 📌 Project Overview
This project focuses on data processing and aggregation for an e-commerce apparel retailer. The objective is to transform raw, transactional data into high-level pivot summaries to extract actionable business insights regarding customer demographics, regional performance, and sales channel efficiency.

## ⚠️ Data Disclaimer
**Please Note:** The dataset used for this project is strictly for **educational and portfolio demonstration purposes**. 
* The data is synthetic/mocked and does not represent the actual proprietary sales, revenue, or customer data of any real-world companies or platforms mentioned (e.g., Amazon, Myntra, Flipkart, Ajio). 
* Any resemblance to real company figures, order volumes, or demographic behavior is purely coincidental. 
* This project is a proof-of-concept to demonstrate data cleaning, aggregation, and analytical skills in a simulated business environment.

## 🛠️ Tools & Technologies Used
* **Microsoft Excel:** Data Cleaning, Pivot Tables, Statistical Aggregation, Business Reporting.

## 📊 Key Business Insights Extracted
Based on the aggregated data of over 31,000 recorded transactions totaling ₹21,176,377 in gross sales, the following insights were established:

1. **Demographic Dominance (`Gender`)**
   * Women are the primary consumer base, accounting for ~69% of the total order volume (21,553 orders) and driving the vast majority of gross revenue. 
   * **Actionable Takeaway:** Marketing spend and product acquisition should remain heavily skewed toward the female demographic to maximize ROI.

2. **Age Segmentation (`Age Category`)**
   * The "Adult" segment (30-49 years) is the leading demographic, accounting for 43.57% of total sales. However, the "Teen" segment closely follows at 42.73%. 
   * **Actionable Takeaway:** The brand is successfully capturing both mature and youthful audiences. Campaigns can be split-tested to target these two distinct, highly profitable age groups.

3. **Regional High-Performers (`Top 10 States`)**
   * Sales are heavily concentrated in specific regions. Maharashtra, Karnataka, and Uttar Pradesh form the top tier of regional sales, collectively generating roughly 35% of total nationwide revenue.
   * **Actionable Takeaway:** Supply chain logistics, warehouse distribution, and localized ad targeting should be prioritized in these three states to improve delivery times and capitalize on high demand.

4. **Sales Channel Efficiency (`E-Commerce Platforms`)**
   * The business is highly dependent on top-tier e-commerce aggregators. Amazon, Myntra, and Flipkart are the highest contributing channels, responsible for ~80% of total gross sales. 
   * **Actionable Takeaway:** While these platforms are crucial for volume, the business should investigate strategies to boost direct-to-consumer sales or improve margins on lower-performing channels (like Meesho and Ajio) to reduce platform dependency.

## ⚙️ Methodology
1. **Data Aggregation:** Utilized Excel Pivot Tables to summarize high-volume transactional data into key business dimensions (Time, Geography, Channel, Demographics).
2. **Order Status Tracking:** Categorized order lifecycle states (Delivered, Cancelled, Refunded, Returned) to provide a baseline for future operational efficiency analysis.
3. **Insight Generation:** Translated raw pivot totals into percentage-based insights for clear, executive-level communication.

<img width="1901" height="999" alt="Annual Sales Overview" src="https://github.com/user-attachments/assets/18902c31-f46e-457c-ba4f-7fb59f6dffea" />

---

## 🕹️ Phase 5:  K.M. Logistics Pvt Ltd: 2022 Annual E-Commerce Sales Dashboard

## 📌 Project Overview
This project involves the end-to-end development of an interactive, executive-level Excel dashboard for "K.M. Logistics Pvt Ltd". The objective was to analyze an extensive dataset of 2022 e-commerce transactions, aggregate the data, and build a dynamic visual reporting tool. This dashboard empowers stakeholders to filter data dynamically and extract actionable insights regarding logistics performance, regional sales distribution, and customer demographics.

## ⚠️ STRICT DATA DISCLAIMER
**CONFIDENTIALITY NOTICE:** The data, company name (K.M. Logistics Pvt Ltd), and metrics presented in this project are **strictly synthetic and mocked for portfolio and educational purposes only**. 
* This dashboard does not contain, reflect, or utilize any real proprietary, confidential, or operational data from any actual entity named K.M. Logistics, nor does it reflect real data from the e-commerce platforms mentioned (Amazon, Flipkart, Myntra, etc.).
* All financial figures, order volumes, and demographic breakdowns are simulated to demonstrate data visualization and analytical competencies.

## 🛠️ Tools & Technologies
* **Microsoft Excel:** Advanced Data Cleaning, Pivot Tables, Pivot Charts, Slicer Integration, Dynamic Dashboard Design.

## 🎛️ Dashboard Features & Interactivity
This dashboard was built with user interaction in mind. It includes a centralized control panel utilizing **Excel Slicers**, allowing users to filter the entire dashboard's metrics simultaneously by:
* **Month:** To analyze seasonal trends and specific timeframes.
* **Category:** To drill down into specific apparel performance (e.g., Ethnic Dress vs. Western Dress).
* **Age Value:** To isolate purchasing behaviors of Teens, Adults, or Old Adults.
* **Channel:** To evaluate specific platform performance (e.g., Amazon vs. Ajio).
* **Gender:** To segment sales and logistics data by male or female consumer bases.

## 📊 Key Business Insights (2022 Annual Review)

1. **Logistics & Fulfillment Success (`Order Status`)**
   * The logistics pipeline is highly efficient, boasting a **92% successful delivery rate**. 
   * Cancellations sit at only 2%, and Returns at 3%, indicating strong inventory management and accurate product descriptions.

2. **Geographical Revenue Centers (`State-Wise Sales`)**
   * **Maharashtra (₹2.99M)** and **Karnataka (₹2.64M)** are the undisputed leaders in sales volume. 
   * **Actionable Insight:** K.M. Logistics should ensure its primary warehousing and last-mile delivery infrastructure is heavily concentrated in these states to maintain the 92% delivery success rate at scale.

3. **Demographic Dominance (`Gender Breakdown`)**
   * The consumer base is heavily skewed, with **Women accounting for 69% of total sales** compared to Men (31%).

4. **Temporal Trends (`Month-Wise Sales Hike`)**
   * A dual-axis analysis of Order Quantity vs. Total Amount reveals distinct seasonal peaks. Sales volume peaks sharply in **March**, followed by a steady decline through the summer, before stabilizing in Q4. 
   * **Actionable Insight:** Logistics staffing and warehouse capacity must be scaled up proactively in Q1 (Jan-Mar) to handle the annual volume surge.

5. **Channel Distribution (`Sales: Channel-Wise`)**
   * **Amazon (35%)** and **Myntra (23%)** are the dominant entry points for logistics volume. Integrating direct API connections with these specific platforms for shipping and tracking should be an operational priority.

<img width="1920" height="1005" alt="Interactive Dashboard" src="https://github.com/user-attachments/assets/6ef7ba49-347d-4f6d-af88-552943726743" />

---
 
**Contact:** [LinkedIn](http://www.linkedin.com/in/kaif-mahaldar-18300b333) | [Email](mailto:kaifmahaldar5@gmail.com)
