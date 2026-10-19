# Online Retail Data Analytics Project

## 1. Project Overview
This project analyzes an Online Retail dataset to understand sales performance, product demand, customer purchasing activity, and trends over time. Python is used for data cleaning, exploratory data analysis (EDA), and visualization. Power BI is used to build an interactive dashboard.

## 2. Problem Statement
Retail businesses need to understand which products and markets contribute most to sales, how sales change over time, and where opportunities for improvement exist. This project explores retail transaction data to identify useful patterns and support data-driven decisions.

## 3. Dataset Description
- **Dataset:** Online Retail
- **Source:** UCI Machine Learning Repository
- **File used:** `online_retail_clean.csv`
- **Main fields:** InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country, and Sales.
- **Sales calculation:** `Sales = Quantity × UnitPrice`

The original dataset contains retail transaction records. The cleaned file is used for analysis and dashboard creation.

## 4. Tools Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Power BI Desktop
- Git and GitHub
- VS Code

## 5. Data Cleaning Process
The dataset was inspected for missing values, data types, and duplicate records. Duplicate rows were removed. Rows missing essential fields such as product description or invoice date were removed. Records with non-positive quantity or unit price were excluded for the sales analysis. Missing `CustomerID` values were retained because the actual IDs were not available. A `Sales` column was calculated as quantity multiplied by unit price.

## 6. Exploratory Data Analysis (EDA)
The analysis included:
- Dataset shape, column names, data types, and missing-value checks.
- Descriptive statistics for Quantity, UnitPrice, and Sales.
- Correlation analysis for numerical fields.
- Sales aggregation by country and month.
- Potential outlier detection using the Interquartile Range (IQR) method.

## 7. Visualizations
Charts created for the project include:
1. Top countries by total sales.
2. Monthly sales trend.
3. Distribution of unit prices.
4. Quantity versus unit price scatter plot.
5. Sales by day of the week.
6. Correlation heatmap.

Chart files are saved in the `outputs/` folder. Update this list if your final filenames differ.

## 8. Power BI Dashboard
The interactive dashboard includes three KPI cards:
- Total Sales
- Total Quantity
- Total Invoices

It also includes visualizations for sales by country, monthly sales trend, top products by sales, and sales by weekday. Country and date slicers allow users to filter the dashboard. The Power BI report is saved as `Online_Retail_Dashboard.pbix` if included in the repository.

## 9. Key Insights
Use the actual values from your charts/dashboard to complete these points before submission:
- **Highest-sales country:** [Enter country and value from dashboard]
- **Lowest-sales country:** [Enter country and value from dashboard]
- **Best-performing month:** [Enter month and value from dashboard]
- **Top-selling product:** [Enter product and value from dashboard]
- **Weekday pattern:** [Enter the highest/lowest sales weekday from dashboard]

Do not submit the bracketed placeholders. Replace them with findings from your actual results.

## 10. Business Recommendations
1. **Improve inventory planning:** Monitor top-selling products and maintain appropriate stock levels to reduce stockouts.
2. **Review low-performing markets:** Investigate countries with lower sales and test targeted promotions where commercially appropriate.
3. **Plan promotions using trends:** Use monthly and weekday sales patterns to test promotions during slower periods and compare results.

Recommendations should be reviewed against the actual dashboard results.

## 11. Conclusion
This project demonstrates how Python and Power BI can be used to clean, analyze, visualize, and communicate retail transaction data. The analysis supports a better understanding of sales patterns and provides a foundation for inventory planning, market evaluation, and business decision-making.

## Project Structure
```text
Online-Retail-Data-Analytics/
├── Data/
│   ├── Online Retail.xlsx
│   └── online_retail_clean.csv
├── Scripts/
│   ├── task3.py
│   ├── task4.py
│   └── task5.py
├── outputs/
│   ├── chart1_country_sales.png
│   ├── chart2_monthly_sales.png
│   ├── chart3_unit_price_distribution.png
│   ├── chart4_quantity_vs_price.png
│   ├── chart5_sales_by_weekday.png
│   ├── chart6_correlation_heatmap.png
│   └── descriptive_statistics.csv
├── Online_Retail_Dashboard.pbix
└── README.md
```

Only list files that actually exist in your repository. Avoid uploading sensitive information or unnecessary large files.
