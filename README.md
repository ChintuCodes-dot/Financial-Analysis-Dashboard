📊 Financial Analysis Dashboard – Power BI

An interactive Power BI dashboard designed to analyze **sales, revenue, gross profit, profit margin, discount impact, business performance, product performance, and geographical performance**. The dashboard provides dynamic **YTD, QTD, and MTD analysis** to help users understand financial performance across different periods and business dimensions.

📌 Project Overview

The **Financial Analysis Dashboard** is an interactive Power BI business intelligence project developed to provide a comprehensive view of financial and sales performance.

The dashboard allows users to analyze key financial metrics such as **Gross Profit, Net Sales, Profit Margin %, and Revenue %** using dynamic time-period selections.

The report is structured into three analytical pages:

1. 🏠 **Summary**
2. 📍 **Profit / Location Analysis**
3. 📦 **Product / Location Analysis**

The dashboard uses interactive slicers and dynamic calculations to allow users to analyze performance based on **Year, Quarter, Month, Segment, Business, Country, City, Category, Product, and Sub-Product**.



# 🎯 Business Problem

Businesses generate large amounts of sales and financial data, but analyzing overall profitability and revenue performance across different dimensions can be difficult using raw data.

Management needs answers to questions such as:

* How much net sales and gross profit were generated?
* What is the overall profit margin?
* Which discount bands generate better margins?
* Which customer segments contribute most to revenue and profitability?
* Which businesses are performing better?
* Which countries and cities generate the highest profit?
* Which products and categories contribute most to sales?
* How does financial performance change between YTD, QTD, and MTD periods?

The dashboard addresses these questions through an interactive financial analysis report.


# 🎯 Goal of the Dashboard

The primary objective is to create an interactive financial analysis tool that:

* Monitors key financial KPIs.
* Analyzes gross profit and net sales.
* Measures profit margin percentage.
* Evaluates revenue contribution.
* Compares performance across discount bands.
* Analyzes segment and business performance.
* Provides country and city-level analysis.
* Provides category, product, and sub-product analysis.
* Supports YTD, QTD, and MTD financial analysis.
* Enables users to explore financial performance through interactive slicers.

# 🛠️ Tech Stack

The dashboard was developed using:

* 📊 **Power BI Desktop** – Main platform used for dashboard development and visualization.
* 📂 **Power Query** – Used for data cleaning, transformation, and preparation.
* 🧠 **DAX** – Used to create financial measures, ratios, time-based calculations, and dynamic analysis.
* 🗂️ **Data Modeling** – Used to structure the data model and enable interactive filtering.
* 📈 **Power BI Visualizations** – Used for KPI cards, charts, slicers, and matrix-based analysis.
* 📁 **File Format** – `.pbix` for Power BI development and `.png` for dashboard previews.



# 📂 Data & Financial Logic

The dashboard follows a structured financial calculation framework.

### Gross Sales


Gross Sales = Units Sold × Sale Price

### Net Sales


Net Sales = Gross Sales − Discounts

### Gross Profit


Gross Profit = Net Sales − COGS


### Profit Margin %


Profit Margin % = Gross Profit / Net Sales

The denominator for Profit Margin % is calculated based on the overall value corresponding to the current slicer selection.

### Revenue %


Rev % = Net Sales / Overall Net Sales


The overall Net Sales denominator is dynamically determined based on the selected analysis period.

These formulas form the core financial logic of the dashboard.



# ⭐ Dashboard Features

## 1. 🏠 Summary Page

The Summary page provides a high-level overview of financial performance.

### Key KPIs

The dashboard tracks:

* 💰 **Gross Profit**
* 📊 **Profit Margin %**
* 💵 **Net Sales**
* 📈 **Revenue %**

These KPIs provide a quick overview of the financial position for the selected period.

### YTD / QTD / MTD Analysis

An interactive period selection allows users to switch between:

* **YTD – Year-to-Date**
* **QTD – Quarter-to-Date**
* **MTD – Month-to-Date**

The report dynamically updates based on the selected period.

### Date Slicer

A hierarchical date slicer allows users to select:

* Year
* Quarter
* Month

This selection drives the financial analysis throughout the report.



# 📊 2. Profit / Location Analysis

This page focuses on understanding profitability and revenue contribution across different business dimensions.

## Profit Margin % by Discount Band

A column chart analyzes **Profit Margin % across different discount bands**.

This helps identify how discount levels affect profitability.

## Profit Margin % by Segment

A pie chart compares **Profit Margin % across customer/business segments**.

This helps identify segments with stronger profitability.

## Profit Margin % by Business

A donut chart compares **Profit Margin % across different businesses**.

This provides a quick view of profitability distribution across business areas.

## Revenue % by Discount Band

A column chart displays **Revenue % by discount band**, helping understand how much of the overall net sales is contributed by each discount category.

## Revenue % by Segment

A pie chart shows the **revenue contribution of different segments**.

## Revenue % by Business

A donut chart displays **revenue contribution across businesses**.

These visuals enable users to compare profitability and revenue contribution from multiple perspectives.



# 🌎 3. Product / Location Analysis

The Product / Location Analysis page provides detailed geographical and product-level analysis.

## 📍 Location Analysis

A matrix visual provides detailed analysis by:

* Country
* City

The values include:

* Gross Profit
* Net Sales
* Profit Margin %
* Revenue %

This allows users to drill down from country-level performance to individual cities.

## 📦 Product Analysis

A second matrix provides hierarchical product analysis using:

* Category
* Product
* Sub-Product

The analysis includes:

* Gross Profit
* Net Sales
* Profit Margin %
* Revenue %

This enables users to understand financial performance from category level down to individual sub-products.



# 🎛️ Interactive Filters

The dashboard provides interactive filtering capabilities.

### Date Filter

Users can select the required:

* Year
* Quarter
* Month

### Segment Filter

Allows users to analyze financial performance for a specific segment.

### Business Filter

Allows users to analyze individual business areas.

The selected filters dynamically affect the dashboard's financial calculations and visualizations.



# 📅 YTD / QTD / MTD Logic

One of the main analytical features of the dashboard is dynamic period-based analysis.

For example, if **May 2014** is selected:

### YTD

The denominator represents **Net Sales from January 2014 through May 2014**.

### QTD

The denominator represents **Net Sales for Q2 of 2014**, covering April and May based on the selected month.

### MTD

The denominator represents **Net Sales for May 2014 only**.

This ensures that Profit Margin % and Revenue % are calculated relative to the appropriate overall period rather than simply the currently displayed row or category.



# 🧠 DAX & Analytical Logic

DAX is used to implement the financial calculations and dynamic period analysis required by the dashboard.

Key analytical calculations include:

* Gross Sales
* Net Sales
* Gross Profit
* Profit Margin %
* Revenue %
* YTD Analysis
* QTD Analysis
* MTD Analysis
* Dynamic denominator calculations
* Filter-dependent financial metrics

The calculations are designed to respond dynamically to the user's slicer selections.



# 🔄 Data Analysis Workflow

The project follows a structured Power BI development workflow:

### 1. Data Preparation

Raw financial and sales data is prepared for analysis.

### 2. Data Cleaning

Power Query is used to clean and transform the data.

Typical preparation includes:

* Removing unnecessary data
* Correcting data types
* Handling missing values
* Standardizing fields
* Preparing analytical columns

### 3. Data Modeling

The cleaned data is structured into an analytical model suitable for Power BI reporting.

### 4. Financial Calculations

DAX measures are created for:

* Sales
* Profit
* Profit Margin
* Revenue %
* Time-period analysis

### 5. Dashboard Development

Interactive visuals, slicers, KPI cards, and matrix visuals are designed according to the dashboard framework.

### 6. Analysis

The final dashboard is used to analyze financial performance across time, location, business, segment, category, product, and sub-product.



# 💡 Key Business Questions Answered

The dashboard helps answer questions such as:

* What is the current gross profit?
* What is the overall profit margin?
* What is the total net sales?
* How much revenue does each segment contribute?
* Which discount bands generate higher profit margins?
* Which businesses contribute most to revenue?
* Which countries and cities generate the highest profit?
* Which categories and products generate the highest sales?
* How does profitability change between YTD, QTD, and MTD?
* What percentage of total revenue is contributed by a particular segment, business, product, or location?



# 📈 Business Impact

### 💰 Financial Performance Monitoring

Provides management with a centralized view of important financial KPIs.

### 📊 Profitability Analysis

Helps identify differences in profit margins across discount bands, segments, businesses, products, and locations.

### 🌎 Geographic Analysis

Enables comparison of financial performance across countries and cities.

### 📦 Product Performance

Helps identify categories, products, and sub-products contributing to sales and profitability.

### 🎯 Revenue Contribution

Shows how individual segments, businesses, discount bands, locations, and products contribute to overall net sales.

### 📅 Period-Based Decision Making

YTD, QTD, and MTD analysis allows users to evaluate performance at different time horizons.


# 📷 Dashboard Preview

Add screenshots of the three dashboard pages here.


📊 Summary
📈 Profit / Location Analysis
📦 Product / Location Analysis


Example:

![Summary Dashboard](https://github.com/ChintuCodes-dot/Sales-Analytics-Dashboard/blob/main/Screenshot%202026-09-03%20193742.png)

![Profit Location Analysis](https://github.com/ChintuCodes-dot/Sales-Analytics-Dashboard/blob/main/Screenshot%202026-08-29%20142706.png)

![Product Location Analysis](images/product-location-analysis.png)



# 📁 Project Structure


Financial-Analysis-Dashboard/
│
├── 📊 Financial Analysis Dashboard.pbix
│
├── 📷 images/
│   ├── summary.png
│   ├── profit-location-analysis.png
│   └── product-location-analysis.png
│
├── 📂 dataset/
│   └── financial-analysis-data.csv
│
└── 📄 README.md

# 🚀 How to Use

1. Download or clone this repository.
2. Open the `.pbix` file using **Power BI Desktop**.
3. Refresh the data if the dataset is included.
4. Select a date using the Year / Quarter / Month hierarchy.
5. Choose **YTD, QTD, or MTD** analysis.
6. Use Segment and Business slicers to filter the analysis.
7. Explore the Summary, Profit / Location, and Product / Location pages.
8. Interact with the visuals and matrix tables to analyze detailed performance.


# 📚 Skills Demonstrated

This project demonstrates practical experience in:

* Power BI
* Power Query
* DAX
* Data Cleaning
* Data Transformation
* Data Modeling
* Financial Analysis
* Sales Analysis
* Profitability Analysis
* Revenue Analysis
* Time Intelligence
* KPI Development
* Data Visualization
* Interactive Dashboard Development
* Business Intelligence



# 🔮 Future Improvements

Potential improvements for future versions include:

* 📈 Sales and profit forecasting
* 📊 Year-over-Year growth analysis
* 🎯 Target vs Actual analysis
* 🔍 Drill-through pages
* 📅 Advanced time-intelligence analysis
* 🔮 Predictive analytics
* 📱 Power BI mobile optimization
* ☁️ Deployment through Power BI Service
* 🔄 Automated data refresh



## 👨‍💻 Project Author

**Soumyaranjan**

Data Analyst | Power BI | SQL | Python | Excel

---

⭐ If you found this project useful, consider giving the repository a star.
