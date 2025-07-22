# DBMS-Project
Hackathon Management System(PL/SQL + Oracle SQL) 
# 🛠️ Hackathon Management System (PL/SQL + Oracle SQL)

A robust backend system designed to manage users, teams, projects, roles, and evaluation workflows for hackathons. Built using Oracle SQL and PL/SQL to automate core operations and ensure data integrity.

## 📌 Project Overview

This project simulates a real-world hackathon management system using a relational database and procedural logic. It enables organizers to track team participation, assign judges, input scores, and auto-declare winners based on evaluation rules.

## ⚙️ Key Features

- **Relational Database Design**:
  - Normalized tables for users, roles, teams, judges, projects, and scores
  - Foreign key constraints to maintain referential integrity
  - Cascading deletes to handle dependent data

- **PL/SQL Automation**:
  - Procedures for:
    - Inserting users and forming teams
    - Assigning and storing scores
    - Declaring winners based on average or total points
  - Use of loops, conditionals, and exception handling
  - Randomized test data via `DBMS_RANDOM`

- **Dynamic SQL Queries**:
  - Complex joins and subqueries to fetch leaderboard data
  - Aggregation functions for team scoring
  - Flexible filtering using parameters

## 🧪 Sample SQL Snippets

```sql
-- Procedure to insert a new user
BEGIN
  insert_user('John Doe', 'Developer', 'john@example.com');
END;
