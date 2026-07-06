# 🧪 Lab 39: Python Style & PEP 8 Checks

## 📌 Lab Summary

In this lab, Python coding standards were explored using the **PEP 8 Style Guide**. Popular tools including **flake8**, **black**, and **autopep8** were installed and used to identify style violations, automatically format code, and improve overall readability. Following PEP 8 standards helps developers write clean, consistent, and maintainable Python code.

---

## 🎯 Objectives

- Understand the Python PEP 8 style guide
- Identify coding style violations using `flake8`
- Automatically format Python code using `black`
- Fix PEP 8 issues using `autopep8`
- Improve code readability and maintainability

---

## 🛠️ Tools Used

- Ubuntu Linux
- Python 3.x
- PyCharm Community Edition
- flake8
- black
- autopep8
- Ubuntu Terminal

---

## 🗂️ Lab Environment

| Component | Details |
|----------|---------|
| Operating System | Ubuntu Linux |
| Python Version | Python 3.x |
| IDE | PyCharm Community Edition |
| Style Guide | PEP 8 |
| Terminal | Ubuntu CLI |

---

## ✅ Task 1: Create Sample Python Code

A Python script containing several PEP 8 style violations was created.

### Example Code

```python
def exampleFunction():
    x = {'key': 42, 'another_key': 23}

    if(x['key'] > 0):
        print("Positive number")
    else:
        print("Zero or Negative")
```

### Result

- ✅ Sample code prepared for style checking.

---

## ✅ Task 2: Install flake8

Install the **flake8** linter.

```bash
pip3 install flake8 --break-system-packages
```

### Run flake8

```bash
flake8 example.py
```

### Result

- ✅ Style violations were identified successfully.

---

## ✅ Task 3: Install and Run Black

Install the **Black** code formatter.

```bash
pip3 install black --break-system-packages
```

Format the Python file.

```bash
black example.py
```

### Result

- ✅ Code formatted automatically according to Black's style conventions.

---

## ✅ Task 4: Install and Run autopep8

Install **autopep8**.

```bash
pip3 install autopep8 --break-system-packages
```

Automatically fix PEP 8 violations.

```bash
autopep8 --in-place --aggressive --aggressive example.py
```

### Result

- ✅ PEP 8 issues corrected automatically.

---

## 💻 Commands Used

### Install flake8

```bash
pip3 install flake8 --break-system-packages
```

### Check Code Style

```bash
flake8 example.py
```

### Install Black

```bash
pip3 install black --break-system-packages
```

### Format Code

```bash
black example.py
```

### Install autopep8

```bash
pip3 install autopep8 --break-system-packages
```

### Auto Format

```bash
autopep8 --in-place --aggressive --aggressive example.py
```

---

## 📋 Validation

The following tasks were successfully completed:

- ✅ Installed `flake8`
- ✅ Detected coding style violations
- ✅ Installed `black`
- ✅ Automatically formatted the source code
- ✅ Installed `autopep8`
- ✅ Corrected PEP 8 violations
- ✅ Improved overall code readability

---

## 📚 Key Concepts

| Concept | Description |
|----------|-------------|
| PEP 8 | Official Python style guide for writing clean and consistent code |
| flake8 | Linter that checks code quality, syntax errors, and style violations |
| black | Opinionated Python code formatter that automatically formats code |
| autopep8 | Tool that automatically fixes PEP 8 style violations |
| Code Linting | The process of analyzing code to detect programming and style issues |
| Code Formatting | Automatically restructuring source code to follow style guidelines |

---

## 🌍 Benefits of Following PEP 8

Following Python coding standards provides several advantages:

- Better Code Readability
- Easier Maintenance
- Improved Team Collaboration
- Professional Code Quality
- Consistent Coding Style
- Reduced Style-Related Issues

---

## 🌍 Real-World Applications

PEP 8 compliance is essential in:

- Software Development
- Open Source Projects
- Python Frameworks
- Automation Scripts
- Data Science
- Machine Learning
- Cybersecurity Tools
- DevOps Projects

---

## 📸 Screenshots

Include screenshots for:

- Python source code before formatting
- Python source code after formatting
- flake8 terminal output
- Black formatting output
- autopep8 formatting output

---

## 📖 What I Learned

- How to apply Python's official PEP 8 coding standards.
- How to detect style violations using `flake8`.
- How to automatically format Python code using `black`.
- How to fix PEP 8 issues using `autopep8`.
- Why maintaining consistent coding standards improves software quality and collaboration.

---

## ✅ Conclusion

This lab demonstrated how to write cleaner, more maintainable Python code by following the **PEP 8** style guide. Using tools such as **flake8**, **black**, and **autopep8**, coding style violations were identified and corrected automatically. Adhering to these standards enhances **code readability, maintainability, and collaboration**, making them an essential part of professional Python development.
