# Lab 06: For & While Loops

## Objective

The objective of this lab is to understand iterative programming using Python's for and while loops. The lab demonstrates how loops automate repetitive tasks and control program execution.

---

## Lab Environment

| Component        | Details                   |
| ---------------- | ------------------------- |
| Operating System | Ubuntu Linux              |
| Python Version   | Python 3.x                |
| IDE              | PyCharm Community Edition |
| Terminal         | Ubuntu CLI                |

---

## Task 1: Using a For Loop

### Code

```python
for i in range(1, 6):
    print(i)
```

### Output

```text
1
2
3
4
5
```

### Explanation

The `range(1, 6)` function generates numbers from 1 to 5. The loop iterates through each number and prints it.

---

## Task 2: Using a While Loop

### Code

```python
total = 0
i = 1

while total <= 20:
    total += i
    i += 1

print("Final total:", total)
```

### Output

```text
Final total: 21
```

### Explanation

The loop continuously adds values to the total until the total exceeds 20.

---

## Comparison: For vs While Loop

| For Loop                       | While Loop                           |
| ------------------------------ | ------------------------------------ |
| Used when iterations are known | Used when iterations are unknown     |
| Iterates over sequences        | Executes based on a condition        |
| Simpler for fixed ranges       | More flexible for dynamic conditions |

---

## Real-World Applications

* Processing log files
* SIEM event analysis
* Data processing
* Automation scripts
* Monitoring systems
* Network scanning

---

## Screenshots

### Screenshot 1

For loop source code.

### Screenshot 2

For loop output.

### Screenshot 3

While loop source code.

### Screenshot 4

While loop output.

---

## Skills Learned

* Iteration
* range() function
* Loop variables
* Accumulators
* While loop conditions
* Preventing infinite loops
* Repetitive task automation

---

## Conclusion

This lab introduced Python's two primary looping constructs: for loops and while loops. Both techniques are essential for automation, data processing, cybersecurity scripting, and efficient software development.
