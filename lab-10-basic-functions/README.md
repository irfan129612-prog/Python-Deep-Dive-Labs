# Lab 10: Basic Functions

## Objective

The objective of this lab is to understand Python functions, parameters, default values, and keyword arguments. Functions help organize code into reusable and maintainable blocks.

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
# Function with parameter
def greet(name):
    return f"Hello, {name}!"

print(greet("Alice"))
print(greet("Bob"))
print(greet("Charlie"))

# Function with default parameter
def greet_default(name="Guest"):
    return f"Hello, {name}!"

print(greet_default())

# Function with keyword argument
print(greet_default(name="Diana"))
```

---

## Output

```text
Hello, Alice!
Hello, Bob!
Hello, Charlie!
Hello, Guest!
Hello, Diana!
```

---

## Key Concepts

### Function

A reusable block of code designed to perform a specific task.

### Parameter

Input variable defined in a function.

```python
def greet(name):
```

### Argument

Actual value passed to the function.

```python
greet("Alice")
```

### Return Statement

Returns a value from the function.

```python
return f"Hello, {name}!"
```

### Default Parameter

Used when no argument is supplied.

```python
def greet_default(name="Guest"):
```

### Keyword Argument

Arguments passed using parameter names.

```python
greet_default(name="Diana")
```

---

## Real-World Applications

* User greeting systems
* Login modules
* SIEM alert functions
* API request handlers
* Data processing tasks
* Automation scripts

---

## Screenshots

### Screenshot 1

Complete lab code.

### Screenshot 2

Program output.

---

## Skills Learned

* Defining functions
* Calling functions
* Using parameters
* Using arguments
* Returning values
* Using default parameters
* Using keyword arguments

---

## Conclusion

This lab demonstrated how functions improve code organization and reusability. Parameters, default values, and keyword arguments provide flexibility, making functions one of the most essential building blocks in Python programming.
