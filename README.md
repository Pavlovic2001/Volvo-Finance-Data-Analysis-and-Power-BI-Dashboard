[README.md](https://github.com/user-attachments/files/26467743/README.md)
# Volvo Finance Data Analysis and Power BI Dashboard

This project demonstrates a complete, end-to-end workflow for collecting, processing, and visualizing Volvo Car AB financial data. It showcases the integration of Excel, SQL, and Power BI to generate an interactive report providing insights into financial performance and key metrics.

The project highlights a full pipeline: from data scraping and cleaning to relational database modeling, SQL query development, and interactive dashboard creation.

## Technology Stack

-   **Data Collection & Cleaning**: Excel, PostgreSQL
-   **Database & SQL Queries**: PostgreSQL  
-   **Visualization**: Power BI  

## Key Features

-   **Data Collection & Preparation**: Scraped financial data from Volvo Car AB Annual and Sustainability Report 2024 and structured it in Excel for consistency and accuracy.  
-   **Relational Data Modeling**: Built and normalized relational tables in PostgreSQL to enable robust analytics pipelines.  
-   **Advanced SQL Queries**: Created SQL scripts for extracting, combining, and preparing datasets for analysis (`Finance.sql`, `Volume.sql`, `Joins.sql`, `Load_tables.sql`).  
-   **Interactive Power BI Dashboard**: Visualized financial insights, trends, and key metrics, enabling stakeholders to make data-driven decisions.  
-   **Documentation & Reporting**: Provided both a `.pdf` summary and `.pbix` interactive dashboard for full reporting.

## File Structure
```bash
├── Finance_dataset.csv          # Raw financial dataset
├── Model_volume_dataset.csv     # Raw dataset for volume modeling
├── Region_finance_dataset.csv   # Dataset by region
├── Volume_dataset.csv           # Volume dataset
├── volvo_cars_key_financial_data_q4_2024_final.xlsx  # Original cleaned Excel file
├── Finance.sql                  # SQL schema and table creation
├── Volume.sql                   # SQL schema and table creation for volume
├── Joins.sql                    # SQL queries to join and process tables
├── Load_tables.sql              # SQL scripts to load data into PostgreSQL
├── volvo_analytics.pbix         # Power BI interactive dashboard
├── volvo_analytics.pdf          # Exported PDF report of dashboard
├── Volvo_analytics.zip           # Optional zipped backup of Power BI file
├── README.md
```

## Getting Started

Follow these steps to replicate the project locally.

### Prerequisites

-   PostgreSQL  
-   Power BI Desktop  
-   Excel 2016+ (for initial dataset handling)  

### Setup & Installation

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/Volvo-Finance-Data-Analysis-and-Power-BI-Dashboard
    ```

2.  **Database Setup:**
    - Open PostgreSQL and create a database.  
    - Run the SQL scripts in this order:
      ```sh
      psql -f Finance.sql
      psql -f Volume.sql
      psql -f Load_tables.sql
      ```
    - Use `Joins.sql` to extract combined datasets for analysis.

3.  **Data Preparation:**
    - Ensure all `.csv` and `.xlsx` files are in the appropriate directories.  
    - Verify data consistency and quality in Excel or your preferred editor.

## Usage / Workflow

1.  **Load & Explore Data:**
    - Use PostgreSQL to query and validate the datasets.

2.  **Data Analysis & Modeling:**
    - Perform aggregations, trends, and KPI calculations using SQL queries in PostgreSQL.

3.  **Power BI Dashboard:**
    - Open `volvo_analytics.pbix` in Power BI Desktop.  
    - Explore interactive visualizations of key financial metrics, volume trends, and regional comparisons.

## Workflow Overview

- Collect and clean financial datasets in Excel  
- Model relational tables and create SQL pipelines in PostgreSQL  
- Execute queries to extract insights and combine data  
- Load prepared datasets into Power BI  
- Build an interactive dashboard and export PDF reports  
