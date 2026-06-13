# Online Bookstore Database Practice

This repository contains the solution to the Online Bookstore Database practice mission. It includes table schema definitions, sample data population, and various analytical queries performed using PostgreSQL.

## File Contents

- `postgre.sql`: Contains the DDL to create the tables (`customers`, `books`, `orders`), DML to populate them with the provided dataset, and the SQL queries for the practice questions.

## Database Schema

### `customers`
- `customer_id`: INTEGER (PK)
- `customer_first_name`: VARCHAR(50) (Renamed from `first_name`)
- `last_name`: VARCHAR(50)
- `email`: VARCHAR(100)
- `city`: VARCHAR(50)
- `country`: VARCHAR(50)
- `registration_date`: DATE

### `books`
- `book_id`: INTEGER (PK)
- `title`: VARCHAR(200)
- `author`: VARCHAR(100)
- `genre`: VARCHAR(50)
- `price`: DECIMAL(10, 2)
- `publication_year`: INTEGER
- `stock_quantity`: INTEGER

### `orders`
- `order_id`: INTEGER (PK)
- `customer_id`: INTEGER (FK)
- `book_id`: INTEGER (FK)
- `order_date`: DATE
- `quantity`: INTEGER
- `total_amount`: DECIMAL(10, 2)

## Practice Queries

The `postgre.sql` file includes solutions for:
1. Sorting books by price.
2. Listing unique countries.
3. Filtering books by title prefix.
4. Schema alteration (renaming columns).
5. Filtering by genre.
6. Counting total orders.
7. Aggregating data with grouping and `HAVING` clauses.
8. Complex filtering with `LIKE` and `IN`.
9. String formatting with `UPPER`, `LOWER`, and concatenation.
10. Date-based aggregation for financial analysis.
