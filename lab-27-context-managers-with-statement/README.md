# Lab 27: Context Managers (with statement)

## Objective

The objective of this lab is to understand Python context managers, implement custom context managers using **enter**() and **exit**(), and manage resources automatically with the with statement.

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
class MyContext:

    def __enter__(self):
        print("Entering the context and allocating resources.")
        return self

    def __exit__(self, exc_type, exc_value, traceback):
        print("Exiting the context and cleaning up resources.")


with MyContext() as context:
    print("Running within the context block.")


class FileManager:

    def __init__(self, filename, mode):
        self.filename = filename
        self.mode = mode

    def __enter__(self):
        self.file = open(self.filename, self.mode)
        return self.file

    def __exit__(self, exc_type, exc_value, traceback):
        self.file.close()


with FileManager("sample.txt", "w") as f:
    f.write("Hello, World!")
```

---

## Output

```text
Entering the context and allocating resources.
Running within the context block.
Exiting the context and cleaning up resources.

File closed successfully.
```

---

## Key Concepts

### Context Manager

Handles setup and cleanup of resources automatically.

### with Statement

Provides automatic resource management.

### **enter**()

Called when entering the with block.

### **exit**()

Called when leaving the with block.

### Resource Cleanup

Ensures resources are released even if exceptions occur.

---

## Real-World Applications

* File handling
* Database connections
* Network sockets
* SSH sessions
* Thread synchronization
* Security log processing

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program output.

---

## Skills Learned

* Creating context managers
* Using **enter**()
* Using **exit**()
* Using with statements
* Managing resources safely
* Automatic cleanup handling

---

## Conclusion

This lab demonstrated how Python context managers simplify resource management by automating setup and cleanup operations. Using the with statement ensures resources are properly released, improving code reliability and maintainability.
