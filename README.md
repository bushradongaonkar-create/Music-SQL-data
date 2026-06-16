# Digital Music Store Data Analysis (SQL)

## 📌 Project Overview
This repository contains an end-to-end SQL portfolio project focused on analyzing a relational database for a digital music store. The objective of this project is to explore, query, and analyze the dataset to extract actionable business insights, evaluate store performance, understand customer behavior, and ultimately provide data-driven recommendations for business growth.

The project covers a multi-tiered analysis, tackling data challenges that progress from beginner-level aggregations to advanced analytical data manipulation using complex queries.

---

## 🛠️ Tech Stack & Tools
* **Database Management System:** PostgreSQL
* **Interface Tool:** pgAdmin 4
* **Language:** SQL (Structured Query Language)
* **Concepts Used:** Relational Databases (RDBMS), Data Analysis, Schema Restorations.

---

## 📊 Database Schema & Key Concepts
The project utilizes a music playlist database (`music_database`) containing multiple interconnected tables including `employee`, `customer`, `invoice`, `invoice_line`, `track`, `mediatype`, `genre`, `album`, and `artist`. 

To solve real-world business problems, the queries in this repository leverage:
* **Core Functions:** Aggregations (`COUNT`, `SUM`, `AVG`), Grouping (`GROUP BY`), and Ordering (`ORDER BY`).
* **Relational Mapping:** Joins (`INNER JOIN`, `LEFT JOIN`) across multiple tables to consolidate normalized data.
* **Advanced Analytical SQL:** 
  * **Common Table Expressions (CTEs):** To break down complex multi-stage problems into clean, readable sequential blocks.
  * **Window Functions:** Utilizing clauses like `ROW_NUMBER()` combined with `OVER (PARTITION BY ...)` to perform sophisticated data ranking and filtering without collapsing rows.

---

## 💡 Key Business Questions Addressed

### 🔹 Level 1: Beginner
* Identifying the senior-most employee based on job title to map internal organizational hierarchy.
* Finding the countries with the most invoices to pinpoint top geographic revenue streams.
* Extracting the top 3 values of total invoices to observe peak purchase behaviors.
* Determining the city that generates the highest revenue to optimize local promotional events.
* Identifying the best customer (the one who has spent the most money overall) to launch targeted VIP loyalty campaigns.

### 🔹 Level 2: Intermediate
* Querying the email, first name, last name, and genre of all Rock Music listeners to curate dedicated marketing email blasts.
* Inviting the artists who have written the most rock music in our dataset by ranking them based on overall track count.
* Returning all track names that have a song length longer than the average song length to optimize playlist curation strategies.

### 🔹 Level 3: Advanced
* **Customer Spending by Artist:** Finding how much money each customer spent on individual artists.
* **Most Popular Genre per Country:** Determining the top music genre for each country based on the highest number of purchases (using `ROW_NUMBER()` and CTEs to handle ties gracefully).
* **Top Customer per Country:** Writing a query that determines the customer that has spent the most money for each country.

---

## 🚀 How to Run This Project

### Prerequisite
Ensure you have **PostgreSQL** and **pgAdmin** installed on your local machine.

### Execution Steps
1. **Create the Database:** Open pgAdmin, open the Query Tool, and run:
```sql
   CREATE DATABASE music_database;
