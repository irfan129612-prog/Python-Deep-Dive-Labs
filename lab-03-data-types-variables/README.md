# Lab 03: Data Types & Variables

## Objective

The objective of this lab is to understand Python variables, data types, and type casting techniques. The lab demonstrates how data is stored, manipulated, and converted between different formats.

---

## Lab Environment

| Component        | Details                   |
| ---------------- | ------------------------- |
| Operating System | Ubuntu Linux              |
| Python Version   | Python 3.x                |
| IDE              | PyCharm Community Edition |
| Terminal         | Ubuntu CLI                |

---

## Task 1: Creating Variables

### Code

```python
name = "John Doe"
age = 25
is_student = True
height = 175.5

print("Name:", name, "Type:", type(name))
print("Age:", age, "Type:", type(age))
print("Is Student:", is_student, "Type:", type(is_student))
print("Height:", height, "Type:", type(height))
```

### Output

```text
Name: John Doe Type: <class 'str'>
Age: 25 Type: <class 'int'>
Is Student: True Type: <class 'bool'>
Height: 175.5 Type: <class 'float'>
```

---

## Task 2: Implicit Type Casting

### Code

```python
a = 10
b = 10.5

result = a + b

print("Result:", result)
print("Type:", type(result))
```

### Output

```text
Result: 20.5
Type: <class 'float'>
```

---

## Task 3: Explicit Type Casting

### Integer to String

```python
age = 25
age_str = str(age)

print(age_str)
print(type(age_str))
```

### String to Integer

```python
number_str = "100"

number_int = int(number_str)

print(number_int)
print(type(number_int))
```

---

## Task 4: Customer Data Intake Case Study

### Code

```python
customer_name = "Alice Johnson"
customer_age = "30"
customer_membership = "True"

customer_age = int(customer_age)

customer_membership = customer_membership == "True"

print("Customer Name:", customer_name)
print("Customer Age:", customer_age)
print("Customer Membership Status:", customer_membership)
```

### Output

```text
Customer Name: Alice Johnson
Customer Age: 30
Customer Membership Status: True
```

---

## Key Concepts Learned

* Variables
* String Data Type
* Integer Data Type
* Float Data Type
* Boolean Data Type
* type() Function
* Implicit Type Casting
* Explicit Type Casting
* Data Validation

---

## Screenshots

### Screenshot 1

Creating variables of different data types.

### Screenshot 2

Output showing variable types using type().

### Screenshot 3

Implicit casting example.

### Screenshot 4

Customer data intake case study output.

---

## Conclusion

This lab introduced Python variables and fundamental data types. Both implicit and explicit type casting were explored, demonstrating how data can be converted and validated. These concepts form the foundation for data processing, automation, cybersecurity scripting, and data science applications.
