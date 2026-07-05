# Lab 08: Tuples & Sets

## Objective

The objective of this lab is to understand tuples and sets in Python and observe their key properties through practical examples.

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
# Lab 08: Tuples & Sets

coordinates = (10, 20, 30)
print("Coordinates Tuple:", coordinates)

try:
    coordinates[0] = 100
except TypeError as e:
    print("Tuple Error:", e)

number_set = {1, 2, 3, 4, 5}
print("Initial Set:", number_set)

number_set.add(3)
print("Set after adding duplicate:", number_set)
```

---

## Output

```text
Coordinates Tuple: (10, 20, 30)
Tuple Error: 'tuple' object does not support item assignment
Initial Set: {1, 2, 3, 4, 5}
Set after adding duplicate: {1, 2, 3, 4, 5}
```

---

## Explanation

A tuple is an ordered and immutable collection. Once a tuple is created, its values cannot be changed.

A set is an unordered collection that stores only unique values. When a duplicate value is added to a set, Python automatically ignores it.

---

## Screenshots

### Screenshot 1

Complete lab code.

### Screenshot 2

Program output.

---

## Skills Learned

* Creating tuples
* Understanding tuple immutability
* Handling TypeError using try-except
* Creating sets
* Adding values to sets
* Understanding duplicate removal in sets

---

## Conclusion

This lab demonstrated the use of tuples and sets in Python. Tuples are useful for fixed data, while sets are useful for storing unique values and removing duplicates.
