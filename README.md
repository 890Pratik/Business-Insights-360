# Business-Insights-360

## Project Overview

AtliQ Hardware is growing rapidly in the recent years, and they have decided to implement Data Analytics using Power BI in their company for the first time to surpass their competitors in the market and to make data driven decisions. This project is hoped to give answers to the questions of stakeholders in terms of all aspects like Finance, Sales, Marketing and Supply Chain

Live Project Link - 
https://app.powerbi.com/view?r=eyJrIjoiOWI0MjkyYzktNjNhYy00YWFlLWI1YTktYTc2NDBkNDU3ZWU5IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9
# Tech Stacks

- SQL
- Power BI Desktop
- Excel
- DAX language
- DAX Studio (for optimizing the report)
- Project charter file

# Power BI Technique

- What all questions should be asked before staring the Project
- Creating calculated columns
- creating measures using DAX language
- Data modeling
- Using Bookmarks to switch between visuals
- Page navigation with buttons
- Using divide function to prevent zero division errors
- creating date table using m language
- Dynamic titles based on the applied filters
- Using KPI indicators
- Conditional formatting the values in visuals using icons or background color
- Data validation techniques
- Power BI Services
- Publishing reports to Power BI Services
- Setting up Personal Gateway to set up the auto refresh of data
- Power BI App creation
- Collaboration, workspace, access permissions in Power BI Services

# Business Related Terms

- Gross Price
- Pre-Invoice Deductions
- Post-Invoice Deductions
- Net Invoice Sale
- Gross Margin
- Net Sales
- Net Profit
- COGS - Cost Of Goods Sold
- YTD - Year to Date
- YTG - Year to Go
- Direct
- Retailer
- Distributors
- Consumer


# Dataset Understanding

- gdb041:
- dim_customer
    - 27 distinct markets (ex India, USA, Spain)
    - 75 distinct customers thorough out the market
    - 2 types of platforms
      - Brick & Motors - Physical/offline store
      - E-commerce - Online Store (Amazon, flipkart)
    - Three channels
      - Retailer
      - Direct
      - Distributors
  - dim_market
      - 27 distinct markets (ex India, USA, spain)
      - 7 sub-zones
      - 4 regions
          - APAC
          - EU
          - NA
          - LATAM
- dim_product
    - Divisions
       - P & A
         - Peripherals
         - Accessories
       - PC
         - Notebook
         - Desktop
      - N & S
        - Networking
        - Storage
- There are 14 different categories, Like Internal HDD, Keyboard
- There are different variants available for the same product
- fact_forecast_monthly
    This table is used to forecast the customer’s need in advance, which can help in
         Higher customer satisfaction
          Reduced cost in warehouses for storage purpose
- The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
- All the date of the month will be replaced by the start date of the month
- It will have all the column names and in the end it will have the forecast quantity need of the customer
- fact_sales_monthly
    This table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value.
_ gdb056
- freight_cost
    This table has details of travel cost and other cost for each market with fiscal year
- gross_price
    Has the details of gross prices with product code
- manufacturing_cost
    Has the details of manufacturing cost with product code and year
- Pre_invoice_dedutions
    Has the details of pre invoice deductions percentage for each cutomer and year
- Post_invoice_deductions
    Post invoice deductions and other deductions details
