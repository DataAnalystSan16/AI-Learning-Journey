# Day 14 – AI-Assisted SQL Business Analysis
**Phase 1: AI Faster | 20 November 2026**

## Objective
Turn retail-management questions into SQL, validate AI-assisted queries against the actual MySQL schema, interpret outputs, and make business recommendations.

## Exercises completed
1. **Top 3 best-selling products** – identified the required tables (`products`, `order_items`), join key (`product_id`), `SUM(quantity)`, descending sort and `LIMIT 3`. Query logic and schema were validated; an execution-result screenshot was not captured in the learning record.
2. **Category-wise revenue** – Electronics ₹110,000; Furniture ₹50,000; Grocery ₹8,500; Clothing ₹6,500; Home Appliances ₹3,995. Total ₹178,995. These are gross revenue figures before discounts and returns.
3. **Product-wise gross profit** – used `(unit_selling_price × quantity) − discount_amount − (unit_cost_at_sale × quantity)`. Used historical `unit_cost_at_sale` rather than current/reference `standard_cost`.
4. **Product-wise profit margin** – calculated gross profit ÷ net sales × 100 and used `NULLIF` to protect against division by zero. Men's T-Shirt led the reported margins at 46.60%, followed by Women's Jeans at 41.34%.
5. **Store-wise gross profit and margin** – Bangalore Central led gross profit (₹24,598) and net sales (₹112,698); Hyderabad Central led margin (28.07%) but had the lowest gross profit (₹3,200) and net sales (₹11,400).

## Key SQL concepts
- `INNER JOIN` using validated primary/foreign key relationships
- `SUM()` with `GROUP BY`
- `ORDER BY` and `LIMIT`
- Revenue, net sales, gross profit and profit margin calculations
- `NULLIF()` for safe division
- Business interpretation and recommendation from query outputs

## Business recommendation
For Hyderabad Central, improve store visibility and promotions, understand customer needs, and pilot additional products/categories only after validating demand. Monitor sales, gross profit, margin, stock availability and inventory turnover together. A high margin alone is not enough to justify increasing stock.

## Validation and assumptions
- `discount_amount` is treated as the total discount for each order-item row.
- Category revenue is before discounts and returns.
- Profit calculations use `unit_cost_at_sale` for historical cost.
- The store output shown was not adjusted for cancellations or returns.
- Gross-profit figures in separate exercise outputs differed slightly; figures are retained as displayed rather than silently reconciled.
- Exercise 1 query logic was validated, but its actual execution result was not captured.

## Takeaway
I learned to use AI as a learning and query-development partner while personally checking table names, join keys, formulas and results. I also practised moving from SQL output to practical, evidence-based business recommendations.
