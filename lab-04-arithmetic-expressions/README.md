# Lab 04: Arithmetic & Expressions

## Objective

The objective of this lab is to perform basic arithmetic operations using Python and understand the difference between integer division and floating-point division.

---

## Lab Environment

| Component        | Details                   |
| ---------------- | ------------------------- |
| Operating System | Ubuntu Linux              |
| Python Version   | Python 3.x                |
| IDE              | PyCharm Community Edition |
| Terminal         | Ubuntu CLI                |

---

## Task 1: Basic Arithmetic Operations

### Code

```python
number1 = int(input("Enter the first number: "))
number2 = int(input("Enter the second number: "))

addition_result = number1 + number2
subtraction_result = number1 - number2
multiplication_result = number1 * number2
division_result = number1 / number2

print(f"Addition: {number1} + {number2} = {addition_result}")
print(f"Subtraction: {number1} - {number2} = {subtraction_result}")
print(f"Multiplication: {number1} * {number2} = {multiplication_result}")
print(f"Division: {number1} / {number2} = {division_result}")
```

### Example Output

```text
Addition: 20 + 5 = 25
Subtraction: 20 - 5 = 15
Multiplication: 20 * 5 = 100
Division: 20 / 5 = 4.0
```

---

## Task 2: Integer Division vs Float Division

### Code

```python
integer_division_result = number1 // number2
float_division_result = number1 / number2

print(f"Integer Division: {number1} // {number2} = {integer_division_result}")
print(f"Float Division: {number1} / {number2} = {float_division_result}")
```

### Example Output

```text
Integer Division: 10 // 3 = 3
Float Division: 10 / 3 = 3.3333333333333335
```

---

## Understanding the Code

### input()

Used to receive data from the user.

### int()

Converts string input into an integer.

### Arithmetic Operators

| Operator | Purpose          |
| -------- | ---------------- |
| +        | Addition         |
| -        | Subtraction      |
| *        | Multiplication   |
| /        | Float Division   |
| //       | Integer Division |

### f-Strings

Used to embed variables inside strings for cleaner output formatting.

---

## Screenshots

### Screenshot 1

Creating the arithmetic_operations.py script.

### Screenshot 2

Executing the program from Ubuntu terminal.

### Screenshot 3

Results of addition, subtraction, multiplication, and division.

### Screenshot 4

Comparison between integer division and float division.

---

## Skills Learned

* Taking user input
* Converting data types using int()
* Performing arithmetic calculations
* Using f-strings
* Understanding integer division
* Understanding floating-point division

---

## Conclusion

This lab demonstrated how arithmetic expressions are implemented in Python. User input was collected, converted to integers, and processed through various arithmetic operations. The distinction between integer division and floating-point division was explored to strengthen understanding of Python's numerical behavior.
