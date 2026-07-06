# Lab 19: Basic Recursion Example

## Objective

The objective of this lab is to understand recursion in Python, implement a recursive factorial function, compare recursion with iteration, and explore tail recursion.

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
def factorial(n):

    if n <= 1:
        return 1

    return n * factorial(n - 1)


def iterative_factorial(n):

    result = 1

    for i in range(2, n + 1):
        result *= i

    return result


def tail_recursive_factorial(n, accumulator=1):

    if n <= 1:
        return accumulator

    return tail_recursive_factorial(
        n - 1,
        n * accumulator
    )


print("Recursive Factorial:", factorial(5))
print("Iterative Factorial:", iterative_factorial(5))
print("Tail Recursive Factorial:", tail_recursive_factorial(5))
```

---

## Output

```text
Recursive Factorial: 120
Iterative Factorial: 120
Tail Recursive Factorial: 120
```

---

## Key Concepts

### Recursion

A technique where a function calls itself.

### Base Case

Stops the recursion.

```python
if n <= 1:
    return 1
```

### Recursive Case

Calls the same function with a smaller problem.

```python
return n * factorial(n - 1)
```

### Iteration

Uses loops instead of recursive calls.

### Tail Recursion

A special recursion pattern where the recursive call is the last operation.

---

## Real-World Applications

* Directory traversal
* Tree structures
* Graph algorithms
* Search algorithms
* Cybersecurity file scanning
* Data processing

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program output.

---

## Skills Learned

* Defining recursive functions
* Creating base cases
* Recursive problem solving
* Using loops for iteration
* Understanding tail recursion
* Comparing recursion and iteration

---

## Conclusion

This lab demonstrated how recursion can solve problems by breaking them into smaller sub-problems. Recursive, iterative, and tail-recursive approaches were implemented to calculate factorial values and compare different problem-solving techniques.
