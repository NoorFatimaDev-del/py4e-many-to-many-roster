Multi-Entity Student Roster Database System
📌 Project Overview
This project demonstrates a robust data pipeline that parses complex student enrollment data from JSON format into a fully normalized SQLite Relational Database. The core achievement is modeling a Many-to-Many relationship using industry-standard schema design.

🛠️ Technical Stack
Language: Python 3.x

Database Engine: SQLite3

Data Interchange: JSON

Architecture: Relational Database Management (RDBMS)

🏗️ Database Architecture
To ensure data integrity and eliminate redundancy, the system utilizes a three-table structure:

User Table: Unique student records.

Course Table: Unique academic course titles.

Member Table (Junction): Connects users and courses with assigned roles.

🚀 Key Features
Data Normalization: Successfully resolved many-to-many complexities into two one-to-many relationships.

Efficient Logic: Implemented INSERT OR IGNORE and UNIQUE constraints to maintain a clean dataset.

Advanced Querying: Employs multi-table JOIN statements to reconstruct and report on interconnected data.

📊 Sample SQL Query
The following logic was used to extract the relationship data for verification:

SQL
SELECT User.name, Course.title, Member.role 
FROM User JOIN Member JOIN Course 
ON User.id = Member.user_id AND Member.course_id = Course.id
ORDER BY User.name DESC;
