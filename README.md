# Digital Music Store Data Analysis (SQL)

## 📌 Project Overview
This repository contains an end-to-end SQL portfolio project focused on analyzing a relational database for a digital music store. The objective is to explore, query, and analyze the dataset to extract actionable business insights, evaluate store performance, understand customer behavior, and provide data-driven recommendations for business growth.

The project covers multi-tiered analysis, progressing from beginner-level aggregations to advanced analytical SQL using complex queries.

---

## 🛠️ Tech Stack & Tools
- **Database Management System:** PostgreSQL
- **Interface Tool:** pgAdmin 4
- **Language:** SQL (Structured Query Language)
- **Concepts Used:** Relational databases (RDBMS), data analysis, schema restoration

---

## 📊 Database Schema & Key Concepts
The project uses a music playlist database (`music_database`) with interconnected tables including:
- `employee`
- `customer`
- `invoice`
- `invoice_line`
- `track`
- `mediatype`
- `genre`
- `album`
- `artist`

To solve real-world business problems, the SQL analysis includes:
- **Core functions:** `COUNT`, `SUM`, `AVG`, `GROUP BY`, `ORDER BY`
- **Relational mapping:** `INNER JOIN`, `LEFT JOIN`
- **Advanced SQL:**
  - **CTEs** for readable multi-step query design
  - **Window functions** such as `ROW_NUMBER() OVER (PARTITION BY ...)` for ranking and top-N analysis

---

## 💡 Key Business Questions Addressed

### 🔹 Level 1: Beginner
- Identify the senior-most employee based on job title.
- Find the countries with the most invoices.
- Extract the top 3 invoice totals.
- Determine the city with the highest total revenue.
- Identify the best customer based on total spending.

### 🔹 Level 2: Intermediate
- Retrieve email, first name, last name, and genre of all Rock music listeners.
- Rank artists who have written the most Rock tracks.
- Return tracks with duration longer than the average track length.

### 🔹 Level 3: Advanced
- **Customer spending by artist:** Calculate how much each customer spent on individual artists.
- **Most popular genre per country:** Find top genre(s) in each country by purchases (using CTEs and `ROW_NUMBER()`).
- **Top customer per country:** Determine the highest-spending customer in each country.

---

## 🚀 How to Run This Project

### Prerequisites
- PostgreSQL
- pgAdmin 4

### Execution Steps
1. Create the database:
   ```sql
   CREATE DATABASE music_database;
   ```
2. Restore/import the project schema and data into `music_database` using pgAdmin (Restore) or `psql`.
3. Open the Query Tool in pgAdmin and run the analysis queries.
4. Review result sets to derive business insights and recommendations.
