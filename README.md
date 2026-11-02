# Employee Health Center Database (SQL Project)

A beginner SQL project built in MySQL that models an employee database for a health center and practices core query skills.

## What's inside
- `health_center.sql`: database setup, table creation, sample data, and queries

## Database design
**Database:** `health_center`

**Table:** `employees`

| Column | Type | Notes |
|---|---|---|
| employee_id | INT | Primary key, auto increment |
| employee_name | VARCHAR(100) | |
| department | VARCHAR(100) | |
| age | INT | |

## How to run
1. Open MySQL Workbench (or any MySQL client)
2. Open `health_center.sql`
3. Run the whole script. It's safe to run many times because it drops and recreates the database each time

## SQL concepts practiced
- CREATE DATABASE / CREATE TABLE
- INSERT INTO
- SELECT
- WHERE
- AND, OR, IN
- ORDER BY

  ## Example queries

| # | Query | What it does | Result |
|---|---|---|---|
| 1 | `WHERE department = 'Operations'` | Filters by one department | Sujith |
| 2 | `WHERE age > 30` | Employees older than 30 | Rishav, Wakib, Emmi |
| 3 | `WHERE department = 'Operations' AND age > 30` | Both conditions must be true | 0 rows |
| 4 | `WHERE employee_name = 'Girish'` | Finds one employee | Girish |
| 5 | `WHERE department = 'Operations' OR department = 'Admin'` | Either condition can be true | Girish, Sujith |
| 6 | `ORDER BY age DESC` | Sorts by age, highest first | All employees, oldest first |

## Sample data
7 employees across departments: HR, Finance, Security, Housekeeping, Admin, Operations, Supervisor.
## Example queries

| # | Query | What it does | Result |
|---|---|---|---|
| 1 | `WHERE department = 'Operations'` | Filters by one department | Sujith |
| 2 | `WHERE age > 30` | Employees older than 30 | Rishav, Wakib, Emmi |
| 3 | `WHERE department = 'Operations' AND age > 30` | Both conditions must be true | 0 rows |
| 4 | `WHERE employee_name = 'Girish'` | Finds one employee | Girish |
| 5 | `WHERE department = 'Operations' OR department = 'Admin'` | Either condition can be true | Girish, Sujith |
| 6 | `ORDER BY age DESC` | Sorts by age, highest first | Oldest to youngest |
| 7 | `WHERE department = 'Security'` | Filters by Security department | Rishav |
| 8 | `WHERE age < 30` | Employees younger than 30 | Rahul, Shreya, Sujith |
| 9 | `WHERE department IN ('Operations', 'Admin') ORDER BY employee_name` | Same as query 5, written shorter with IN, sorted A to Z | Girish, Sujith |
| 10 | `ORDER BY age ASC` | Sorts by age, lowest first | Youngest to oldest |

## Sample data
7 employees across departments: HR, Finance, Security, Housekeeping, Admin, Operations, Supervisor.

## Author
Suprova Mondal
