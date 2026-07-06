# Lab 30: Basic SQLite Usage

## Objective

The objective of this lab is to understand SQLite database operations in Python, including creating tables, inserting records, querying data, and displaying results.

---

## Lab Environment

| Component        | Details                   |
| ---------------- | ------------------------- |
| Operating System | Ubuntu Linux              |
| Python Version   | Python 3.x                |
| IDE              | PyCharm Community Edition |
| Terminal         | Ubuntu CLI                |

---

## Complete Code

```python
import sqlite3

connection = sqlite3.connect(":memory:")

cursor = connection.cursor()

cursor.execute("""
CREATE TABLE students (
    id INTEGER PRIMARY KEY,
    name TEXT NOT NULL,
    grade REAL
)
""")

students_data = [
    (1, "Alice", 85.5),
    (2, "Bob", 78.0),
    (3, "Charlie", 92.0)
]

cursor.executemany(
    "INSERT INTO students VALUES (?, ?, ?)",
    students_data
)

connection.commit()

cursor.execute("SELECT * FROM students")

results = cursor.fetchall()

for row in results:
    print(row)

connection.close()
```

---

## Output

```text
(1, 'Alice', 85.5)
(2, 'Bob', 78.0)
(3, 'Charlie', 92.0)
```

---

## Key Concepts

### SQLite

A lightweight embedded relational database.

### Connection

Used to connect Python with the database.

```python
sqlite3.connect()
```

### Cursor

Executes SQL commands and retrieves results.

### CREATE TABLE

Creates a database table.

### INSERT

Adds records into a table.

### SELECT

Retrieves data from a table.

### fetchall()

Returns all query results.

### commit()

Saves database changes.

---

## SQL Commands Used

```sql
CREATE TABLE
INSERT INTO
SELECT *
```

---

## Real-World Applications

* Student management systems
* Inventory systems
* Log storage
* SIEM alerts
* Security monitoring
* Local application databases

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program output.

---

## Skills Learned

* Connecting to SQLite
* Creating tables
* Inserting records
* Querying databases
* Fetching results
* Understanding SQL basics

---

## Conclusion

This lab demonstrated the basic use of SQLite in Python. By creating a table, inserting records, and retrieving data, students gained practical experience in database operations that form the foundation for larger data-driven applications.
