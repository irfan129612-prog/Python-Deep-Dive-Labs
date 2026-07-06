# Lab 32: Logging with Python Logging Module

## Objective

The objective of this lab is to understand Python's logging module, configure log levels and formats, and implement logging in a practical Python application.

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
import logging

logging.basicConfig(
    level=logging.DEBUG,
    format="%(asctime)s - %(levelname)s - %(message)s"
)

logging.debug("This is a debug message.")
logging.info("This is an info message.")
logging.warning("This is a warning message.")
logging.error("This is an error message.")
logging.critical("This is a critical message.")


def divide_numbers(a, b):
    try:
        result = a / b
        logging.info("Division successful.")
        return result

    except ZeroDivisionError:
        logging.error("Division by zero error.")
        return None


result = divide_numbers(10, 0)

print("Result:", result)
```

---

## Output

```text
DEBUG - This is a debug message.
INFO - This is an info message.
WARNING - This is a warning message.
ERROR - This is an error message.
CRITICAL - This is a critical message.
ERROR - Division by zero error.
Result: None
```

---

## Key Concepts

### Logging

Logging records program activity, errors, warnings, and runtime information.

### Logging Levels

| Level    | Purpose                               |
| -------- | ------------------------------------- |
| DEBUG    | Detailed debugging information        |
| INFO     | General successful execution messages |
| WARNING  | Possible issue                        |
| ERROR    | Serious problem                       |
| CRITICAL | Very serious failure                  |

### basicConfig()

Used to configure logging level and output format.

### Log Format

```python
"%(asctime)s - %(levelname)s - %(message)s"
```

Displays time, log level, and message.

---

## Real-World Applications

* Debugging applications
* Monitoring automation scripts
* SIEM log generation
* Error tracking
* API monitoring
* Production system troubleshooting

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program output showing different log levels.

---

## Skills Learned

* Importing logging module
* Configuring logging level
* Formatting log messages
* Logging DEBUG, INFO, WARNING, ERROR, and CRITICAL messages
* Handling errors with logs
* Replacing print debugging with structured logging

---

## Conclusion

This lab demonstrated how Python's logging module provides a professional way to track program execution and errors. Logging is more reliable than print statements and is widely used in production systems, automation tools, and cybersecurity applications.
