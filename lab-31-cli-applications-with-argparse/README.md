# Lab 31: CLI Applications with argparse

## Objective

The objective of this lab is to understand how to build Command Line Interface (CLI) applications in Python using the argparse module.

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
import argparse

parser = argparse.ArgumentParser(
    description="A simple greeting application."
)

parser.add_argument(
    "--name",
    type=str,
    help="The name of the person to greet."
)

args = parser.parse_args()

if args.name:
    print(f"Hello, {args.name}!")
else:
    print("Hello, Stranger!")
```

---

## Running the Program

### Example 1

```bash
python3 greet.py --name Alice
```

Output:

```text
Hello, Alice!
```

### Example 2

```bash
python3 greet.py
```

Output:

```text
Hello, Stranger!
```

### Example 3

```bash
python3 greet.py --help
```

Output:

```text
usage: greet.py [-h] [--name NAME]
```

---

## Key Concepts

### CLI

Command Line Interface used to interact with applications using terminal commands.

### argparse

Python module used to parse command-line arguments.

### ArgumentParser

Creates a command-line parser.

### add_argument()

Defines command-line options.

### parse_args()

Reads and stores command-line arguments.

### Automatic Help

argparse automatically generates help documentation.

---

## Real-World Applications

* Security scanners
* Network automation tools
* Log analyzers
* Backup scripts
* System administration utilities
* Data processing tools

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program execution and help output.

---

## Skills Learned

* Creating CLI applications
* Using argparse
* Defining arguments
* Parsing command-line input
* Generating automatic help text
* Building user-friendly tools

---

## Conclusion

This lab demonstrated how Python's argparse module simplifies the development of command-line applications. By defining arguments and parsing user input, developers can create flexible and reusable automation tools commonly used in software development, system administration, and cybersecurity.
