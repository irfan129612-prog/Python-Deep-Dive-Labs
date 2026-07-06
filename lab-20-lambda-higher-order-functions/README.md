# Lab 20: Using Lambda & Higher-Order Functions

## Objective

The objective of this lab is to understand lambda functions and use them with higher-order functions such as map(), filter(), and reduce().

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
from functools import reduce

numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

doubled_numbers = list(map(lambda x: x * 2, numbers))
print("Doubled Numbers:", doubled_numbers)

even_numbers = list(filter(lambda x: x % 2 == 0, numbers))
print("Even Numbers:", even_numbers)

total_sum = reduce(lambda x, y: x + y, numbers)
print("Sum of Numbers:", total_sum)
```

---

## Output

```text
Doubled Numbers: [2, 4, 6, 8, 10, 12, 14, 16, 18, 20]

Even Numbers: [2, 4, 6, 8, 10]

Sum of Numbers: 55
```

---

## Key Concepts

### Lambda Function

An anonymous function written in a single line.

Example:

```python
lambda x: x * 2
```

### map()

Applies a function to every element of an iterable.

### filter()

Returns elements that satisfy a condition.

### reduce()

Reduces a sequence into a single value.

---

## Real-World Applications

* Data cleaning
* Data transformation
* ETL pipelines
* Log processing
* Cybersecurity automation
* Data Science workflows

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program output.

---

## Skills Learned

* Creating lambda functions
* Using map()
* Using filter()
* Using reduce()
* Functional programming concepts
* Data transformation techniques

---

## Conclusion

This lab demonstrated how lambda functions can be combined with higher-order functions to write concise and efficient Python code. These techniques are commonly used in Data Science, Automation, and Data Processing applications.
