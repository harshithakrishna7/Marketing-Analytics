# Marketing Analytics SQL + Python + Power BI Project

This project is a marketing analytics portfolio project built using SQL Server, Python, and Power BI-style reporting logic. It focuses on customer, product, engagement, and review data to support insights around campaign performance, customer behavior, and sentiment analysis.

## Project Objective

The goal is to transform raw marketing data into a clean analytical layer and generate business-ready insights such as:

- customer segmentation and geography enrichment
- product and engagement performance analysis
- campaign interaction trends
- customer review sentiment analysis
- dashboard-ready data models for reporting

## Tech Stack

- SQL Server
- T-SQL
- Python
- Pandas
- NLTK VADER sentiment analysis
- Power BI for dashboard visualization
- CSV output for downstream reporting

## Power BI and Analytics Workflow

This project is designed to build a complete marketing analytics data pipeline for a Power BI dashboard. The SQL scripts prepare the dimensions and fact tables, Python adds business context through sentiment analysis, and the DAX calendar logic supports time-based reporting.

The workflow combines:

- customer and product dimension tables
- campaign and engagement fact data
- customer journey data for behavioral analysis
- review enrichment for sentiment and satisfaction insights
- a Power BI-ready reporting layer for visual storytelling

## Repository Structure

- `dim_customers.sql` — customer dimension table logic
- `dim_products.sql` — product dimension data preparation
- `fact_customer_reviews.sql` — fact table for customer review data
- `fact_engagement_data.sql` — marketing engagement and content performance data
- `fact_customer_journey.sql` — customer journey / funnel logic
- `customer_reviews_enrichment.py` — Python script to enrich review data with sentiment analysis
- `fact_customer_reviews_enrich.csv` — enriched customer review dataset
- `Calendar DAX Script.txt` — calendar logic for Power BI / DAX reporting
- `README.md` — project overview and usage guide

## Key Business Use Cases

- Track which campaigns and content types drive engagement
- Understand customer demographics and geography
- Evaluate customer satisfaction from review text
- Measure product and customer journey performance over time
- Create a reporting layer for a marketing analytics dashboard

## Data Flow

1. Raw marketing data is modeled in SQL using dimension and fact tables.
2. Customer and engagement datasets are cleaned and normalized.
3. Python is used to enrich customer reviews with sentiment scores.
4. The resulting data is structured for Power BI reporting and dashboard analysis.

## How to Use

1. Open the SQL files in SQL Server Management Studio or Azure Data Studio.
2. Run the dimension and fact scripts to create the analytical tables.
3. Execute the Python enrichment workflow for sentiment analysis.
4. Use the output CSV and DAX script as the reporting foundation.

## Example Workflow

```sql
SELECT *
FROM dbo.fact_engagement_data;
```

```python
# Run the sentiment enrichment script
python customer_reviews_enrichment.py
```

## Future Enhancements

- add more campaign attribution metrics
- build a full Power BI dashboard in a Windows environment
- add forecasting and retention analysis
- create automated SQL + Python pipeline scripts

## Author

Harshitha Krishna
