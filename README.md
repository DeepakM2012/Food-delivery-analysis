## 🍽️ Food Delivery Data Engineering & Analytics

This project demonstrates an end-to-end data engineering workflow where data from multiple sources and formats is transformed into a single, clean analytical dataset and used to generate meaningful business insights.

The task simulates a real-world scenario where transactional data, user master data, and restaurant master data must be integrated for analysis.

## 📁 Data Sources

| File Name       | File Type | Key Fields                         | Description                                                |
|-----------------|-----------|------------------------------------|------------------------------------------------------------|
| orders.csv      | CSV       | order_id, user_id, restaurant_id  | Transactional data containing all food orders              |
| users.json      | JSON      | user_id, name, city, membership   | User master data with membership and location details      |
| restaurants.sql | SQL       | restaurant_id, cuisine, rating    | Restaurant master data with cuisine type and ratings       |

## Engineering Workflow

- Loaded heterogeneous data formats using Python

- Converted SQL script into a table using SQLite

- Performed LEFT JOINS to preserve all order records:

- user_id to merge user information

- restaurant_id to merge restaurant details

- Cleaned, standardized, and renamed columns

- Generated a unified dataset: final_food_delivery_dataset.csv

- This dataset (10,000 rows) acts as the single source of truth for all analysis.

## Data Cleaning & Preparation

- Fixed date formats for time-based analysis

- Resolved duplicate columns after merge

- Renamed columns for clarity and consistency

- Ensured no missing values in the final dataset

## Analysis Performed

Using the final dataset, the following insights were derived:

- Order trends over time and quarterly revenue

- Behavior comparison between Gold and Regular members

- City-wise revenue performance

- Cuisine-wise average order value

- Restaurant performance using ratings and revenue

- Peak ordering hours and seasonal patterns

## Technologies Used

- Python

- Pandas

- SQLite

- Jupyter Notebook

## Repository Contents

- food_delivery_analysis.ipynb — Complete implementation
  
- final_food_delivery_dataset.csv — Clean merged dataset
  
- orders.csv — Raw order data

- users.json — User master data

- restaurants.sql — Restaurant master data

## Outcome

- This project highlights practical skills in:

- Data ingestion from multiple formats

- Data merging using keys

- Data cleaning and transformation

- Analytical querying and visualization

It reflects real-world data engineering and analytics practices used in industry.
