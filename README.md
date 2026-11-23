# SQL Data Analytics

A SQL Server portfolio project for exploring sales data and building customer and product reports. The goal is to practice translating business questions into SQL queries, from basic exploration to window-function analysis.

**Tools:** Microsoft SQL Server, T-SQL, SQL Server Management Studio, Git.

## Questions explored

- How do sales change by month and year?
- Which customers and products contribute most to sales?
- How do current results compare with previous periods and averages?
- How can customers and products be grouped using the available business metrics?

## Files and analysis order

The data used by the initializer is in `datasets/csv-files/`, including `gold.dim_customers.csv`, `gold.dim_products.csv`, and `gold.fact_sales.csv`. Other Bronze, Silver, and report CSV files are also supplied. No database backup file is included.

```text
scripts/
  00_init_database.sql
  01_database_exploration.sql
  02_dimensions_exploration.sql
  03_date_range_exploration.sql
  04_measures_exploration.sql
  05_magnitude_analysis.sql
  06_ranking_analysis.sql
  07_change_over_time_analysis.sql
  08_cumulative_analysis.sql
  09_performance_analysis.sql
  10_part_to_whole_analysis.sql
  11_data_segmentation.sql
  12_report_customers.sql
  13_report_products.sql
```

Scripts 01 to 06 explore the schema, dimensions, date ranges, metrics, and rankings. Scripts 07 to 11 cover trends, cumulative measures, comparisons, category contributions, and segmentation. Scripts 12 and 13 create the customer and product report views.

## Before running

> **Destructive setup:** `scripts/00_init_database.sql` drops and recreates `DataWarehouseAnalytics` if it exists. All existing contents will be deleted. Run only in a disposable development database after reviewing the script and backing up anything important.

SQL Server permissions are needed for database creation and `BULK INSERT`. The SQL Server service must have access to the CSV folder, including when the database server is remote.

## Setup

```bash
git clone https://github.com/Ahmedbadour14/sql-data-analytics-project.git
cd sql-data-analytics-project
```

1. Open `scripts/00_init_database.sql`. Change each hardcoded path containing `01_datasets/csv-files` to your actual server-readable `datasets/csv-files` location. Match each CSV filename exactly.
2. Review the destructive setup warning, then run the initializer in your development instance.
3. Select `DataWarehouseAnalytics` as the database context. Run analysis scripts 01 to 11 in order and inspect the outputs.
4. Run scripts 12 and 13 to create `gold.report_customers` and `gold.report_products`.
5. Explore the generated views:

```sql
USE DataWarehouseAnalytics;
GO
SELECT TOP (20) * FROM gold.report_customers;
SELECT TOP (20) * FROM gold.report_products;
```

These preview queries have no specified ordering. Add an explicit `ORDER BY` when answering a ranked business question.

## Reports

- **Customer report:** order and sales totals, quantity, product count, lifespan, recency, spending metrics, and customer segments.
- **Product report:** sales and order totals, quantity, customer count, lifespan, recency, revenue metrics, and product performance segments.

The SQL demonstrates aggregations, CASE expressions, date functions, CTEs, joins, and window functions. Some recency calculations use the current date, so outputs can change when the same scripts are run later.

## Limits and next documentation steps

This is a learning and portfolio project, not evidence of production deployment or measured business impact. Reproducible query-output examples and their interpretation still need to be added. Dataset/course attribution and my own changes should be documented before presenting the project as fully documented.

## License and author

See [MIT License](LICENSE) for the code license; dataset rights must be checked separately.

[Ahmed Badour](https://github.com/Ahmedbadour14)
