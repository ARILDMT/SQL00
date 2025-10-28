# SQL Bootcamp - Day 00

A comprehensive introduction to relational databases and SQL, focusing on fundamental query techniques including subqueries, date filtering, and data manipulation.

## Overview

This project demonstrates proficiency in SQL fundamentals through a series of progressively challenging exercises. The exercises utilize a pizza delivery database schema to practice real-world query scenarios.

## Database Schema

The project uses a relational database with five interconnected tables:

- **pizzeria** - Restaurant directory with ratings
- **person** - Customer information
- **menu** - Pizza offerings and prices by restaurant
- **person_visits** - Visit history to restaurants
- **person_order** - Order transaction records

![Database Schema](misc/images/schema.png)

## Skills Demonstrated

- Writing SELECT queries with filtering and sorting
- Using comparison operators and BETWEEN clauses
- Working with subqueries in SELECT and FROM clauses
- Date range filtering and manipulation
- Calculated fields and conditional expressions (CASE statements)
- String concatenation and formatting
- Query optimization without JOINs
- Data analysis across multiple related tables

## Project Structure

```
.
├── materials/
│   └── model.sql          # Database schema and seed data
├── src/
│   ├── ex00/              # Basic SELECT queries
│   ├── ex01/              # Filtering and sorting
│   ├── ex02/              # Range queries
│   ├── ex03/              # Date filtering
│   ├── ex04/              # Calculated fields
│   ├── ex05/              # Subqueries in SELECT
│   ├── ex06/              # Conditional expressions
│   ├── ex07/              # CASE statements
│   ├── ex08/              # Modulo operations
│   └── ex09/              # Subqueries in FROM
└── README.md
```

## Setup

1. Ensure PostgreSQL is installed on your system
2. Create a new database:
   ```bash
   createdb pizza_db
   ```
3. Load the database schema and data:
   ```bash
   psql -d pizza_db -f materials/model.sql
   ```
4. Run individual exercises:
   ```bash
   psql -d pizza_db -f src/ex00/day00_ex00.sql
   ```

## Exercises

### Exercise 00: Basic Selection
Select names and ages of people from a specific city.

### Exercise 01: Filtering with Sorting
Query with WHERE clause and ORDER BY on multiple conditions.

### Exercise 02: Range Queries
Two syntactically different approaches to range filtering (comparison operators vs BETWEEN).

### Exercise 03: Date Filtering
Complex filtering with date ranges and multiple OR conditions.

### Exercise 04: Calculated Fields
String concatenation to create formatted output with proper quoting.

### Exercise 05: Subqueries in SELECT
Using subqueries in the SELECT clause to retrieve related data.

### Exercise 06: Conditional Logic
Implementing boolean checks using CASE expressions.

### Exercise 07: Age Intervals
Categorizing data into intervals using nested CASE statements.

### Exercise 08: Even Numbers
Filtering results using modulo operations.

### Exercise 09: Subqueries in FROM
Complex queries using subqueries in the FROM clause for virtual tables.

## Constraints

Each exercise has specific requirements and restrictions:
- Language: ANSI SQL
- Some exercises prohibit JOINs and IN clauses to focus on alternative techniques
- Emphasis on subquery usage and creative problem-solving

## Technologies

- PostgreSQL (latest version recommended)
- SQL (ANSI standard)

## Learning Outcomes

This project develops fundamental SQL skills essential for:
- Data analysis and reporting
- Backend application development
- Database administration
- Understanding relational data models

## License

This project is available under the MIT License. See [LICENSE](LICENSE) for details.

---

**Note**: This is an educational project focusing on SQL fundamentals and query construction techniques.
