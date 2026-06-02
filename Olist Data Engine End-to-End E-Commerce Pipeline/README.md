## Olist Data Engine: End-to-End E-Commerce Pipeline

# Project overview
This project addresses the critical business challenge of operational inefficiency and logistics bottlenecks in digital retail. Using a comprehensive database of over 100,000 Brazilian e-commerce transactions, I developed an end-to-end data pipeline that moves from raw data processing to a live interactive executive reporting dashboard.

The goal of this project was to analyze shipping delays, evaluate product performance, map out geographic revenue distribution, and establish concrete operational insights to protect customer satisfaction.

---

# Tech Stack
 * Data Processing: Python (Pandas, NumPy)

 * Querying & Metrics: SQL

 * Business Intelligence: Tableau Public

 * Documentation: Markdown

---

# The Data Pipeline

The project is organized into four distinct phases:

 * Data Cleaning & EDA: Handled missing relational records, formatted complex timestamp datatypes, and merged multiple datasets to establish a unified "Source of Truth."

 * Structural Verification: Applied SQL queries to validate transactional integrity, extract database metrics, and structure high-level business fields for reporting.

 * Logistical Impact Modeling: Analyzed the correlation between shipment fulfillment delays and historical customer satisfaction trends.

 * Executive Dashboard: Designed a 1-page fully synchronized interactive dashboard for regional performance tracking and operational scenario planning.

---

# Key Business Insights

Based on the live telemetry and historical order trends:

 * Total Transactional Revenue Analyzed: Over R$ 19.6M+ in sales value across the country.

 * Fulfillment Volume: Successfully tracked and segmented 95k+ unique customer orders.

 * The 3-Day Shipping Rule: Pinpointed a critical "cliff drop" in customer satisfaction, where average scores plummet from a healthy 4.0 down to 1.8 stars when delivery delays exceed 3 days.

 * Regional Concentration: Identified the state of São Paulo as the primary operational hub, contributing the highest volume of orders and overall business revenue.

---

# Repository Structure

├── notebooks/                  # Step-by-step technical analysis in Python
│   └── Data_Cleaning&EDA.ipynb  # Merging relational datasets and formatting timestamps
│   └── Data_Collection.ipynb    # Collecting raw data 
├── sql_queries/                # SQL verification scripts
│   └── 01_business_kpis.sql
    └── 02_Customer Analysis.sql
    └── 03_Delivery Analysis.sql
    └──04_payment_analysis.sql
    └──05_advance analysis.sql
│
├── Olist Brazilian E-Commerce Analytics Dashboard.twbx  # Original Tableau workbook file for local layout inspection
│
└── README.md                   # Project documentation and business summary

---

# Dashboard Preview
[👉 Click Here to Interact with the Live Dashboard][dashboard]

*Note: Clicking on the live link above will open the fully interactive version of this dashboard. Since no static images are used, you can interact directly with the dynamic maps, charts, and KPI cards via Tableau Public. Selecting any specific state on the interactive map will automatically filter and update the synchronized revenue trends, top product categories, and delivery metrics.*

---

# How to Run

Clone the repository to your local system.

Open the Jupyter Notebooks inside the `notebooks/` folder to view the Python data wrangling process.

Execute the scripts inside `sql_queries/` within your SQL workbench for database metric extraction.

Download the `.twbx` workbook file to inspect, edit, or interact with the visualization layer locally using Tableau Desktop or Tableau Public.

[dashboard]: https://public.tableau.com/app/profile/aashi.thakur/viz/OlistBrazilianE-CommerceAnalyticsDashbarod/Dashboard1