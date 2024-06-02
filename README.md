# Online-store-dashboard

Objective :
Using Power BI to create a comprehensive dashboard for our simple online store customer data, empowering stakeholders with real-time insights to optimize marketing strategies, improve customer experiences, and drive business growth.

Steps
1. Extracting raw data
2. Setting up the dashboard
3. Importing data in Power BI
4. Data Cleaning and Processing
5. Determining the dashboard KPIs
6. Finally adding the charts

DAX

AgeGroup = SWITCH(
     TRUE(),
     'online_store_customer_data'[Age]<30, "15-20",
     'online_store_customer_data'[Age]>=30 && 'online_store_customer_data'[Age]<40, "30-40",
     'online_store_customer_data'[Age]>=40 && 'online_store_customer_data'[Age]<50, "40-50",
     'online_store_customer_data'[Age]>=50 && 'online_store_customer_data'[Age]<60, "50-60",
     'online_store_customer_data'[Age]>=60 , "60+",
     "unknown"
)
