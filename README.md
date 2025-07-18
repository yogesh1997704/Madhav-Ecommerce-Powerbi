                                      ## Madhav Ecommerce Sales Dashboard (Power BI)##


## 📌 Project Overview
This is an interactive *Power BI Dashboard* built to analyze ecommerce sales data.  
The dashboard provides insights on:
- Sales by State
- Profit trends by Month
- Quantity & Amount by Category and Sub-Category
- Top Customers
- Payment Mode Distribution

---

## 🗂 Dataset Details
Files included in this repository:
| File | Description |
|------|-------------|
| data/Orders.csv | Order-level data (Order ID, Customer Name, State, Category, Payment Mode, Amount) |
| data/Details.csv | Additional details like Profit, Quantity, Discount |
| Madhav_Ecommerce_Sales_Dashboard.pbix | Power BI Report file |
| images/dashboard_screenshot.jpg | Dashboard Preview |

---

## 🔍 Key KPIs in Dashboard
- *Total Sales:* 438K  
- *Total Profit:* 37K  
- *Total Quantity:* 5615  
- *Avg Order Value (AOV):* 121K  

---

## 🛠 Data Transformation (Power Query)
- Loaded Orders.csv and Details.csv
- Fixed data types
- Created relationships: Order ID key
- Created calculated columns for Month, Year
- Removed null values

---

## 📊 Visuals Used
- KPI Cards (Sales, Profit, Quantity, AOV)
- Bar Chart: Sales by State
- Line/Bar Chart: Profit by Month
- Donut Chart: Payment Mode share
- Donut Chart: Category-wise distribution
- Bar Chart: Sub-Category Quantity

---

## 🧮 DAX Measures
```DAX
Total Amount = SUM(Orders[Amount])
Total Profit = SUM(Details[Profit])
Total Quantity = SUM(Details[Quantity])
Avg Order Value = DIVIDE([Total Amount], DISTINCTCOUNT(Orders[Order ID]))
# Madhav Ecommerce Sales Dashboard (Power BI)
---

## ![Dashboard Screenshot](images/dashboard_screenshot.jpg)
