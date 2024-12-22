E-commerce Database with MongoDB

This project demonstrates the creation and management of an E-commerce database using MongoDB and Python.

Schema Design Decisions:

Customers:
Embedded Address: The address of a customer is embedded within the customer document. This simplifies data access and updates related to customer addresses.
Products:
Flat Schema: Products are stored as flat documents, as they typically don't have complex nested structures. This keeps the data structure simple and efficient.
Orders and Order Items:
Referenced Schema: Orders and order items are linked through references. This avoids data duplication and improves scalability, especially when dealing with a large number of orders and order items.
Running the Scripts:

Prerequisites:

MongoDB: Ensure MongoDB is installed and running on your system.
Python: Install the required Python libraries:
Bash

pip install pymongo pandas names_generator
Run the Python script: Execute the Python script (e.g., ecommerce_db.py) in your terminal. This will:

Create and populate the collections (customers, products, orders, order_items) with sample data.
Perform data analysis queries (e.g., revenue by category, delivery time, customer count).
Queries and Results:

Revenue by Category:
Calculates the total revenue and number of orders for each product category.
Results are displayed in descending order of revenue.
Delivery Time:
Calculates the average delivery time for all orders.
Customer Count by State:
Counts the number of customers in each state and city.
Results are displayed in descending order of customer count.
Top Products per Order:
Identifies the top 3 most expensive products in each order.
Key Features:

Data Generation: Generates realistic sample data for customers, products, orders, and order items.
Data Analysis: Performs various data analysis queries to gain insights into the E-commerce data.
Schema Design: Implements appropriate schema designs for different entities.
Indexes: Creates indexes on frequently queried fields for improved query performance.
Transaction Handling: Demonstrates atomic order creation with product stock updates within a transaction.
Change Monitoring: Shows how to monitor real-time changes in the orders collection.
Data Validation: Ensures all products have valid prices.
This README provides a basic overview of the project. For more detailed information, refer to the comments within the Python script.