# Employee Database Management System

## 📌 Project Overview

This project demonstrates the use of **MySQL** to create and analyze an Employee Database. It contains employee information such as name, gender, mother tongue, department, salary, date of birth, date of joining, and experience.

The project includes **50 SQL queries** covering basic to intermediate SQL concepts such as filtering, sorting, aggregation, grouping, date functions, and conditional analysis.

---

## 🎯 Objectives

* Create and manage an employee database using MySQL.
* Practice SQL queries for retrieving and filtering data.
* Perform employee and department-wise analysis.
* Use aggregate functions to generate meaningful insights.
* Analyze salary, experience, gender, department, and joining-date information.
* Strengthen practical SQL and database management skills.

---

## 🛠️ Technologies Used

* **Database:** MySQL
* **Language:** SQL
* **Tool:** MySQL Workbench

---

## 🗃️ Database Structure

### Database

`details`

### Table

`employee`

| Column          | Data Type     | Description              |
| --------------- | ------------- | ------------------------ |
| `emp_id`        | INT           | Unique employee ID       |
| `emp_name`      | VARCHAR(50)   | Employee name            |
| `gender`        | VARCHAR(10)   | Employee gender          |
| `mother_tongue` | VARCHAR(30)   | Employee's mother tongue |
| `department`    | VARCHAR(30)   | Employee department      |
| `salary`        | DECIMAL(10,2) | Employee salary          |
| `dob`           | DATE          | Date of birth            |
| `doj`           | DATE          | Date of joining          |
| `experience`    | INT           | Years of experience      |

---

## 📊 Dataset

The database contains **50 employee records** with information from different departments and language backgrounds.

### Departments

* IT
* HR
* Finance
* Sales
* Marketing
* Operations

### Other Attributes

* Gender
* Mother tongue
* Salary
* Date of birth
* Date of joining
* Experience

---

## 🔍 SQL Concepts Covered

### 1. Basic Data Retrieval

* `SELECT`
* `SELECT *`
* Selecting specific columns

### 2. Filtering

* `WHERE`
* `AND`
* `OR`
* `BETWEEN`
* `LIKE`

### 3. Sorting

* `ORDER BY ASC`
* `ORDER BY DESC`

### 4. Removing Duplicates

* `DISTINCT`

### 5. Limiting Results

* `LIMIT`

### 6. Aggregate Functions

* `COUNT()`
* `SUM()`
* `AVG()`
* `MAX()`
* `MIN()`

### 7. Grouping & Analysis

* `GROUP BY`
* `HAVING`

### 8. Date Functions

* `YEAR()`
* `MONTH()`
* `CURDATE()`
* `TIMESTAMPDIFF()`

---

## 📈 Sample Queries

### Find employees working in IT

```sql
SELECT *
FROM employee
WHERE department = 'IT';
```

### Find employees earning more than 50,000

```sql
SELECT *
FROM employee
WHERE salary > 50000;
```

### Find department-wise employee count

```sql
SELECT department, COUNT(*) AS EmployeeCount
FROM employee
GROUP BY department;
```

### Find average salary by department

```sql
SELECT department, AVG(salary) AS AverageSalary
FROM employee
GROUP BY department;
```

### Find the top 5 highest-paid employees

```sql
SELECT *
FROM employee
ORDER BY salary DESC
LIMIT 5;
```

### Find employees older than 25

```sql
SELECT *
FROM employee
WHERE TIMESTAMPDIFF(YEAR, dob, CURDATE()) > 25;
```

---

## 📚 Key Learning Outcomes

Through this project, I strengthened my understanding of:

* Writing SQL queries from business requirements.
* Filtering and sorting structured data.
* Performing statistical calculations using aggregate functions.
* Grouping data for department-wise and gender-wise analysis.
* Working with dates in MySQL.
* Using `GROUP BY` and `HAVING` for analytical queries.
* Extracting useful information from an employee dataset.

---

## 📂 Project Structure

```text
Employee-Database/
│
├── 02_Employee.sql
└── README.md
```

---

## 🚀 How to Run the Project

1. Install **MySQL** or open **MySQL Workbench**.
2. Open `02_Employee.sql`.
3. Execute the database and table creation commands.
4. Insert the employee records.
5. Run the SQL queries individually to view the results.

---

## 👩‍💻 Author

**Nafeela Beer**

This project was created as part of my SQL learning journey to gain practical experience in database management and data analysis.

---

## ⭐ Conclusion

The **Employee Database Management System** is a practical SQL project designed to demonstrate how MySQL can be used to store, retrieve, filter, aggregate, and analyze employee data.

It helped me build a stronger foundation in **SQL, MySQL, and data analysis** through hands-on practice.
