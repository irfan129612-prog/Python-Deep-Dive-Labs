# Lab 09: Dictionaries & Key Operations

## Objective

The objective of this lab is to understand Python dictionaries and perform common operations such as creating, accessing, updating, removing, and iterating through dictionary data.

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
user_profile = {
    "name": "Alice",
    "age": 30,
    "city": "New York"
}

print("Initial Dictionary:", user_profile)

print("User Name:", user_profile["name"])

user_profile["age"] = 31
print("Updated Dictionary:", user_profile)

user_profile.pop("city")
print("After Removing City:", user_profile)

for key, value in user_profile.items():
    print(f"{key}: {value}")

for key in user_profile.keys():
    print(f"Key: {key}")
```

---

## Output

```text
Initial Dictionary: {'name': 'Alice', 'age': 30, 'city': 'New York'}

User Name: Alice

Updated Dictionary: {'name': 'Alice', 'age': 31, 'city': 'New York'}

After Removing City: {'name': 'Alice', 'age': 31}

name: Alice
age: 31

Key: name
Key: age
```

---

## Key Concepts

### Dictionary

A dictionary stores data in key-value pairs.

Example:

```python
{
    "name": "Alice",
    "age": 30
}
```

### Accessing Values

```python
user_profile["name"]
```

### Updating Values

```python
user_profile["age"] = 31
```

### Removing Keys

```python
user_profile.pop("city")
```

### Iterating Through Dictionary

```python
for key, value in user_profile.items():
```

---

## Real-World Applications

* JSON data processing
* API responses
* User profiles
* Configuration files
* SIEM alerts and logs
* Network device information

---

## Screenshots

### Screenshot 1

Complete lab code.

### Screenshot 2

Program output.

---

## Skills Learned

* Creating dictionaries
* Accessing dictionary values
* Updating dictionary entries
* Removing keys using pop()
* Iterating with items()
* Iterating with keys()

---

## Conclusion

This lab demonstrated how dictionaries store and manage key-value data efficiently. Dictionaries are one of the most commonly used data structures in Python and play a critical role in data processing, APIs, automation, and cybersecurity scripting.
