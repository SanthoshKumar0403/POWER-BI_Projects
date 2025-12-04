# 🛍️ E-commerce Sales Performance Analysis (Power BI)

## 🎯 Project Objective

To conduct an end-to-end **E-commerce Sales Analysis** using Business Intelligence (BI) tools to provide management with a clear, interactive overview of sales performance, profitability, and customer buying trends. The final deliverable is an actionable dashboard that supports strategic decisions in areas like inventory, marketing, and sales operations.

---

## 🛠️ Tools & Methodology

This project demonstrates proficiency in the full data analysis lifecycle, from raw data integration to final dashboard publication.

* **Tools:** **Power BI Desktop**, **SQL/Excel CSV Files** (as data sources), **DAX** (Data Analysis Expressions).
* **Methodology:**
    1.  **Data Integration:** Merged data from two separate CSV sources based on a common key.
    2.  **Data Cleaning & Transformation:** Used Power Query (M Language) to clean and transform columns, including handling date formats and calculating derived columns.
    3.  **Data Modeling:** Established a **Star Schema** to define efficient relationships between the fact (Details) and dimension (Orders) tables.
    4.  **DAX Calculation:** Created key performance indicators (KPIs) and complex metrics (e.g., Year-over-Year Sales, Profit Margin).
    5.  **Visualization:** Designed an interactive, executive-level dashboard focusing on clarity and actionability.

---

## 🏗️ Data Model (Star Schema)

The analysis relies on a robust data model built by integrating two separate datasets via a one-to-many relationship (`1:*`) on the shared key, **`Order ID`**.

| Table Type | File Name | Key Metrics/Columns | Role in Model |
| :--- | :--- | :--- | :--- |
| **Fact Table** | `Details_Daset.csv` | `Amount`, `Profit`, `Quantity`, `Category`, `PaymentMode` | Contains quantifiable, event-level data (Sales facts). |
| **Dimension Table** | `Orders _Dataset.csv` | `Order Date`, `CustomerName`, `State`, `City` | Contains descriptive, categorical data (Who, Where, When). |



---

## 📈 Key Insights & Business Recommendations

The final Power BI dashboard provides immediate insights into performance drivers, enabling focused strategic actions:

| Insight Area | Key Finding Demonstrated | Actionable Recommendation |
| :--- | :--- | :--- |
| **Profitability** | Products like **Bookcases** and **Tables** were high-revenue, but certain **Clothing** sub-categories showed negative profit margins. | **Optimize Inventory:** Re-evaluate pricing or supplier costs for low-profit/loss-making categories to immediately boost the bottom line. |
| **Geographic Performance** | Identified the top 3 high-volume states (e.g., **Maharashtra, UP, MP**) and the lowest performers. | **Target Marketing:** Allocate advertising budget to underperforming states with high potential; reward top-performing regional teams. |
| **Customer Behavior** | Revealed the most popular **Payment Modes** and **Product Categories** by volume. | **Optimize Checkout:** Prioritize and streamline the most popular payment gateway (e.g., UPI, Credit Card) for a smoother customer experience. |
| **Time-Based Trends** | Identified peak sales months (e.g., Festival Season) and seasonal demand fluctuations. | **Strategic Stocking:** Use trend data to ensure timely stocking and distribution of high-demand items ahead of peak periods. |

---

## 📁 Repository Deliverables

| File Name | Description |
| :--- | :--- |
| **`E-COMMERCE SALES ANALYSIS.pbix`** | The complete, final Power BI dashboard file. Contains the data model, all DAX measures, and interactive visualizations. |
| **`Details_Daset.csv`** | Raw data file containing transaction and product details (Fact Table). |
| **`Orders _Dataset.csv`** | Raw data file containing order and customer information (Dimension Table). |
| **`README.md`** | This summary document for quick project assessment. |
