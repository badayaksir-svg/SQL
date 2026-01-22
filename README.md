University Database SQL Example
This repository provides a simple example of a university database setup using MySQL. It includes SQL scripts for creating the database schema, inserting sample data, and verifying the data through a query. A Docker Compose configuration is provided to easily spin up a MySQL instance and initialize the database with the provided scripts.
Purpose
The project demonstrates basic database design for a university system, including tables for majors, students, courses, and enrollments. It's useful for learning SQL, database normalization, and Docker-based database deployment.
Prerequisites

Docker and Docker Compose installed on your system.

Setup and Usage

Clone the repository:textgit clone https://github.com/badayaksir-svg/SQL.git
cd SQL
Start the MySQL container using Docker Compose:textdocker-compose up -dThis will:
Pull the MySQL 8.0 image.
Create a container named university_db.
Map port 3303 on the host to 3306 in the container.
Mount the ./sql directory to /docker-entrypoint-initdb.d in the container, which automatically executes the SQL scripts in alphabetical order (01_schema.sql, 02_data.sql, 03_verify.sql).

Connect to the database:
Use a MySQL client (e.g., MySQL Workbench, command-line mysql).
Host: localhost
Port: 3303
Username: root
Password: root
Database: university_db

Verify the data:
Run the query from 03_verify.sql to see joined data from all tables.

Stop the container:textdocker-compose down# SQL
