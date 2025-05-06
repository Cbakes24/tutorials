# PostgreSQL (psql) Cheat Sheet

## 🔧 Connection & Navigation
```bash
psql -d my_database              # Connect to a specific database
\c another_db                   # Connect to a different database from within psql
\q                              # Quit psql
```

## 🗃️ Database Management
```bash
\l                              # List all databases
CREATE DATABASE dbname;        # Create a new database
DROP DATABASE dbname;          # Delete a database
```

## 📂 Table Management
```bash
\d                              # List all tables
\d table_name                   # Describe a table (schema, columns, etc.)
SELECT * FROM table_name;       # View all data in a table
```

## 📦 Basic Queries
```sql
SELECT column FROM table;               # Select column data
SELECT * FROM table WHERE id = 1;       # Conditional select
INSERT INTO table (col1, col2) VALUES ('val1', 'val2');
UPDATE table SET col = 'val' WHERE id = 1;
DELETE FROM table WHERE id = 1;
```

## 🧱 Schema Stuff
```bash
\dt                             # List all tables
\di                             # List all indexes
\dn                             # List all schemas
```

## 👤 Users and Roles
```bash
\du                             # List users and roles
CREATE USER name WITH PASSWORD 'pass';
GRANT ALL PRIVILEGES ON DATABASE dbname TO name;
```

## 📜 Miscellaneous
```bash
\?                              # Help menu
\h                              # SQL command syntax help (e.g., \h SELECT)
\conninfo                       # Show current connection info
```
