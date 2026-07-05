# Lab 05: Understanding Conditionals (if, elif, else)

## Objective

The objective of this lab is to understand conditional logic in Python using if, elif, and else statements. These constructs allow programs to make decisions based on specific conditions.

---

## Lab Environment

| Component        | Details                   |
| ---------------- | ------------------------- |
| Operating System | Ubuntu Linux              |
| Python Version   | Python 3.x                |
| IDE              | PyCharm Community Edition |
| Terminal         | Ubuntu CLI                |

---

## Task 1: Number Classification

### Code

```python
number = float(input("Enter a number: "))

if number > 0:
    print("Positive")

elif number < 0:
    print("Negative")

else:
    print("Zero")
```

### Example Output

```text
Enter a number: 15
Positive
```

```text
Enter a number: -5
Negative
```

```text
Enter a number: 0
Zero
```

---

## Task 2: Grade Classification

### Code

```python
score = int(input("Enter your score: "))

if score >= 90:
    print("Grade: A")

elif score >= 80:
    print("Grade: B")

elif score >= 70:
    print("Grade: C")

elif score >= 60:
    print("Grade: D")

else:
    print("Grade: F")
```

### Example Output

```text
Enter your score: 85
Grade: B
```

---

## Understanding the Code

### if

Executes code when a condition evaluates to True.

### elif

Checks additional conditions when previous conditions are False.

### else

Executes when all previous conditions are False.

### Comparison Operators

| Operator | Meaning                  |
| -------- | ------------------------ |
| >        | Greater Than             |
| <        | Less Than                |
| >=       | Greater Than or Equal To |
| <=       | Less Than or Equal To    |
| ==       | Equal To                 |
| !=       | Not Equal To             |

---

## Real-World Applications

* Login authentication
* SIEM alert generation
* User access control
* Grade management systems
* Temperature monitoring
* Security event classification

---

## Screenshots

### Screenshot 1

Number classification program.

### Screenshot 2

Positive number output.

### Screenshot 3

Negative number output.

### Screenshot 4

Grade classification output.

---

## Skills Learned

* Using if statements
* Using elif statements
* Using else statements
* Evaluating conditions
* Comparing values
* Decision-making in programs
* User input processing

---

## Conclusion

This lab demonstrated how Python programs can make decisions using conditional statements. By evaluating user input and applying logical conditions, the program successfully classified numbers and assigned grades based on score ranges. These concepts are essential for building interactive and intelligent applications.
