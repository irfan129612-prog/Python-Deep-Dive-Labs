# 🧪 Lab 36: Using Collections (`deque` & `Counter`)

## 📌 Lab Summary

In this lab, Python's **collections** module was explored by working with two specialized data structures: **deque** and **Counter**. A `deque` was used to efficiently add and remove elements from both ends of a queue, while `Counter` was used to count the frequency of items in a collection and identify the most common elements.

---

## 🎯 Objectives

- Understand Python's `collections` module
- Learn how to use `deque` for queue operations
- Perform insertion and deletion from both ends of a deque
- Count item occurrences using `Counter`
- Identify the most common elements in a dataset

---

## 🛠️ Tools Used

- Ubuntu Linux
- Python 3.x
- PyCharm Community Edition
- Ubuntu Terminal

---

## 🗂️ Lab Environment

| Component | Details |
|----------|---------|
| Operating System | Ubuntu Linux |
| Python Version | Python 3.x |
| IDE | PyCharm Community Edition |
| Module | collections |
| Terminal | Ubuntu CLI |

---

## ✅ Task 1: Import Required Classes

Import the `deque` and `Counter` classes from Python's **collections** module.

```python
from collections import deque
from collections import Counter
```

### Result

- ✅ Required classes imported successfully.

---

## ✅ Task 2: Perform Queue Operations Using `deque`

Create a deque and perform insertion and deletion operations.

```python
d = deque()

d.append("task1")
d.append("task2")

last_task = d.pop()

d.appendleft("task0")

first_task = d.popleft()
```

### Operations Performed

- Add elements to the right side
- Remove the last element
- Add an element to the left side
- Remove the first element

### Result

- ✅ Queue operations executed successfully.

---

## ✅ Task 3: Count Data Using `Counter`

Create a list of words and count their occurrences.

```python
words = [
    "apple",
    "orange",
    "banana",
    "apple",
    "orange",
    "apple"
]

word_count = Counter(words)
```

Display the results.

```python
print(word_count)

print(word_count.most_common(2))
```

### Output

```text
Counter({'apple': 3, 'orange': 2, 'banana': 1})

[('apple', 3), ('orange', 2)]
```

### Result

- ✅ Word frequencies calculated successfully.
- ✅ Most common words identified.

---

## 💻 Complete Code

```python
from collections import deque
from collections import Counter

d = deque()

d.append("task1")
d.append("task2")

last_task = d.pop()

d.appendleft("task0")

first_task = d.popleft()

words = [
    "apple",
    "orange",
    "banana",
    "apple",
    "orange",
    "apple"
]

word_count = Counter(words)

print(word_count)

print(word_count.most_common(2))
```

---

## 💻 Command Used

```bash
python3 collections_demo.py
```

---

## 📋 Validation

The following tasks were successfully completed:

- ✅ Imported `deque` and `Counter`
- ✅ Added elements using `append()`
- ✅ Added elements using `appendleft()`
- ✅ Removed elements using `pop()`
- ✅ Removed elements using `popleft()`
- ✅ Counted word occurrences
- ✅ Displayed the most common elements

---

## 📚 Key Concepts

| Concept | Description |
|----------|-------------|
| collections | Python module providing specialized container data types |
| deque | Double-ended queue that supports fast insertion and deletion from both ends |
| append() | Adds an element to the right side of a deque |
| appendleft() | Adds an element to the left side of a deque |
| pop() | Removes and returns the rightmost element |
| popleft() | Removes and returns the leftmost element |
| Counter | Counts the frequency of hashable objects |
| most_common() | Returns the most frequently occurring elements |

---

## 🌍 Real-World Applications

Python collections are commonly used in:

- Task Scheduling
- Queue Management
- Browser History
- Log Analysis
- Event Counting
- SIEM Monitoring
- Data Processing
- Network Packet Queues

---

## 📸 Screenshots

Include screenshots for:

- Complete Python source code
- Program execution
- Counter output
- `most_common()` results

---

## 📖 What I Learned

- How to use Python's **collections** module.
- How `deque` enables efficient queue operations.
- How to insert and remove elements from both ends of a queue.
- How `Counter` simplifies counting repeated data.
- How `most_common()` quickly identifies the most frequent elements.
- Where these data structures are commonly used in cybersecurity and software development.

---

## ✅ Conclusion

This lab demonstrated the practical use of Python's **collections** module through the **deque** and **Counter** data structures. The `deque` provided efficient queue operations for managing ordered data, while `Counter` simplified frequency analysis by counting repeated elements and identifying the most common values. These specialized data structures improve code readability and performance and are widely used in **task scheduling, log analysis, SIEM monitoring, event processing, and data analytics**.
