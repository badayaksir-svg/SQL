# SQL University Database Project

This repository contains a simple **University Database** project built using **MySQL**.  
It is designed for learning and practicing **SQL**, **database design**, and **Docker-based database setup**.

---

## 📌 Features

- University database schema (students, courses, departments, enrollments, etc.)
- Sample data for testing SQL queries
- Verification queries to validate database structure and data
- Docker & Docker Compose support for easy setup
- Suitable for beginners and academic use

---

## 📁 Project Structure

SQL/
├── sql/
│ ├── 01_schema.sql # Database tables and constraints
│ ├── 02_data.sql # Sample data insertion
│ └── 03_verify.sql # Verification queries
├── docker-compose.yml # Docker configuration for MySQL
└── README.md # Project documentation


---

## 🧰 Requirements

- Docker  
- Docker Compose  

Make sure Docker is installed and running on your system.

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/badayaksir-svg/SQL.git
cd SQL
2️⃣ Start MySQL Using Docker
docker-compose up -d
This will:

Start a MySQL 8.0 container

Create the university_db database

Automatically run all SQL files in the sql/ folder

🔐 Database Credentials
Host: localhost
Port: 3303
Username: root
Password: root
Database: university_db
You can connect using:

MySQL Workbench

Command line

VS Code SQL extensions

✅ Verify the Database
Run the queries in:

sql/03_verify.sql
These queries help confirm that tables and data are correctly created.

🛑 Stop the Container
docker-compose down
📚 Learning Purpose
This project is ideal for:

SQL practice

Database normalization

Academic assignments

Understanding Docker + MySQL integration

