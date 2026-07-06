# 🧪 Lab 38: Parameter Passing & Unpacking

## 📌 Lab Summary

In this lab, Python's flexible parameter passing features were explored using **`*args`** and **`**kwargs`**. Functions were designed to accept a variable number of positional and keyword arguments, while the unpacking operators (`*` and `**`) were used to pass lists and dictionaries as function arguments. These techniques are widely used in Python frameworks, APIs, automation scripts, and reusable software development.

---

## 🎯 Objectives

- Understand flexible parameter passing in Python
- Learn how to use `*args`
- Learn how to use `**kwargs`
- Perform list and dictionary unpacking
- Build reusable and flexible functions

---

## 🛠️ Tools Used

- Ubuntu Linux
- Python 3.x
- PyCharm Community Edition
- Ubuntu Terminal

---

## 🗂️ Lab Environment

| Component | Details |
|----------|---------|
| Operating System | Ubuntu Linux |
| Python Version | Python 3.x |
| IDE | PyCharm Community Edition |
| Programming Language | Python |
| Terminal | Ubuntu CLI |

---

## ✅ Task 1: Create a Function Using `*args`

A function was created to accept any number of positional arguments and calculate their total.

```python
def add_numbers(*args):

    total = 0

    for num in args:
        total += num

    return total
```

### Result

- ✅ Function accepted multiple positional arguments.
- ✅ Sum of all numbers calculated successfully.

---

## ✅ Task 2: Create a Function Using `**kwargs`

A function was created to accept any number of keyword arguments.

```python
def show_info(**kwargs):

    for key, value in kwargs.items():
        print(f"{key}: {value}")
```

### Result

- ✅ Function accepted dynamic keyword arguments.
- ✅ Key-value pairs displayed successfully.

---

## ✅ Task 3: Pass Multiple Positional Arguments

Call the function using individual values.

```python
print(add_numbers(1, 2, 3, 4, 5))
```

### Output

```text
15
```

---

## ✅ Task 4: Pass Keyword Arguments

Call the function using named parameters.

```python
show_info(
    name="Alice",
    age=30,
    city="New York"
)
```

### Output

```text
name: Alice
age: 30
city: New York
```

---

## ✅ Task 5: List Unpacking

Create a list and unpack it using the `*` operator.

```python
numbers = [10, 20, 30, 40]

print(add_numbers(*numbers))
```

### Output

```text
100
```

### Result

- ✅ List unpacked into positional arguments.

---

## ✅ Task 6: Dictionary Unpacking

Create a dictionary and unpack it using the `**` operator.

```python
info = {
    "occupation": "Engineer",
    "country": "USA"
}

show_info(**info)
```

### Output

```text
occupation: Engineer
country: USA
```

### Result

- ✅ Dictionary unpacked into keyword arguments.

---

## 💻 Complete Code

```python
def add_numbers(*args):

    total = 0

    for num in args:
        total += num

    return total


def show_info(**kwargs):

    for key, value in kwargs.items():
        print(f"{key}: {value}")


print(add_numbers(1, 2, 3, 4, 5))

show_info(
    name="Alice",
    age=30,
    city="New York"
)

numbers = [10, 20, 30, 40]

print(add_numbers(*numbers))

info = {
    "occupation": "Engineer",
    "country": "USA"
}

show_info(**info)
```

---

## 💻 Commands Used

```bash
python3 parameter_unpacking.py
```

---

## 📋 Validation

The following tasks were successfully completed:

- ✅ Used `*args` for positional arguments
- ✅ Used `**kwargs` for keyword arguments
- ✅ Performed list unpacking
- ✅ Performed dictionary unpacking
- ✅ Verified expected program output

---

## 📚 Key Concepts

| Concept | Description |
|----------|-------------|
| `*args` | Accepts any number of positional arguments |
| `**kwargs` | Accepts any number of keyword arguments |
| Unpacking | Expands lists or dictionaries into function arguments |
| Positional Arguments | Arguments passed based on their order |
| Keyword Arguments | Arguments passed using parameter names |
| Flexible Functions | Functions capable of handling varying numbers of inputs |

---

## 🌍 Real-World Applications

Flexible parameter passing is commonly used in:

- Web Development
- REST APIs
- Automation Scripts
- Python Frameworks
- Data Science Libraries
- Machine Learning Projects
- Cybersecurity Tools
- Configuration Management

---

## 📸 Screenshots

Include screenshots for:

- Complete Python source code
- Program execution
- Output showing `*args`
- Output showing `**kwargs`
- List unpacking result
- Dictionary unpacking result

---

## 📖 What I Learned

- How to use `*args` to accept multiple positional arguments.
- How to use `**kwargs` to accept dynamic keyword arguments.
- How to unpack lists using the `*` operator.
- How to unpack dictionaries using the `**` operator.
- Why flexible parameter passing improves function reusability and simplifies Python programming.

---

## ✅ Conclusion

This lab demonstrated Python's flexible parameter passing capabilities using **`*args`**, **`**kwargs`**, and the unpacking operators (`*` and `**`). These features enable developers to write reusable and adaptable functions that can handle varying numbers of inputs. Such techniques are widely used in **Python frameworks, automation scripts, APIs, cybersecurity tools, and data science applications**, making them essential skills for professional Python development.
