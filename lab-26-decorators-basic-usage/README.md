# Lab 26: Decorators - Basic Usage

## Objective

The objective of this lab is to understand Python decorators, learn how they modify function behavior, and implement a simple logging decorator.

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
def log_decorator(func):

    def wrapper(*args, **kwargs):

        print("Start")

        result = func(*args, **kwargs)

        print("End")

        return result

    return wrapper


@log_decorator
def say_hello(name):
    print(f"Hello, {name}!")


say_hello("Alice")
```

---

## Output

```text
Start
Hello, Alice!
End
```

---

## Key Concepts

### Decorator

A function that modifies the behavior of another function.

### Wrapper Function

A nested function used to execute code before and after the original function.

### *args

Accepts any number of positional arguments.

### **kwargs

Accepts any number of keyword arguments.

### @ Syntax

Applies a decorator to a function.

```python
@log_decorator
```

Equivalent to:

```python
say_hello = log_decorator(say_hello)
```

---

## Real-World Applications

* Logging
* Authentication
* Authorization
* Caching
* Performance Monitoring
* Cybersecurity Auditing

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program output.

---

## Skills Learned

* Creating decorators
* Using wrapper functions
* Using *args and **kwargs
* Applying decorators with @
* Extending function behavior
* Implementing reusable logging

---

## Conclusion

This lab demonstrated how decorators provide a clean and reusable way to extend function behavior without modifying the original function code. Decorators are widely used in modern Python applications for logging, authentication, monitoring, and performance optimization.
