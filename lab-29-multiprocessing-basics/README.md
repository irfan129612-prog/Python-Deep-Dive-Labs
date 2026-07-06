# Lab 29: Multiprocessing Basics

## Objective

The objective of this lab is to understand multiprocessing in Python, create multiple processes, and compare multiprocessing with multithreading.

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
import multiprocessing


def sum_large_list(num_list):

    total = sum(num_list)

    print(f"Sum of the list is: {total}")


if __name__ == "__main__":

    numbers = list(range(1000000))

    process1 = multiprocessing.Process(
        target=sum_large_list,
        args=(numbers,)
    )

    process2 = multiprocessing.Process(
        target=sum_large_list,
        args=(numbers,)
    )

    process1.start()
    process2.start()

    process1.join()
    process2.join()

    print("All processes completed.")
```

---

## Output

```text
Sum of the list is: 499999500000
Sum of the list is: 499999500000

All processes completed.
```

---

## Key Concepts

### Process

An independent running program.

### Multiprocessing

Running multiple processes simultaneously.

### start()

Begins process execution.

### join()

Waits for process completion.

### CPU-Bound Tasks

Tasks requiring heavy processor usage.

---

## Multiprocessing vs Multithreading

| Feature     | Thread       | Process            |
| ----------- | ------------ | ------------------ |
| Memory      | Shared       | Separate           |
| Isolation   | Low          | High               |
| Performance | Good for I/O | Good for CPU Tasks |

---

## Real-World Applications

* Image processing
* Video rendering
* Machine learning
* Data analysis
* Password cracking
* Security scanning

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program output.

---

## Skills Learned

* Creating processes
* Starting processes
* Using join()
* Understanding CPU-bound processing
* Understanding process isolation
* Comparing threads and processes

---

## Conclusion

This lab demonstrated how multiprocessing enables parallel execution of CPU-intensive tasks using independent processes. Unlike threads, processes operate in separate memory spaces, providing better isolation and improved performance for computational workloads.
