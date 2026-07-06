# Lab 25: Intro to Unit Testing with unittest

## Objective

The objective of this lab is to understand the basics of unit testing in Python using the built-in unittest module and verify the correctness of a simple function.

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
import unittest


def add(a, b):
    return a + b


class TestMath(unittest.TestCase):

    def test_add(self):
        self.assertEqual(add(2, 3), 5)


if __name__ == "__main__":
    unittest.main()
```

---

## Run Test

```bash
python3 -m unittest discover
```

---

## Output

```text
.
----------------------------------------------------------------------
Ran 1 test in 0.000s

OK
```

---

## Key Concepts

### Unit Testing

Testing small parts of code individually.

### unittest

Python's built-in testing framework.

### Test Case

A class that contains test methods.

### assertEqual()

Checks whether two values are equal.

```python
self.assertEqual(add(2, 3), 5)
```

### Test Discovery

```bash
python3 -m unittest discover
```

Automatically finds test files starting with `test_`.

---

## Real-World Applications

* Testing Python functions
* Automation script validation
* API testing
* Data processing validation
* Cybersecurity tool testing
* Preventing bugs before deployment

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Successful test output.

---

## Skills Learned

* Writing testable functions
* Creating unittest test cases
* Using assertEqual()
* Running tests from terminal
* Understanding test pass output
* Using test discovery

---

## Conclusion

This lab introduced unit testing in Python using the unittest module. A simple add function was tested successfully, demonstrating how unit tests help verify program correctness and improve code reliability.
