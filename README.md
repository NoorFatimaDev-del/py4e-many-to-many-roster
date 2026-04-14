# Relational Database Automation (Student Roster)

## 📌 Project Overview
This project demonstrates an **ETL (Extract, Transform, Load)** process using Python and SQLite to manage complex relationships. It automates the transformation of a flat JSON data source into a **Many-to-Many normalized relational database** involving students, courses, and roles.

## 🛠️ Technical Features
* **Many-to-Many Modeling:** Implements a junction table (`Member`) to bridge the relationship between `User` and `Course` tables.
* **Data Integrity:** Utilizes `UNIQUE` constraints and `INSERT OR IGNORE` logic to ensure data consistency and prevent duplicate records.
* **Normalization:** Separates entities into distinct tables to minimize redundancy and optimize storage.
* **SQL Mastery:** Features complex multi-table `JOIN` queries to reconstruct and retrieve interconnected data.

## 🚀 How to Run
1. Ensure you have the `roster_data.json` file in the same directory.
2. Run the script using Python: `python roster.py`.
3. The script will generate a `rosterdb.sqlite` file automatically.

## 📊 Database Schema
The database consists of three primary tables:
* **User:** Stores student names with unique constraints.
* **Course:** Stores course titles with unique constraints.
* **Member:** The junction table storing `user_id`, `course_id`, and the student's `role`.
