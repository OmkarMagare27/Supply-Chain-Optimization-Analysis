Dashboard: https://app.powerbi.com/groups/me/reports/a00f6e66-a457-4ebf-8a4b-a0f7860570b3?experience=power-bi
Dashboard Screenshot: 
![image](https://github.com/user-attachments/assets/83a606df-14ac-4b3d-9ce5-4c42245d7057)


## Supply Chain Analysis Project
# Table of Contents
1 Project Overview
2 Data Sources
3 SQL Query Explanation
4 Python Script Explanation
5 Dashboard Overview
6 Metrics and KPIs
7 Technologies Used
8 Instructions to Run
9 Future Enhancements


1. Project Overview
This project analyzes the supply chain performance of multiple cities across various stores. The main goal is to evaluate the On-Time, In-Full (OTIF) delivery performance across different metrics such as Order Lines, Volume Fill Rate, Line Fill Rate, and OTIF %. The dashboard helps identify gaps between actual performance and target KPIs, aiding in strategic decision-making and operational improvements in supply chain management.

2. Data Sources
Orders Data: Contains customer orders and their line items.
Delivery Data: Includes information on delivered quantities per line item and whether the deliveries were on-time.
Product Categories: Information on different product categories, including total ordered and delivered quantities.

3. SQL Query Explanation
The SQL query used in this project extracts relevant information from the database to calculate key metrics:

Orders and Order Lines: Fetches customer orders and line items, assigning a unique order ID and line details.
On-Time and In-Full Metrics: Queries data to determine if each order was delivered on time and in full, generating the key performance indicators (KPIs) for OTIF %.
Aggregating Metrics by Region: Calculates performance metrics at a regional level (Ahmedabad, Surat, Vadodara), focusing on order accuracy and fulfillment.
Joining Tables: Combines customer, product, and order data to create a comprehensive dataset for further analysis in the Power BI dashboard.

4. Python Script Explanation
The Python script enhances data pre-processing and metric calculations, preparing the dataset for the Power BI dashboard. Below are the key sections:

Data Cleaning: Processes raw data by removing null values, ensuring consistency in date formats, and transforming categorical variables for analysis.
Metric Calculations: Computes advanced metrics such as Line Fill Rate (LIFR), Volume Fill Rate (VOFR), and OTIF % using custom formulas to derive insights from the data.
Visualization Prep: Formats the data for visualizations, such as time series plots for weekly trends in OTIF performance.

5. Dashboard Overview
The Power BI dashboard visualizes key supply chain metrics, providing insights across different cities and stores. Key components include:

City-wise Performance: Shows OTIF %, Line Fill Rate (LIFR %), and Volume Fill Rate (VOFR %) for Ahmedabad, Surat, and Vadodara.
Weekly Trends: Analyzes week-wise performance against targets for OTIF, On-Time %, and In-Full %.
Store-level Analysis: Compares performance across various stores such as Acclaimed Stores, Lotus Mart, and Expert Mart, highlighting discrepancies in delivery performance.
Product Category Insights: Focuses on the performance of key product categories like Dairy, Food, and Beverages, showing the total quantity ordered and delivered.

6. Metrics and KPIs
The following KPIs were measured:

Line Fill Rate (LIFR %): Measures the percentage of order lines fulfilled compared to the total lines ordered.
Volume Fill Rate (VOFR %): Quantifies the percentage of the total volume delivered against the total volume ordered.
On-Time %: Percentage of orders delivered within the expected timeframe.
In-Full %: Percentage of orders where all line items were delivered in full.
OTIF %: A critical metric combining On-Time and In-Full metrics to assess complete and punctual deliveries.

7. Technologies Used
SQL: Used to query and aggregate data from the underlying database, preparing it for analysis.
Python: Employed for data preprocessing, metric calculations, and custom logic implementation.
Power BI: Visualization tool used to create dynamic dashboards showcasing trends and insights in supply chain performance.
Microsoft Excel: May be used for initial data validation and cleaning before feeding into Power BI.

8. Instructions to Run
SQL
Run the provided SQL query (SQLQuery1.sql) in your preferred SQL environment to extract the raw data needed for analysis.
Export the results as a CSV file or feed it directly into Python for further processing.
Python
Install the required libraries (e.g., pandas, numpy, matplotlib, seaborn).
Run the Python script to clean the data and calculate the metrics.
The output will be in the form of a clean CSV file or a direct connection to the Power BI dashboard.
Power BI
Load the cleaned dataset into Power BI.
The dashboard (Supply chain Analysis.pbix) is pre-configured with the metrics and visuals needed.
Review and analyze the insights on the dashboard to monitor supply chain performance.

9. Future Enhancements
Real-time Data Integration: Introduce real-time data pipelines for immediate monitoring of supply chain KPIs.
Machine Learning for Predictions: Implement predictive analytics to forecast future OTIF performance based on historical trends.
Interactive Reporting: Enable more dynamic reporting capabilities with filters for different time frames and geographies.
Automation: Automate the entire data extraction, processing, and dashboard update pipeline for continuous monitoring.
