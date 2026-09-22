# 💻 ITSM Service Desk & Ticket Operations

This project is based on IT Service Management (ITSM) data and focuses on understanding service desk tickets, SLA performance and customer satisfaction.

I worked on this project using PostgreSQL and Python, with the analysis carried out in Jupyter Notebook. I also created a Power BI dashboard to present the main findings in an interactive way.

The main goal was to take the available ticket and SLA data, prepare it properly, explore it through different types of analysis, and understand what the data was telling us about service performance.

---

## 📌 Project Overview

The dataset represents an IT service environment where a managed IT services company supports multiple enterprise clients.

The data contains information related to:

- Service tickets
- Customers and users
- Support agents
- SLA tracking
- Ticket activity
- Operational KPIs
- Customer satisfaction
- Management-level summaries

The main analysis focused on ticket activity, SLA performance, actual handling time and customer satisfaction.

The data used for the analysis covers the period from **April 2021 to July 2021**.

---

## 🛠️ Tools & Technologies

- Python
- PostgreSQL
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook
- Power BI

---

## 📂 What I Worked On

### 1. PostgreSQL Database

I worked with the ITSM database structure and used PostgreSQL for the database side of the project.

The database contains tables related to companies, users, tickets, SLA records, KPIs and ticket activity.

### 2. Data Loading & Preparation

The ticket and SLA data were loaded into Python and prepared for analysis.

The two datasets were merged in Jupyter Notebook using Pandas.

The final cleaned dataset contained:

- 360,000 rows
- 29 columns

Two additional columns were also created during data preparation:

- `sla_variance_minutes`
- `sla_performance_percentage`

### 3. Exploratory Data Analysis

I performed different types of EDA to understand the data:

- Univariate Analysis
- Bivariate Analysis
- Multivariate Analysis

The analysis included numerical summaries, distributions, comparisons and visualizations.

### 4. SLA Analysis

A major part of the project was understanding SLA performance.

I looked at:

- SLA status
- SLA type
- SLA target time
- Actual time
- Breach minutes
- SLA variance
- SLA performance percentage

### 5. Customer Satisfaction

I also explored customer satisfaction ratings and compared them with SLA-related information to understand whether there were noticeable patterns in the data.

---

## 📊 Power BI Dashboard

To make the analysis more interactive, I created a Power BI dashboard using the cleaned ITSM dataset.

The dashboard focuses on SLA performance, customer satisfaction and actual handling time.

### Dashboard Includes

#### KPI Cards

- Total SLA Records
- SLA Breached
- SLA Met
- SLA Breach Percentage
- Average Customer Satisfaction (CSAT)
- Average Actual Time
- Average SLA Performance
- Average SLA Variance

#### Visual Analysis

- Total SLA Records by SLA Status
- Total SLA Records by SLA Type and SLA Status
- Average CSAT by SLA Status
- Average SLA Variance by SLA Status
- Average SLA Performance by SLA Type

#### Interactive Filters

- SLA Type
- SLA Status

The dashboard was created to make the main analysis easier to understand through visual comparisons and interactive filtering.

---

## 📊 Some Key Observations

During the analysis, I found that **310,006 SLA records were breached**, while **49,994 were met**.

The Resolution SLA showed a particularly noticeable pattern, with all **180,000 Resolution SLA records marked as breached** in this dataset.

I also compared customer satisfaction across SLA statuses. The average CSAT was approximately **3.01** for both breached and met records, so the analysis did not show a strong difference in average customer satisfaction based on SLA status alone.

The overall SLA breach percentage was approximately **86.11%**.

These observations helped me understand why it is important to look at the actual data before making business conclusions.

---

## 🧹 Data Quality Checks

Before performing the analysis, I checked the dataset for:

- Missing values
- Duplicate rows
- Invalid values
- Numerical outliers
- Negative SLA-related values

There were no exact duplicate rows, and the IQR-based check did not identify potential numerical outliers.

There were also missing Customer Satisfaction Rating values, which were kept as missing because they represented records where a rating was not provided.

---

## 💡 What I Learned

This project helped me understand how a data analysis project moves from database data to useful insights.

Some of the main things I learned were:

- How PostgreSQL data can be brought into Python for analysis
- How to prepare and merge datasets using Pandas
- How to perform univariate, bivariate and multivariate analysis
- How to create visualizations to understand data
- How to work with SLA-related metrics
- How to create useful derived columns
- How to work with Power BI dashboards
- How interactive filters can be used to explore data
- Why data quality checks are important before analysis
- How to connect technical analysis with a business problem

One thing I learned especially from this project is that creating charts is only one part of analysis.

Understanding the data first is what makes the analysis meaningful.

---

## 📁 Project Structure

```text
ITSM-Service-Desk-Ticket-Operations/
│
├── 01_Business Problem.pdf
├── 02_Dataset Overview.pdf
├── 03_Datacleaning.ipynb
├── 04_Unianalysis.ipynb
├── 05_Bianalysis.ipynb
├── 06_Multianalysis.ipynb
├── 07_Exploratory Data Analysis Report.pdf
├── 08_Key Insights Report.pdf
├── 09_Executive Summary Report.pdf
├── 10_Conclusion Report.pdf
├── 11_ITSM SQL Queries.pdf
├── 12_ITSM ER Diagram.png
├── 13_ITSM DASHBOARD.pbix
└── README.md
```

🎯 Project Outcome

Overall, this project gave me practical experience in working with database data, preparing data for analysis, performing EDA and finding business-related observations from ITSM ticket and SLA information.

The project also helped me understand that good analysis is not only about writing code or creating graphs.

It is about:

Understand → Prepare → Analyze → Visualize → Find Insights

🌱 Learning Takeaway

This project was a good opportunity for me to apply the Python and SQL concepts I had been learning to a practical dataset.

There were challenges during the process, especially around understanding the data and checking whether the results actually made sense.

Working through those problems was an important part of the learning experience.

Still learning. Still building. Still improving. 🚀
