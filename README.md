# Pizzahut SQL Analysis

A self-learning project where I practiced SQL by analyzing a Pizzahut-style sales dataset — progressing from basic aggregation to advanced window functions.

## Dataset

The dataset contains 4 tables:
- `orders` — order-level data (order id, date, time)
- `order_details` — line items per order (pizza id, quantity)
- `pizzas` — pizza variants (size, price)
- `pizza_types` — pizza names and categories

## Objectives

- Practice core SQL: COUNT, SUM, GROUP BY, filtering
- Apply intermediate techniques: multi-table JOINs, subqueries, ranking
- Master advanced concepts: correlated subqueries, window functions (`SUM() OVER`)

## File

All 12 queries are in [`pizzahut_sql_workbook.sql`](./pizzahut_sql_workbook.sql), ordered from basic to advanced.

## Key Findings

| # | Question | Key Result |
|---|----------|-----------|
| 01 | Total orders placed | 21,350 |
| 02 | Total revenue generated | ₹8,17,860.05 |
| 03 | Highest-priced pizza | The Greek Pizza (₹35.95) |
| 04 | Most common pizza size ordered | Large (18,526 orders) |
| 05 | Top 5 pizzas by quantity sold | Classic Deluxe led with 2,453 units |
| 06 | Total quantity by category | Classic: 14,888 |
| 07 | Order distribution by hour | Peak at 12–1 PM (2,520 orders) |
| 08 | Pizza count by category | Veggie & Supreme: 9 each |
| 09 | Avg. pizzas ordered per day | 138 |
| 10 | Top 3 pizza types by revenue | The Thai Chicken Pizza (₹43,434.25) |
| 11 | % revenue contribution by category | Classic 26.91%, Supreme 25.46%, Chicken 23.96%, Veggie 23.68% |
| 12 | Cumulative revenue over time | Running total via `SUM() OVER (ORDER BY order_date)` |

## Tools Used

- MySQL Workbench
- SQL (joins, subqueries, aggregate functions, window functions)

## Author

**Pratyush Kr. Singh**
