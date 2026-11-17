
# Day 13 – AI-Assisted SQL: JOINs and Aggregations

## Learning Objective
Practise combining relational database tables and generating store-wise business insights using SQL.

## Database
retail_sales_intelligence

## Topics Practised
1. INNER JOIN – two tables
2. INNER JOIN – three tables
3. Table aliases
4. WHERE filtering
5. COUNT() and COUNT(DISTINCT)
6. SUM() for gross sales
7. GROUP BY
8. HAVING
9. Discount-adjusted net sales
10. Independent business reporting challenge

## Hands-on Project Work

Used the stores, orders and order_items tables to generate a store-wise sales report.

### Final Results

| Store | Orders | Gross Sales | Discounts | Net Sales |
|---|---:|---:|---:|---:|
| Bangalore Central | 3 | 116598 | 3900 | 112698 |
| Bangalore South | 2 | 34498 | 1100 | 33398 |
| Chennai Central | 3 | 29947 | 1175 | 28772 |
| Hyderabad Central | 2 | 12100 | 700 | 11400 |

## Key Learnings
- Understood how primary and foreign keys connect tables.
- Learned the difference between WHERE and HAVING.
- Used COUNT(DISTINCT) to avoid counting the same order multiple times.
- Calculated gross sales using unit selling price × quantity.
- Calculated net sales after deducting discounts.
- Practised validating SQL output against business expectations.

## Learning Reflection
Today I learned how to translate business requirements into SQL queries.

I independently attempted the final store-wise sales report and corrected mistakes involving JOIN conditions, table aliases and aggregate functions.

AI helped me understand concepts, review my queries and improve my SQL problem-solving skills. I executed the SQL queries myself in MySQL Workbench.

## Day 13 Status
Completed – 8 exercises.

Next: Day 14 – AI Learning Journey.
