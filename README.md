🚀 E-Commerce Sales Analysis — Power BI Dashboard

Analyzed 34,500+ e-commerce transactions to uncover revenue trends, product performance, customer behavior, return rates, and operational efficiency.
Final deliverable: a 2-page interactive Power BI report with KPIs, breakdown visuals, DAX measures, and exploratory insights.

📌 Table of Contents

--Project Overview

--Dashboard Pages

--Features

--Dataset

--Data Cleaning & Preparation

--DAX Measures

--Key Insights

--Recommendations

--Repository Structure

--Tools Used

--How to Use This Project

--License

📊 Project Overview

This project explores the sales and operational performance of an e-commerce business.
The dashboard helps answer questions like:

-How are revenue and orders trending over time?

-Which categories and regions generate the most profit?

-What customer demographics drive sales?

-Which products have the highest return rate and why?

-Do delivery delays influence returns?

-The report is designed for data analysts, business managers, and stakeholders who want quick, actionable insights.

📈 Dashboard Pages
1️⃣ KPI Summary Page

Visual summary of key business metrics such as:

-Total Revenue

-Total Profit

-Total Orders

-Return Rate

-Profit Margin %

-Avg Delivery Days

-Revenue per Customer

-Monthly Revenue

🔍 Preview

2️⃣ Sales Overview Dashboard

Interactive visuals to explore:

-Revenue Over Time

-Orders Over Time

-Revenue by Category

-Revenue by Region

-Revenue by Customer Age

-Return Rate by Category

-Detailed Transaction Table

🔍 Preview

🧩 Features

✔ Interactive slicers (Month, Category, Region)
✔ 10+ custom DAX measures
✔ Clean, professional UI
✔ Drill-down ready visuals
✔ Fully documented folder structure
✔ End-to-end analysis workflow

📂 Dataset

Rows: 34,500+

Columns: Customer details, product info, pricing, discounts, orders, profit, delivery time, return flags

Time Range: Jan 2024 – Aug 2025

Dataset includes:

Order ID

Customer ID

Category

Region

Price, Quantity, Discount

Revenue, Profit

Delivery Days

Returned Flag

Customer Age & Gender

You can find the dataset in:

/dataset.xlsx

🧹 Data Cleaning & Preparation

1)Performed using SQL + Power BI:

2)Removed invalid rows (missing IDs, negative quantity)

3)Standardized date formats

4)Created derived columns: revenue, order_month, returned_flag

5)Normalized discount values

6)Validated totals between SQL & Power BI

7)Created delivery performance groups

🧮 DAX Measures

Below are some of the main DAX measures used:

1)Total Revenue = SUM(ecommerce_sales[revenue])

2)Total Profit = SUM(ecommerce_sales[profit])

3)Total Orders = COUNT(ecommerce_sales[order_id])

5)AOV = DIVIDE([Total Revenue], [Total Orders])

6)Return Rate =
DIVIDE(
    SUM(ecommerce_sales[returned_flag]),
    [Total Orders]
)

7)Profit Margin % = DIVIDE([Total Profit], [Total Revenue])

8)Avg Delivery Days = AVERAGE(ecommerce_sales[delivery_time_days])


Full DAX collection is stored in:

/DAX/

🔍 Key Insights

✔ Revenue shows strong month-on-month growth, especially during sales periods.
✔ Home & Electronics dominate sales, consistently the top-earning categories.
✔ South & North regions lead in revenue, while Central shows opportunity for growth.
✔ Fashion and Electronics have the highest return rates, indicating quality/sizing issues.
✔ Customers aged 25–45 generate the most revenue.
✔ Delivery delays increase return probability, showing operational bottlenecks.

💡 Recommendations

Improve delivery speed in slower regions to reduce return rates.

Investigate high-return categories (Fashion, Electronics).

Increase marketing spend in Home & Electronics; strongest performance.

Strengthen Central region presence; large untapped potential.

Target mid-age customers (25–45) with tailored promotions.

🗂 Repository Structure
Ecommerce-Sales-Analysis/
│── README.md
│── Ecommerce Sales.pbix
│── dataset.xlsx
│
├── images/
│     ├── Ecommerce Dashboard.png
│     └── Ecommerce KPIs.png
│
└── DAX/
      ├── TotalRevenue.dax
      ├── TotalProfit.dax
      ├── TotalOrders.dax
      ├── AOV.dax
      ├── ReturnRate.dax
      ├── ProfitMarginPercent.dax
      ├── RevenuePerCustomer.dax
      ├── AvgDeliveryDays.dax
      └── MonthlyRevenue.dax

🛠 Tools Used

=Power BI Desktop

=SQL

=Excel

=DAX

=GitHub

=Power Query

▶ How to Use This Project

Download the repo or clone using:

git clone https://github.com/navamgupta2251-hash/Ecommerce-Sales-Analysis


Open Ecommerce Sales.pbix in Power BI Desktop.

Explore dashboards using slicers.

Review DAX formulas inside /DAX/.

View screenshots inside /images/.

📄 License

This project is available under the MIT License.
You may use the dashboard, code, and insights for learning or portfolio purposes.
