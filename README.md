# task-7-sales-summary
Sales summary using SQLite and Python

## Objective
To extract basic sales information from a SQLite database using SQL inside Python.

## Tools Used
- Python
- SQLite
- pandas
- matplotlib
- Jupyter Notebook

## Steps Performed
1. Created a SQLite database and sales table
2. Inserted sample sales data
3. Used SQL queries with GROUP BY to calculate total quantity and revenue
4. Loaded SQL results into pandas DataFrame
5. Displayed the sales summary
6. Visualized revenue using a bar chart

## SQL Query Used
```sql
SELECT product,
       SUM(quantity) AS total_quantity,
       SUM(quantity * price) AS revenue
FROM sales
GROUP BY product;
