<h1>A database is an organized collection of information that is stored electronically so it can be easily accessed, managed, updated, and searched</h1><br>
<img width="2059" height="1302" alt="Difference_R-NR@4x-8" src="https://github.com/user-attachments/assets/6b260183-5169-4fdc-bac9-0c545a08ae55" />

## Relational Databases (SQL)

Relational databases store data in **tables** consisting of rows and columns. Relationships between tables are created using **primary keys** and **foreign keys**. They are ideal for structured data and support **SQL (Structured Query Language)** for querying and managing data.

### Popular Relational Databases

- **MySQL** – Open-source relational database widely used for web applications.
- **PostgreSQL** – Advanced open-source relational database with powerful features and standards compliance.
- **Microsoft SQL Server** – Enterprise-grade relational database developed by Microsoft.
- **Oracle Database** – High-performance commercial relational database commonly used in large enterprises.

---

## Non-relational Databases (NoSQL)

Non-relational databases (NoSQL) do not store data in fixed tables. Instead, they use flexible data models such as documents, key-value pairs, columns, or graphs. They are designed for scalability, high performance, and handling unstructured or semi-structured data.

### Popular Non-relational Databases

- **MongoDB** *(Document Database)* – Stores data as JSON-like documents.
- **Redis** *(Key-Value Database)* – Stores data as key-value pairs for extremely fast access.
- **Apache Cassandra** *(Column-Family Database)* – Optimized for large-scale distributed data storage.
- **Neo4j** *(Graph Database)* – Stores data as nodes and relationships, ideal for connected data such as social networks and recommendation systems.

# What is a Query?

A **query** is a request sent to a database to **retrieve, insert, update, or delete data**. It is the primary way users and applications interact with a database.

Think of a query as asking the database a question or giving it an instruction.

CRUD (CREATE, READ, UPDATE, DELETE)

<img width="743" height="413" alt="images" src="https://github.com/user-attachments/assets/01da2eee-ea83-4151-b6ca-a8ce1c2de0b3" />

# SQL for Data Analytics: A Quick-Start Guide

Welcome to this repository! This guide provides a foundational roadmap for using SQL to perform data analysis. 

## 🚀 The Analytics Workflow
Data analysis in SQL typically follows this logical flow:

1. **Extract** (SELECT)
2. **Filter** (WHERE)
3. **Aggregate** (GROUP BY)
4. **Combine** (JOIN)
5. **Analyze** (WINDOW FUNCTIONS)

---

## 1. Extracting Data
The `SELECT` statement is your primary tool for retrieving data.

sql
```SELECT 
    customer_id, 
    order_date, 
    total_amount
FROM orders
LIMIT 10;

## 2. Filtering & Cleaning
The `WHERE` statement is for narrow down statement.

```SELECT *
FROM orders
WHERE status = 'Completed' 
  AND order_date >= '2026-01-01';
