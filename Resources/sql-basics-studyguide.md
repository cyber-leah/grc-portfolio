
# 🧠 SQL Basics Cheat Sheet

Welcome to your SQL basics guide! This Markdown file is designed to help you refresh and build confidence with common SQL commands and concepts.

---

## 📌 What is SQL?
**SQL (Structured Query Language)** is used to interact with relational databases. It allows you to retrieve, insert, update, and delete data.

---

## 🔍 SELECT – Retrieve Data

```sql
SELECT column1, column2
FROM table_name;
```

**Example:**
```sql
SELECT first_name, last_name
FROM employees;
```

---

## 🎯 WHERE – Filter Data

```sql
SELECT column1
FROM table_name
WHERE condition;
```

**Example:**
```sql
SELECT * 
FROM customers
WHERE state = 'NC';
```

---

## 🔢 ORDER BY – Sort Results

```sql
SELECT *
FROM table_name
ORDER BY column_name ASC|DESC;
```

**Example:**
```sql
SELECT name, signup_date
FROM users
ORDER BY signup_date DESC;
```

---

## #️⃣ COUNT – Count Records

```sql
SELECT COUNT(*)
FROM table_name
WHERE condition;
```

**Example:**
```sql
SELECT COUNT(*)
FROM transactions
WHERE status = 'Pending';
```

---

## 🎛️ LIMIT – Limit Results

```sql
SELECT *
FROM table_name
LIMIT number;
```

**Example:**
```sql
SELECT *
FROM products
LIMIT 5;
```

---

## 🔄 Common Clauses Recap
- `SELECT` → Choose which columns to retrieve
- `FROM` → Specify the table
- `WHERE` → Filter rows
- `ORDER BY` → Sort results
- `COUNT()` → Count the number of rows
- `LIMIT` → Limit how many rows return

---

## ✅ Bonus Tips
- SQL is **not case sensitive**, but it’s common to capitalize commands.
- Always end SQL commands with a **semicolon (;)**.
- Use **single quotes** around text values (`'NC'`, `'Pending'`).

---

_This file is a quick-reference guide. You can add examples from your own learning or use this to build simple practice challenges for yourself!_
