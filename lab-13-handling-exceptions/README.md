# Lab 13: Handling Exceptions

## Objective

The objective of this lab is to understand exception handling in Python and learn how to prevent program crashes using try, except, and finally blocks.

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
user_input = input("Enter a number: ")

try:
    number = int(user_input)
    print(f"The number is {number}")

except ValueError:
    print("Error: Input is not a valid number. Please enter an integer.")

try:
    result = 10 / int(user_input)
    print(f"Result is: {result}")

except ValueError:
    print("Error: Please enter numeric values!")

except ZeroDivisionError:
    print("Error: Division by zero is undefined!")

finally:
    print("Program execution completed.")
```

---

## Example Output

### Valid Input

```text
Enter a number: 5
The number is 5
Result is: 2.0
Program execution completed.
```

### Invalid Input

```text
Enter a number: abc
Error: Input is not a valid number. Please enter an integer.
Error: Please enter numeric values!
Program execution completed.
```

### Division by Zero

```text
Enter a number: 0
The number is 0
Error: Division by zero is undefined!
Program execution completed.
```

---

## Key Concepts

### try

Contains code that may generate an exception.

### except

Handles specific exceptions and prevents crashes.

### ValueError

Occurs when invalid data type conversion is attempted.

### ZeroDivisionError

Occurs when dividing by zero.

### finally

Always executes regardless of whether an exception occurs.

---

## Real-World Applications

* User input validation
* File handling
* API requests
* Database operations
* SIEM log processing
* Automation scripts

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program output showing exception handling.

---

## Skills Learned

* Using try blocks
* Handling exceptions
* Using multiple except blocks
* Working with ValueError
* Working with ZeroDivisionError
* Using finally blocks

---

## Conclusion

This lab demonstrated how Python exception handling prevents application crashes and improves reliability. Using try, except, and finally blocks allows programs to handle unexpected situations gracefully and continue execution safely.
