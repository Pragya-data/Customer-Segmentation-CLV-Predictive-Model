# 📊 Customer Segmentation & Predictive CLV Model

**Author:** Pragya Singh  
**Tools Used:** Power BI, Power Query, DAX, K-Means Clustering Machine Learning

## 📑 Project Overview
The goal of this project was to transition from reactive historical reporting to proactive, predictive analytics. I engineered an end-to-end Business Intelligence tool that utilizes Machine Learning to automatically segment a customer database into distinct behavioral personas, allowing the marketing team to launch highly targeted, data-driven campaigns.

## 🏗️ Technical Architecture & Methodology

### 1. Data Pipeline & ETL (Power Query)
* Ingested flat raw data files and transformed them into a robust **1-to-Many Star Schema**.
* Created custom conditional columns and handled missing values to prepare the dataset for algorithmic clustering.

### 2. Business Logic & DAX 
Developed custom DAX measures to calculate core KPIs, including:
* **Customer Lifetime Value (CLV)**
* **Recency, Frequency, Monetary (RFM) modeling**
* **Average Order Value & Campaign Conversion Rates**

### 3. Machine Learning (K-Means Clustering)
Deployed a K-Means clustering algorithm directly within the Power BI environment to analyze the correlation between transaction frequency and total revenue. The algorithm successfully segmented the database into 4 primary behavioral clusters:
* **Cluster 1:** High Value / Loyalists
* **Cluster 2:** Low Value / Hibernating
* **Cluster 3:** High Frequency / At-Risk
* **Cluster 4:** Moderate Value / Promising

### 4. Interactive UI & Advanced Drill-Through
Designed an executive-facing dashboard featuring:
* **AI Decomposition Tree:** Allows managers to dynamically map revenue flow by age tier, preferred shopping channel, and assigned cluster.
* **Targeted Drill-Through Action Lists:** Engineered a hidden database layer that allows marketing teams to right-click any cluster or channel and instantly generate an exportable, targeted list of specific Customer IDs for campaign targeting.

## 📂 Repository Contents
* `Customer_Segmentation_CLV_Model.pbix`: The complete, interactive Power BI project file (requires Power BI Desktop to open).
* `Dashboard_Preview.pdf`: A static PDF export of the main executive dashboard and drill-through action list for quick viewing.

## 🚀 How to Use the Dashboard
1. Navigate the primary KPIs and K-Means scatter plot on the main Executive Dashboard.
2. Expand the **Revenue Drivers** Decomposition Tree to explore specific demographic flows.
3. **Generate an Action List:** Right-click on any cluster within the tree or the 'Preferred Channel' donut chart, select **Drill through**, and click **Action List** to view the raw customer data for that specific segment.
