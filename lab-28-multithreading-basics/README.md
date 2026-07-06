# Lab 28: Multithreading Basics

## Objective

The objective of this lab is to understand the fundamentals of multithreading in Python, create and manage threads, and explore shared memory concepts and concurrency issues.

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
import threading


def print_numbers(thread_name, start, end):

    for number in range(start, end):
        print(f"{thread_name}: {number}")


thread1 = threading.Thread(
    target=print_numbers,
    args=("Thread-1", 0, 5)
)

thread2 = threading.Thread(
    target=print_numbers,
    args=("Thread-2", 5, 10)
)


thread1.start()
thread2.start()

thread1.join()
thread2.join()

print("All threads completed.")
```

---

## Example Output

```text
Thread-1: 0
Thread-1: 1
Thread-2: 5
Thread-2: 6
...
All threads completed.
```

---

## Key Concepts

### Thread

A lightweight execution unit within a process.

### Multithreading

Running multiple threads concurrently.

### start()

Starts thread execution.

### join()

Waits for a thread to finish.

### Shared Memory

Threads share the same memory space.

### Race Condition

Occurs when multiple threads modify shared data simultaneously.

---

## Real-World Applications

* Web servers
* Log monitoring
* Port scanning
* Network monitoring
* Background tasks
* Security automation

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program output.

---

## Skills Learned

* Creating threads
* Starting threads
* Using join()
* Understanding concurrency
* Understanding shared memory
* Recognizing race conditions

---

## Conclusion

This lab demonstrated how multithreading allows multiple tasks to execute concurrently within a single program. Threads improve responsiveness and performance but require careful handling of shared resources to avoid concurrency-related issues.
