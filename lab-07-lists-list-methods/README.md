# Lab 07: Lists & List Methods

## Objective

The objective of this lab is to understand Python lists and perform common list operations such as appending, removing, sorting, and iterating through elements.

---

## Lab Environment

| Component        | Details                   |
| ---------------- | ------------------------- |
| Operating System | Ubuntu Linux              |
| Python Version   | Python 3.x                |
| IDE              | PyCharm Community Edition |
| Terminal         | Ubuntu CLI                |

---

## Task 1: Create a List

### Code

```python
fruits = ["apple", "banana", "cherry"]

print("Initial list of fruits:", fruits)
```

### Output

```text
Initial list of fruits: ['apple', 'banana', 'cherry']
```

---

## Task 2: Append a New Item

### Code

```python
fruits.append("orange")

print("After append:", fruits)
```

### Output

```text
After append: ['apple', 'banana', 'cherry', 'orange']
```

---

## Task 3: Remove an Item

### Code

```python
fruits.remove("banana")

print("After remove:", fruits)
```

### Output

```text
After remove: ['apple', 'cherry', 'orange']
```

---

## Task 4: Sort the List

### Code

```python
fruits.sort()

print("After sorting:", fruits)
```

### Output

```text
After sorting: ['apple', 'cherry', 'orange']
```

---

## Task 5: Iterate Through the List

### Code

```python
for fruit in fruits:
    print("Fruit:", fruit)
```

### Output

```text
Fruit: apple
Fruit: cherry
Fruit: orange
```

---

## Understanding List Methods

| Method   | Purpose                          |
| -------- | -------------------------------- |
| append() | Add item at end                  |
| remove() | Delete specific item             |
| sort()   | Arrange items in ascending order |
| insert() | Add item at specific position    |
| pop()    | Remove item by index             |
| len()    | Count total elements             |

---

## Real-World Applications

* Managing user records
* Storing IP addresses
* Processing log entries
* Working with CSV data
* API response handling
* Network scanning results

---

## Screenshots

### Screenshot 1

Initial list creation.

### Screenshot 2

Appending and removing items.

### Screenshot 3

Sorting the list.

### Screenshot 4

Iterating through list elements using a for loop.

---

## Skills Learned

* Creating lists
* Adding items with append()
* Removing items with remove()
* Sorting data
* Iterating using for loops
* Understanding list indexing

---

## Conclusion

This lab introduced Python lists and demonstrated how they can store and manage collections of data efficiently. Common list operations such as appending, removing, sorting, and iteration were implemented to build a strong foundation for future data processing tasks.
