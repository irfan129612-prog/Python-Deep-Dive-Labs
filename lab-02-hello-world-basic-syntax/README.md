# Lab 02: Hello World & Basic Syntax

## Objective

The objective of this lab is to create and execute a simple Python script, understand Python syntax, and learn how indentation defines code blocks.

---

## Lab Environment

| Component        | Details                   |
| ---------------- | ------------------------- |
| Operating System | Ubuntu Linux              |
| Python Version   | Python 3.x                |
| IDE              | PyCharm Community Edition |
| Terminal         | Ubuntu CLI                |

---

## Task 1: Create a Python Script

Create a file named:

```text
hello.py
```

Add the following code:

```python
print("Hello, World!")
```

---

## Task 2: Execute the Script

Run the script using:

```bash
python3 hello.py
```

### Output

```text
Hello, World!
```

---

## Task 3: Understanding Indentation

### Correct Example

```python
if True:
    print("This will always print because the condition is True.")

print("Hello, World!")
```

### Output

```text
This will always print because the condition is True.
Hello, World!
```

---

### Incorrect Example

```python
if True:
print("This will cause an IndentationError.")
```

### Output

```text
IndentationError: expected an indented block
```

---

## Understanding the Code

### print()

The `print()` function displays text or values on the screen.

### String

Text enclosed in quotation marks is called a string.

Example:

```python
"Hello, World!"
```

### if Statement

The `if` statement executes code only when a condition evaluates to True.

### Indentation

Python uses indentation (spaces) to define blocks of code instead of curly braces `{}`.

Incorrect indentation causes syntax errors and prevents program execution.

---

## Screenshots

### Screenshot 1

Creating hello.py in Ubuntu terminal.

### Screenshot 2

Executing the Hello World script.

### Screenshot 3

Running the correctly indented if statement.

### Screenshot 4

IndentationError generated due to incorrect indentation.

---

## Skills Learned

* Creating Python scripts
* Running Python programs from terminal
* Using the print() function
* Understanding strings
* Working with if statements
* Understanding Python indentation rules
* Identifying and fixing syntax errors

---

## Conclusion

A basic Python script was created and executed successfully. The lab demonstrated how Python programs are run and highlighted the importance of indentation in defining code blocks and preventing syntax errors.
