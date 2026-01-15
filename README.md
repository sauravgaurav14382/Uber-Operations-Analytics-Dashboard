🚖 Uber Analytics Dashboard – Power BI | SQL | DAX

An end-to-end Business Intelligence project built using Power BI, SQL, and DAX, designed to analyze Uber rides, revenue performance, customer behavior, and operational efficiency.
This project converts raw Uber ride data into interactive dashboards with KPIs, drill-downs, filters, and visual insights.

📌 Project Overview

This dashboard provides a 360° view of Uber’s operations—Bookings, Revenue, Vehicles, Locations, Riders, and Ratings—based on the business requirements document.
It includes multiple pages with filters, slicers, trend patterns, and advanced DAX measures.
Insights are supported by PDF dashboard visuals (Uber_Dashboard_pdf.pdf) 

Uber_Dashboard_pdf

 and requirements (Uber Problems and Business Requirements.docx). 

Uber Problems and Bussiness Req…

🧾 Business Requirements Covered

From the requirement document, the dashboard includes:
✔ KPI Cards – Completed Bookings, Lost Bookings, Revenue, Total Distance, Avg Distance 

Uber Problems and Bussiness Req…


✔ Vehicle Filters & Analysis
✔ Monthly & Quarterly Trends (Bookings & Revenue)
✔ Revenue by Vehicle Type
✔ Top Pickup & Drop Locations
✔ Rider Metrics – Cancellations, Payment Method Trends, First/Return/Regular Riders
✔ Location Intelligence – Busy Areas, Time Slots, Distance Metrics
✔ Show/Hide Filter Panel for clean UI ◆ 

Uber Problems and Bussiness Req…

🧰 Tech Stack
Tool	Purpose
🟨 Power BI	Data modeling, Dashboard creation, DAX measures
🐬 SQL	Data cleaning, preprocessing, transformations
📊 DAX (Data Analysis Expressions)	KPIs, Time intelligence, Custom measures
🧮 Key DAX Measures Used


Total_Revenue = SUM(Ubert[Revenue])

Completed_Bookings = CALCULATE(COUNTROWS(Uber), Uber[Status] = "Completed")

Lost_Bookings = CALCULATE(COUNTROWS(Uber), Uber[Status] = "Cancelled")

Avg_Distance = AVERAGE(Uber[Distance_km])

Monthly_Revenue = TOTALMTD([Total_Revenue], 'Calendar'[Date])

Quarterly_Revenue = TOTALQTD([Total_Revenue], 'Calendar'[Date])


📈 Dashboard Pages Included
1️⃣ Overview Page

Contains Uber’s key operational KPIs:

Completed & Lost Bookings

Revenue

Total & Avg Distance

Monthly + Quarterly Analysis

Revenue by Vehicle Type

Top Pickup & Drop Locations

Avg Rider & Driver Ratings
All points sourced from BRD. 

Uber Problems and Bussiness Req…

2️⃣ Vehicle Page

Shows vehicle-level performance metrics:

Booking Count

Revenue

Contribution %
As defined in the requirements. 

Uber Problems and Bussiness Req…

3️⃣ Revenue Page

Breakdown of revenue by:

Customer

Vehicle type

Payment Methods

Monthly & Quarterly trends
(from the BRD). 

Uber Problems and Bussiness Req…

4️⃣ Rider Page

Includes:

Cancel Rides by Reasons

Payment Method trends

First/Return/Regular Rider segmentation

Monthly & QTR comparisons
All listed in the doc. 

Uber Problems and Bussiness Req…

5️⃣ Location Page

Displays:

Monthly Total Distance

Distance by vehicle

Busy Time Slots ⏰

Busy Areas 📍
Based on requirement content. 

Uber Problems and Bussiness Req…

🧠 Insights Generated 

✨ Peak booking times were observed during evening hours.
✨ Bike and Mini categories contributed the highest trip volume.
✨ Card & UPI payments dominated rider preference.
✨ Certain locations consistently appeared as high-traffic pickups & drops.
✨ Regular riders generated a higher revenue share than first-time customers.

You can adjust these according to actual insights from your dashboard.

🚀 Features

Interactive filters with Show/Hide Panel

Dynamic time intelligence using DAX

Page navigation buttons for smooth UX

Geo-visuals for pickup-drop heatmaps

Rider segmentation logic

Responsive layout optimized for wide screens

📂 Project Folder Structure
📁 Uber_Analytics_Dashboard
│── 📊 PowerBI_Report.pbix
│── 🗂 SQL_Queries.sql
│── 📑 Uber_Dashboard_pdf.pdf
│── 📝 Business_Requirements.docx
│── README.md (this file)

⭐ Why This Project is Great for a Resume?

Demonstrates strong Data Analytics concepts

Shows ability to convert business requirements → BI Dashboard

Uses SQL + Power BI + DAX together

Includes Multi-page professional reporting

Highlights real business KPIs

🔗 How to Run the Project

Import SQL datasets into your SQL database.

Clean/transform data using the provided SQL scripts.

Load data into Power BI.

Add DAX measures & relationships.

Publish dashboard to Power BI Service (optional).
