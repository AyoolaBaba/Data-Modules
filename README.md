# Data-Modules
All my notes for my data engineer training at sparta global in one place 

# Week 4

# Customer Orders Processing System

A Python program that loads customer and order data, combines them, calculates statistics, and generates a report.

## What it does

1. Loads customer data from a JSON file.
2. Loads order data from a CSV file.
3. Combines each order with its matching customer.
4. Calculates:
   - Total revenue
   - Revenue by customer
   - Revenue by city
   - Units sold by product
   - Average order value
   - Number of unique customers
5. Builds a final report and writes it to `output/report.json`.

## Files

- `Customers.json` - customer records (id, name, city)
- `orders.csv` - order records (order id, customer id, product, quantity, price)
- `main.py` - the program

## How to run
