**ATLIQ Business Insights 360**

This repository serves as my documentation for the AtliQ Hardwares Business Insights 360 - Power BI Project. It was created as a self-learning project for the course: [Get Job Ready: Power BI Data Analytics for All Levels 4.0]([https://codebasics.io/courses/power-bi-data-analysis-with-end-to-end-project](https://codebasics.io/)) by [Codebasics](https://codebasics.io/).

The entire project has been implemented using Microsoft Power BI Desktop 2.140.1476.0 and published on Microsoft Power BI Service.

The project data files have not been uploaded to this repository in compliance with Codebasics Data & Content Distribution Policy.

-----
**Contents:**

Please find the sectional links for the project below:

- [BI 360 Live Report Link](https://app.powerbi.com/view?r=eyJrIjoiN2NjY2U5NzQtZDliOC00ZmI0LWIxZDAtZTY2N2YwNjkxYTI2IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)
- [](https://app.powerbi.com/view?r=eyJrIjoiN2NjY2U5NzQtZDliOC00ZmI0LWIxZDAtZTY2N2YwNjkxYTI2IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9) [Introduction to AtliQ Hardware](#_introduction_to_atliq)
- [Project Objective](#project-objective)
- [Tools used & Methodologies implemented](#tools-used)
- [](#_tools_used:)[About the Dataset](#about-the-dataset)
  - [Data Sources](#data-sources)
  - [Data Integrity](#data-integrity)
- [](#_data_integrity)[Data Model](#data-model)
- [BI 360 Report Overview](#_bi_360_report)
- [](#_bi_360_report)[Conclusion](#conclusion)

[](#_conclusion:)-----

[**Business Insights 360 Live Report Link**](https://app.powerbi.com/view?r=eyJrIjoiN2NjY2U5NzQtZDliOC00ZmI0LWIxZDAtZTY2N2YwNjkxYTI2IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

[](https://app.powerbi.com/view?r=eyJrIjoiN2NjY2U5NzQtZDliOC00ZmI0LWIxZDAtZTY2N2YwNjkxYTI2IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)-----
# <a name="_introduction_to_atliq"></a>**Introduction to AtliQ Hardware:**
**Domain:** Consumer Goods | **Functions:** Finance, Sales, Marketing, Supply Chain and Executive

- AtliQ Hardwares is company that sells computer hardware and peripherals like PC, mouse, printer etc. to clients across the world.
- They have a major B2B business model wherein they sell to stores like Croma, Best Buy, Staples, Flipkart etc. who then sell it to the end users (consumers). These stores are their main customers.
- They sell through 3 channels: Retailer, Direct and Distributor.
- AtliQ Hardwares’s Customers are of two types. Both these Platforms are called Retailer channels.
  - Brick & Mortar Customer: Actual physical stores e.g. Croma, Best Buy
  - E-commerce Customer: Online websites E.g. Amazon, Flipkart
- AtliQ Hardwares also has a minor B2C business model wherein they own stores: AtliQ E-store and AtliQ Exclusive. These are called Direct channels.
- They also have Distributors in some countries with restricted trade. E.g. Neptune
# <a name="_project_objective:"></a>**Project Objective:**
AltiQ Hardware, a global leader in computers and accessories, faced unexpected losses after opening a store in America. These setbacks were identified to be caused due to reliance on outdated methods such as Excel for data analysis. To address this issue, the company's leadership recognized the need for a transformative approach to leveraging data for informed decision-making. With competitors boasting robust analytics teams, AltiQ Hardware recognizes the urgent need to develop its analytics capabilities using Power BI to thrive in the industry.

To outshine competitors, they've adopted Power BI for analytics with 1.8 million transaction records from Excel, CSV, and MySQL. The Power BI Dashboard includes:

- Home Page: Central navigation for Dashboard.
- Finance: Enhances financial planning.
- Sales: Boosts revenue and market share.
- Marketing: Elevates brand visibility.
- Supply Chain: Optimizes inventory management.
- Executive: Provides top management overview.
# <a name="_tools_used:"></a>**Tools used:**
1. Microsoft Power BI: for Data ETL, Data Modelling, Data Visualization & Dashboarding
1. GitHub - for Documentation

**Skills & Methodologies implemented:**

1. Data Cleaning: **Power Query**
1. Data Manipulation: **DAX Measures & Columns, Numeric & Field Parameters**
1. Data Modelling
1. Data Visualization: **Conditional Formatting, Custom Tooltip**
1. Dashboarding: **Filters, Custom Icon Buttons, Slicers, Bookmarks, Page Navigation**
1. Report Publishing: **PBI Service and Report Optimization**
1. Documentation
-----
# <a name="_about_the_dataset:"></a>[**About the Dataset:**](#_about_the_dataset:)
# <a name="_data_sources:"></a>**Data Sources:**
The dataset contains 11 tables in total, namely:

- From gdb041 MySQL Server:
  - dim\_customer: 209 records | 5 columns
  - dim\_market: 27 records | 3 columns
  - dim\_product: 397 records | 6 columns
  - fact\_forecast\_monthly: 1,885,941 records | 4 columns
  - fact\_sales\_monthly: 1,885,941 records | 4 columns
- From gdb041 MySQL Server:
  - freight\_cost: 135 records | 4 columns
  - manufacturing\_cost: 1,197 records | 3 columns
  - post\_invoice\_deductions: 2,063,076 records | 5 columns
- Excel Files:
  - market\_share: 737 records | 6 columns
  - operational\_expense: 113 records | 4 columns
  - ns\_gm\_target: 321 records | 5 columns
# <a name="_data_integrity:"></a>**Data Integrity:**
ROCCC Evaluation:

- Reliability: MED - The raw dataset is created and updated by Codebasics. It has total 9 files. All of them were utilized in the analysis.
- Originality: HIGH - First party provider (Codebasics)
- Comprehensiveness: HIGH - Total 11 Files with a total of around 5.8 Million records were provided. Dataset contains multiple dimension parameters for Customers & Products as well as comprehensive sales transaction data.
- Current: MED - Dataset was updated upto FY 2022 i.e almost 2 years old. So its not very relevant. Any trends observed and insights gained need to be comprehended as a general (not FY-specific) trend.
- Citation: HIGH - Official citation/reference available.
-----
# <a name="_data_model:"></a>**Data Model:**
![Data Model](https://raw.githubusercontent.com/naveensurla/Business-Insights-360/main/Data%20Model/Data_Model/DM-1.png)
![Data Model](https://raw.githubusercontent.com/naveensurla/Business-Insights-360/main/Data%20Model/Data_Model/DM-2.png)
![Data Model](https://raw.githubusercontent.com/naveensurla/Business-Insights-360/main/Data%20Model/Data_Model/DM-3.png)

-----
# <a name="_project_implementation:"></a><a name="_bi_360_report"></a>**BI 360 Report Overview:**
**I. Home View:**

Central navigation hub with easy access to all views, complete with support and information manual.

![Home Page](https://raw.githubusercontent.com/naveensurla/Business-Insights-360/main/Report_Details/1.Home%20Page.jpg)

**II. Finance View:**

Enhances financial planning and cost control, featuring a P&L Statement, Net Sales Trend and Breakdown by Products/Customers and more.

![Finance Page](https://raw.githubusercontent.com/naveensurla/Business-Insights-360/main/Report_Details/2.Finance%20Page.jpg)


**III. Sales View:**

Focuses on boosting sales revenue and tracking customer performance, including Gross Margin % Variance across Customers/Products and more.

![Sales Page](https://raw.githubusercontent.com/naveensurla/Business-Insights-360/main/Report_Details/3.Sales%20Page.jpg)


**IV. Marketing View:**

Elevates brand visibility and evaluates marketing campaign ROI, with insights into Segment Performance, Net Profit % Variance across Regions and more.

![Marketing Page](https://raw.githubusercontent.com/naveensurla/Business-Insights-360/main/Report_Details/4.Marketing%20Page.jpg)


**V. Supply Chain View:**

Optimizes inventory management and demand forecasting, featuring trends in Forecast Accuracy and Inventory Stock Risk by Customers/Products.

![Supply Chain Page](https://raw.githubusercontent.com/naveensurla/Business-Insights-360/main/Report_Details/5.Supply%20Chain%20Page.jpg)


**VI. Executive View:**

Provides a high-level overview of organizational performance for top AtliQ executives and senior management, showcasing business KPIs, Revenue Contributions by Division/Channel, Top Customers & Products, AtliQ's Market Share Trend and more.

![Executive Page](https://raw.githubusercontent.com/naveensurla/Business-Insights-360/main/Report_Details/6.Executive%20Page.jpg)


-----
# <a name="_conclusion:"></a>**Conclusion:**
The Power BI Report project for AtliQ Hardware provided a comprehensive, data-driven analysis across five critical business functions: Finance, Sales, Marketing, Supply Chain, and Executive. By integrating key business metrics such as Net Sales, Gross Margin, COGS, Net Profit % and Forecast Accuracy % the dashboard offers a holistic view of AtliQ's performance.

The insights gained from this analysis revealed areas of interest, such as robust sales performance and precise forecast accuracy, as well as areas of opportunities for improvement in weak profit margins and supply chain efficiency. Through interactive visualizations and detailed metrics, the dashboard empowers Atliq Hardware's leadership to make informed, strategic decisions that align with their business goals.

## 🔗 PBIX File Download  
[📂 Download the PBIX File](https://drive.google.com/file/d/106LaFsynHQkziELXobbD7F4dHiY7YvA8/view?usp=drive_link)
