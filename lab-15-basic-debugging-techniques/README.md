# Lab 15: Basic Debugging Techniques

## Objective

The objective of this lab is to understand basic debugging techniques in Python using print statements and the Python Debugger (pdb).

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
def calculate_sum(numbers):
    total = 0

    for num in numbers:
        total += num
        print("Debug: Adding", num, "Total so far:", total)

    return total

numbers = [5, 10, 15]

print("Final Sum:", calculate_sum(numbers))


def divide_numbers(a, b):
    import pdb
    pdb.set_trace()

    result = a / b
    print("Result:", result)

    return result

divide_numbers(10, 2)
```

---

## Output

```text
Debug: Adding 5 Total so far: 5
Debug: Adding 10 Total so far: 15
Debug: Adding 15 Total so far: 30

Final Sum: 30
```

Debugger Output:

```text
(Pdb) p a
10

(Pdb) p b
2

(Pdb) c
Result: 5.0
```

---

## Key Concepts

### Debugging

The process of identifying and fixing errors in a program.

### Print Statements

Used to display variable values and track program execution.

### pdb

Python's built-in debugger used to inspect variables and control execution flow.

### Common pdb Commands

| Command    | Purpose              |
| ---------- | -------------------- |
| n          | Execute next line    |
| s          | Step into function   |
| c          | Continue execution   |
| p variable | Print variable value |
| q          | Quit debugger        |

---

## Real-World Applications

* Troubleshooting Python scripts
* Debugging automation tools
* Investigating API responses
* Analyzing SIEM log processing
* Finding logical errors in programs

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Debugger session and program output.

---

## Skills Learned

* Using print statements for debugging
* Tracking variable values
* Using pdb.set_trace()
* Inspecting variables with pdb
* Stepping through code execution
* Understanding debugging workflows

---

## Conclusion

This lab demonstrated how debugging techniques help identify and resolve programming errors. Both print-based debugging and Python's built-in pdb debugger were used to inspect program execution and improve troubleshooting skills.
