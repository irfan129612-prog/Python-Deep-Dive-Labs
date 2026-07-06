# Lab 21: List & Dictionary Comprehensions

## Objective

The objective of this lab is to understand list comprehensions and dictionary comprehensions in Python and learn how they simplify data creation and transformation tasks.

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
# List Comprehension
squares = [x**2 for x in range(10)]

print("Squares:", squares)

# Dictionary Comprehension
words = ["apple", "banana", "cherry", "date"]

lengths = {word: len(word) for word in words}

print("Word Lengths:", lengths)

# Traditional Loop Example
squares_loop = []

for x in range(10):
    squares_loop.append(x**2)

print("Squares using Loop:", squares_loop)
```

---

## Output

```text
Squares: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]

Word Lengths: {'apple': 5, 'banana': 6, 'cherry': 6, 'date': 4}

Squares using Loop: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
```

---

## Key Concepts

### List Comprehension

Creates a list in a single line.

```python
[x**2 for x in range(10)]
```

### Dictionary Comprehension

Creates a dictionary in a single line.

```python
{word: len(word) for word in words}
```

### Advantages

* Shorter code
* Better readability
* Faster execution
* Useful for data transformations

---

## Real-World Applications

* Data cleaning
* Data transformation
* Feature engineering
* Log processing
* Automation scripts
* Cybersecurity reporting

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program output.

---

## Skills Learned

* Creating list comprehensions
* Creating dictionary comprehensions
* Replacing loops with concise syntax
* Transforming data efficiently
* Improving code readability

---

## Conclusion

This lab demonstrated how comprehensions provide a concise and efficient way to create lists and dictionaries. They are widely used in Data Science, Automation, and Python development to simplify repetitive data transformation tasks.
