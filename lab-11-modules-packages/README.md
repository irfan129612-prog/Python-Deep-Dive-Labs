# Lab 11: Modules & Packages

## Objective

The objective of this lab is to understand Python modules and packages, and learn how to organize reusable code across multiple files.

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
lab-11-modules-packages/
│
├── main.py
│
└── mypackage/
    ├── __init__.py
    └── mymodule.py
```

---

## mymodule.py

```python
def add(a, b):
    return a + b
```

---

## main.py

```python
from mypackage import mymodule

result = mymodule.add(5, 3)

print(f"The sum of 5 and 3 is {result}")
```

---

## Output

```text
The sum of 5 and 3 is 8
```

---

## Key Concepts

### Module

A Python file containing functions, variables, or classes.

Example:

```text
mymodule.py
```

### Package

A directory containing multiple modules.

Example:

```text
mypackage/
```

### **init**.py

Marks a directory as a Python package.

### Importing Modules

```python
from mypackage import mymodule
```

### Using Functions from Modules

```python
mymodule.add(5, 3)
```

---

## Real-World Applications

* Large Python projects
* Data Science libraries
* Automation frameworks
* Web applications
* SIEM and security tools
* API development

---

## Screenshots

### Screenshot 1

Project structure and source code.

### Screenshot 2

Program execution and output.

---

## Skills Learned

* Creating modules
* Creating packages
* Importing modules
* Organizing code
* Reusing functions
* Understanding project structure

---

## Conclusion

This lab demonstrated how Python modules and packages help organize code into reusable and maintainable components. Proper use of modules and packages is essential when building scalable applications and automation projects.
