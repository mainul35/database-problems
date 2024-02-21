## Scenario:
Imagine you're working for an e-commerce company that sells electronic devices. Your task is to manage the database for the products, customers, orders, and shipments.

### Table Designs:

#### Products Table:
Columns: product_id (Primary Key), name, description, price, quantity_available
#### Customers Table:
Columns: customer_id (Primary Key), name, email, address
#### Orders Table:
Columns: order_id (Primary Key), customer_id (Foreign Key), order_date, total_amount
#### Order_Items Table:
Columns: order_item_id (Primary Key), order_id (Foreign Key), product_id (Foreign Key), quantity, subtotal
#### Shipments Table:
Columns: shipment_id (Primary Key), order_id (Foreign Key), shipment_date, status
Sample Data:

<b>Let's populate some sample data for these tables:</b>

#### Products Table:

| product_id | name       | description                | price | quantity_available |
|------------|------------|----------------------------|-------|--------------------|
| 1          | Laptop     | High performance laptop    | 800   | 10                 |
| 2          | Smartphone | Latest smartphone model    | 600   | 20                 |
| 3          | Headphones | Noise-canceling headphones | 150   | 30                 |
| 4          | Tablet     | Portable tablet            | 400   | 15                 |

#### Customers Table:

| customer_id | name          | email             | address     |
|-------------|---------------|-------------------|-------------|
| 1           | John Doe      | john@example.com  | 123 Main St |
| 2           | Jane Smith    | jane@example.com  | 456 Elm St  |
| 3           | Alice Johnson | alice@example.com | 789 Oak St  |
#### Orders Table:

| order_id | customer_id | order_date | total_amount |
|----------|-------------|------------|--------------|
| 101      | 1           | 2024-02-10 | 1200         |
| 102      | 2           | 2024-02-15 | 800          |
| 103      | 3           | 2024-02-20 | 550          |
#### Order_Items Table:

| order_item_id | order_id | product_id | quantity | subtotal |
|---------------|----------|------------|----------|----------|
| 1             | 101      | 1          | 1        | 800      |
| 2             | 101      | 3          | 2        | 300      |
| 3             | 102      | 2          | 1        | 600      |
| 4             | 103      | 4          | 1        | 400      |
| 5             | 103      | 3          | 1        | 150      |
#### Shipments Table:

| shipment_id | order_id | shipment_date | status  |
|-------------|----------|---------------|---------|
| 501         | 101      | 2024-02-11    | Shipped |
| 502         | 102      | 2024-02-16    | Shipped |
| 503         | 103      | 2024-02-21    | Pending |
### Difficult Query Questions:

1. Retrieve the total revenue generated from each product in the last month.
2. List the names of customers who have made more than two orders.
3. Find the average quantity of products ordered by each customer.
4. Identify the product with the highest total sales amount.
5. List the customers who have not yet received their shipments.
6. Calculate the total revenue for each month of the year.
7. Retrieve the products that have never been ordered.
8. Find the customer who has spent the most money.
9. List the orders where the quantity of any product exceeds the available quantity.
10. Calculate the average time taken for each shipment to reach customers.