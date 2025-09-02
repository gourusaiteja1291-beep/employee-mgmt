# Employee Management System – SQL

This folder contains the *SQL scripts* for the Employee Management System project.  
The database is hosted on *AWS RDS (MySQL)* and is used by the Spring Boot application.

---

## 📂 Project Structure

- *schema.sql* → Creates tables (departments, employees)
- *seed.sql* → Inserts sample data
- *queries.sql* → Example queries for practice
- *procedures_triggers_views.sql* → Views, Stored Procedures, and Triggers
- *snapshots_notes.md* → Notes & screenshots

---

## 🗄 Database Details (AWS RDS)

- *Endpoint* → emsdb.c3u0oo68mhn7.ap-south-1.rds.amazonaws.com  
- *Port* → 3306  
- *Database Name* → ems  
 

---

## ⚡ How to Run

1. Connect to the RDS instance using *MySQL Workbench* or CLI.  
2. Run the following in order:
   - schema.sql → create schema & tables
   - seed.sql → insert sample data
   - queries.sql → test queries
   - procedures_triggers_views.sql → enable views, triggers & procedures
3. Verify using:
   ```sql
   SELECT e.emp_id, e.full_name, d.dept_name, e.salary
   FROM employees e
   JOIN departments d ON e.dept_id = d.dept_id;

Author
Gouru Sai Teja
gourusaiteja1291@gmail.com

