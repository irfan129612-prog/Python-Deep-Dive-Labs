# Lab 12: File I/O Basics

## Objective

The objective of this lab is to understand how to read from and write to files in Python using built-in file handling functions and context managers.

---

## Lab Environment

| Component        | Details                   |
| ---------------- | ------------------------- |
| Operating System | Ubuntu Linux              |
| Python Version   | Python 3.x                |
| IDE              | PyCharm Community Edition |
| Terminal         | Ubuntu CLI                |

---

## Project Structure

```text
lab-12-file-io-basics/
│
├── write_file.py
├── read_file.py
└── output.txt
```

---

## Writing to a File

### Code

```python
with open("output.txt", "w") as f:
    f.write("Hello, World!\n")
    f.write("This is a file I/O example.\n")
    f.write("Python makes File I/O easy!\n")
```

---

## Reading from a File

### Code

```python
with open("output.txt", "r") as f:
    for line in f:
        print(line.strip())
```

---

## Output

```text
Hello, World!
This is a file I/O example.
Python makes File I/O easy!
```

---

## Key Concepts

### File I/O

File Input/Output allows programs to store and retrieve data from files.

### open()

Used to open files.

```python
open("output.txt", "w")
```

### Write Mode

```python
"w"
```

Creates or overwrites a file.

### Read Mode

```python
"r"
```

Reads data from an existing file.

### Context Manager

```python
with open(...) as f:
```

Automatically closes the file after use.

### strip()

Removes extra spaces and newline characters.

---

## Real-World Applications

* Log file analysis
* SIEM event processing
* Report generation
* Configuration files
* CSV processing
* Data storage

---

## Screenshots

### Screenshot 1

Source code and project structure.

### Screenshot 2

Program output and generated output.txt file.

---

## Skills Learned

* Creating files
* Writing data to files
* Reading data from files
* Using context managers
* Understanding file modes
* Processing text files

---

## Conclusion

This lab demonstrated the fundamentals of file handling in Python. Data was successfully written to and read from a text file using context managers, providing a safe and efficient approach to file operations.
