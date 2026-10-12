# SPECIAL-OPERATORS_SQL_ASSINGMENT
# SQL Special Operators Practice

## 📌 About the Project

This repository contains my Oracle SQL practice queries focused on **special operators, filtering conditions, and data retrieval** using the `EMP` and `DEPT` tables.

The examples demonstrate how to retrieve specific records based on employee names, job roles, salaries, department numbers, commission values, and hire dates. This repository is created to strengthen my SQL fundamentals and improve my database query-writing skills.

## 🎯 Objectives

- Understand SQL special operators.
- Practice filtering records using the `WHERE` clause.
- Learn pattern matching and NULL value checking.
- Apply multiple conditions using logical operators.
- Perform salary calculations and display calculated columns.
- Identify and correct common SQL syntax errors.

## 🛠️ Technologies Used

- **Database:** Oracle Database
- **Language:** SQL
- **Environment:** Oracle SQL*Plus

## 📚 Topics Covered

| Operator / Concept | Purpose |
|---|---|
| `IN` | Matches values from a specified list |
| `NOT IN` | Excludes specified values |
| `BETWEEN` | Checks whether a value falls within a range |
| `NOT BETWEEN` | Excludes values within a range |
| `LIKE` | Matches patterns in text |
| `IS NULL` | Checks for NULL values |
| `IS NOT NULL` | Checks for non-NULL values |
| `AND` | Combines conditions that must all be true |
| `OR` | Combines conditions where at least one must be true |
| `NOT LIKE` | Excludes values matching a pattern |
| `WHERE` | Filters records based on conditions |
| Column Aliases | Gives meaningful names to calculated columns |

## 💻 Sample SQL Queries

### 1. Find Employees with NULL Commission

```sql
SELECT *
FROM EMP
WHERE COMM IS NULL;
```

### 2. Find Employees in Department 30

```sql
SELECT *
FROM EMP
WHERE DEPTNO = 30;
```

### 3. Find Employees with Salaries Between 1000 and 3000

```sql
SELECT *
FROM EMP
WHERE SAL BETWEEN 1000 AND 3000;
```

### 4. Find Employees Whose Names Start with 'S'

```sql
SELECT *
FROM EMP
WHERE ENAME LIKE 'S%';
```

### 5. Calculate Annual Salary

```sql
SELECT EMP.*, SAL * 12 AS ANNUAL_SAL
FROM EMP
WHERE DEPTNO NOT IN (30);
```

### 6. Find Employees with Non-NULL Managers

```sql
SELECT *
FROM EMP
WHERE MGR IS NOT NULL;
```

## 📂 Repository Contents

- `SPECIAL OPERATORS.txt` — SQL practice queries and their outputs, including examples of filtering conditions and query corrections.
- `README.md` — Project overview, topics covered, and sample queries.

## 🚀 How to Use

1. Clone or download this repository.
2. Open Oracle SQL*Plus or another Oracle SQL environment.
3. Ensure the sample `EMP` and `DEPT` tables are available.
4. Open `SPECIAL OPERATORS.txt`.
5. Execute the queries one by one and observe the results.

## 🎓 Learning Outcomes

Through this practice, I improved my understanding of Oracle SQL operators, data filtering, pattern matching, NULL handling, logical conditions, and calculated columns.

## 🔮 Future Improvements

- Practice SQL aggregate functions.
- Learn `GROUP BY` and `HAVING`.
- Explore SQL joins and subqueries.
- Practice functions, constraints, and data manipulation statements.
- Solve more SQL interview and placement questions.

## 👩‍💻 Author

**Shaziya**

B.Tech CSE (IoT) Student 



⭐ If you find this repository useful, feel free to explore the queries and practice along with me.
