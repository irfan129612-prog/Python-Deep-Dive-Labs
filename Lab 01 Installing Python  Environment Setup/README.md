# Lab 01: Installing Python & Environment Setup

## Objective

The objective of this lab is to install Python 3, verify the installation, and configure a Python development environment on Ubuntu Linux.

---

## Lab Environment

| Component        | Details                   |
| ---------------- | ------------------------- |
| Operating System | Ubuntu Linux              |
| Python Version   | Python 3.x                |
| IDE              | PyCharm Community Edition |
| Terminal         | Ubuntu CLI                |

---

## Task 1: Install Python 3

### Update Package Repository

```bash
sudo apt update
```

### Install Python 3

```bash
sudo apt install python3 -y
```

### Verify Installation

```bash
python3 --version
```

### Sample Output

```text
Python 3.12.3
```

---

## Task 2: Verify pip Installation

Check pip version:

```bash
pip3 --version
```

If pip is not installed:

```bash
sudo apt install python3-pip -y
```

Verify again:

```bash
pip3 --version
```

---

## Task 3: Verify PyCharm Installation

Launch PyCharm and create a new Python project.

Create a file named:

```text
hello.py
```

Add the following code:

```python
print("Hello World")
```

Run the program from PyCharm.

### Output

```text
Hello World
```

---

## Understanding What Happened

### Python

Python is a high-level programming language widely used in automation, cybersecurity, data science, machine learning, and software development.

### Python Interpreter

The Python interpreter reads Python code line by line and executes it.

Example:

```python
print("Hello World")
```

The interpreter processes the `print()` function and displays the text on the screen.

### pip

pip is Python's package manager. It allows installation of external libraries and tools required for Python development.

Example:

```bash
pip3 install requests
```

### IDE (Integrated Development Environment)

PyCharm provides features such as:

* Code completion
* Syntax highlighting
* Debugging tools
* Project management

These features improve productivity and simplify Python development.

---

## Skills Learned

* Installing Python on Ubuntu Linux
* Using APT package manager
* Verifying Python installation
* Understanding Python interpreter
* Using pip package manager
* Configuring PyCharm
* Running Python programs

---

## Conclusion

Python 3 was successfully installed and verified on Ubuntu Linux. The development environment was configured using PyCharm, and a simple Python program was executed successfully. The system is now ready for Python development, automation, cybersecurity scripting, and data science projects.
