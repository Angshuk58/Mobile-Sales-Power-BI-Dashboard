# Power BI Dashboard for Mobile Sales Dataset 📊📱

Welcome to my Power BI dashboard project, where I've created an interactive dashboard to visualize and analyze mobile sales data. This project utilizes **DAX (Data Analysis Expressions)** to calculate various metrics, including **MTD (Month-to-Date)** values, and offers insights into mobile sales trends, performance, and KPIs.

## 📌 Project Overview

This Power BI dashboard is built on a mobile sales dataset and demonstrates how to use **DAX** formulas to create dynamic and insightful calculations. The dashboard focuses on the following metrics:

- **Total Sales**: Summing up the sales for the selected period.
- **MTD Sales**: Calculating the sales for the current month up until the selected date.
- **Sales Trends**: Displaying sales performance over time.
- **Top Performing Products**: Ranking products based on sales volume.
- **Sales by Region/Models**: Breakdown of sales across different regions and categories.

## 🔧 Technologies Used

- **Power BI**: For building the interactive dashboard.
- **DAX (Data Analysis Expressions)**: For creating calculated columns, measures, and performing complex calculations.
- **Mobile Sales Dataset**: The dataset used for this dashboard, containing data on sales transactions, product details, regions, and time periods.
- **MTD Calculation**: Using DAX to calculate sales month-to-date for dynamic reporting.

## 📊 Key Features

- **MTD Calculation**: The Month-to-Date sales calculation is performed using DAX formulas to aggregate sales for the current month based on the selected date.
- **Interactive Filters**: The dashboard includes slicers for filtering by product, region, and date to allow deeper insights into the data.
- **Trend Analysis**: Dynamic visuals show the sales trends over time, including daily, weekly, and monthly aggregations.
- **Top Products**: The dashboard ranks the best-selling products based on the total sales and displays them in an interactive table.

## ⚙️ How to Use

To explore the Power BI dashboard:

1. **Clone or Download** this repository to your local machine.
2. Open the `.pbix` file in **Power BI Desktop**.
3. Refresh the data model (if necessary) to ensure the latest data is loaded.
4. Use the slicers (filters) on the dashboard to analyze sales by **region**, **product**, and **time period**.
5. Explore the **MTD** metrics that calculate the current month's performance based on the selected date.

## 🧠 DAX Formulas

Key DAX expressions used in this project:

- **MTD Sales Calculation**:
    ```DAX
    MTD_Sales = 
    CALCULATE(
        SUM(Sales[SalesAmount]),
        DATESMTD(Sales[Date])
    )
    ```

- **Total Sales**:
    ```DAX
    Total_Sales = 
    SUM(Sales[SalesAmount])
    ```

These DAX formulas power the core calculations behind the dashboard, ensuring that all metrics are accurate and dynamic.
