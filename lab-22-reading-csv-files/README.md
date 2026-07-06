# Lab 22: Reading CSV Files

## Objective

The objective of this lab is to understand how to read CSV files in Python using the built-in csv module, handle headers, and store data in structured formats such as dictionaries.

---

## Lab Environment

| Component        | Details                   |
| ---------------- | ------------------------- |
| Operating System | Ubuntu Linux              |
| Python Version   | Python 3.x                |
| IDE              | PyCharm Community Edition |
| Terminal         | Ubuntu CLI                |

---

## Sample CSV File

```csv
Name,Age,City
Alice,25,New York
Bob,30,London
Charlie,28,Toronto
```

---

## Complete Code

```python
import csv

file_path = "sample.csv"

print("=== Reading CSV Rows ===")

with open(file_path, mode="r") as file:
    csv_reader = csv.reader(file)

    for row in csv_reader:
        print(row)

print("\n=== Skipping Header ===")

with open(file_path, mode="r") as file:
    csv_reader = csv.reader(file)

    header = next(csv_reader)

    for row in csv_reader:
        print(row)

print("\n=== CSV as Dictionary ===")

data_list = []

with open(file_path, mode="r") as file:
    csv_reader = csv.DictReader(file)

    for row in csv_reader:
        data_list.append(row)

for item in data_list:
    print(item)
```

---

## Output

```text
['Name', 'Age', 'City']
['Alice', '25', 'New York']
['Bob', '30', 'London']
['Charlie', '28', 'Toronto']

{'Name': 'Alice', 'Age': '25', 'City': 'New York'}
{'Name': 'Bob', 'Age': '30', 'City': 'London'}
{'Name': 'Charlie', 'Age': '28', 'City': 'Toronto'}
```

---

## Key Concepts

### CSV

A text-based format used to store tabular data.

### csv.reader()

Reads CSV rows as lists.

### next()

Used to skip header rows.

### csv.DictReader()

Reads CSV rows as dictionaries using column headers as keys.

---

## Real-World Applications

* Data Science datasets
* Excel exports
* Log analysis
* SIEM reports
* Security scan results
* ETL pipelines

---

## Screenshots

### Screenshot 1

Sample CSV file and Python code.

### Screenshot 2

Program output.

---

## Skills Learned

* Importing the csv module
* Reading CSV files
* Handling headers
* Using csv.reader()
* Using csv.DictReader()
* Storing CSV data in dictionaries

---

## Conclusion

This lab demonstrated how Python's csv module can be used to efficiently read and process CSV files. Understanding CSV handling is essential for Data Science, automation, reporting, and cybersecurity-related data processing tasks.
