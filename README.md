Student Roster Many-to-Many Database System
📌 Project Overview
This project demonstrates the implementation of a Many-to-Many relationship using Python and SQLite. The application parses complex student enrollment data from a JSON format and structures it into a relational database with optimized normalization.

🛠️ Technical Features
JSON Parsing: Extracts user, course, and role data from nested JSON structures.

Database Schema: Implements three tables: User, Course, and a junction table Member.

Relational Logic: Models Many-to-Many relationships where multiple students can be enrolled in multiple courses.

Data Integrity: Utilizes INSERT OR IGNORE and UNIQUE constraints to prevent data duplication.

SQL Mastery: Features complex JOIN queries to reconstruct relationships for reporting.

📁 Database Schema
The system follows a normalized relational structure:

User Table: Stores unique student names.

Course Table: Stores unique course titles.

Member Table (Junction): Links Users and Courses while storing the specific role (Student/Instructor) for that relationship.

🚀 How to Run
Clone the repository:

Bash
git clone https://github.com/your-username/your-repo-name.git
Ensure you have the data file: Place roster_data.json in the project directory.

Execute the script:

Bash
python roster.py
View Results: Open rosterdb.sqlite in any SQLite browser to view the populated tables.

🎓 Learning Outcomes
This project was completed as part of the Using Databases with Python course by the University of Michigan. It highlights my ability to bridge the gap between Python scripting and relational database management systems (RDBMS).
