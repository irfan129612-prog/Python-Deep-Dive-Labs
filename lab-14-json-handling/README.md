# Lab 14: JSON Handling

## Objective

The objective of this lab is to understand JSON handling in Python by converting dictionaries into JSON format, storing JSON data in files, and reading it back into Python objects.

---

## Lab Environment

| Component        | Details                   |
| ---------------- | ------------------------- |
| Operating System | Ubuntu Linux              |
| Python Version   | Python 3.x                |
| IDE              | PyCharm Community Edition |
| Terminal         | Ubuntu CLI                |

---

## Project Structure

```text
lab-14-json-handling/
│
├── json_handling.py
└── employee_data.json
```

---

## Complete Code

```python
import json

employee_data = {
    "name": "John Doe",
    "age": 30,
    "department": "Engineering",
    "skills": ["Python", "Django", "Machine Learning"]
}

employee_data_json = json.dumps(employee_data, indent=4)

print(employee_data_json)

with open("employee_data.json", "w") as json_file:
    json_file.write(employee_data_json)

with open("employee_data.json", "r") as json_file:
    data = json.load(json_file)

print(data)
```

---

## Output

```text
{
    "name": "John Doe",
    "age": 30,
    "department": "Engineering",
    "skills": [
        "Python",
        "Django",
        "Machine Learning"
    ]
}
```

---

## Key Concepts

### JSON

A lightweight data-interchange format used for storing and transmitting structured data.

### json.dumps()

Converts a Python object into a JSON string.

### json.load()

Reads JSON data from a file and converts it into a Python object.

### JSON File Storage

JSON files are commonly used for configuration settings and data exchange.

---

## Real-World Applications

* REST APIs
* SIEM alerts
* Wazuh events
* Elasticsearch documents
* Configuration files
* Cloud services
* Data exchange between applications

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program output and generated JSON file.

---

## Skills Learned

* Creating Python dictionaries
* Converting dictionaries to JSON
* Writing JSON to files
* Reading JSON from files
* Using the json module
* Understanding data serialization

---

## Conclusion

This lab demonstrated how Python handles JSON data using the built-in json module. Data was successfully converted from a dictionary to JSON, stored in a file, and loaded back into Python. JSON remains one of the most important formats for modern software development and API communication.
