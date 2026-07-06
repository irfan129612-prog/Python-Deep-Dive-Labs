# Lab 17: OOP - Defining Classes

## Objective

The objective of this lab is to understand the fundamentals of Object-Oriented Programming (OOP) by creating classes, objects, attributes, and methods in Python.

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
class Car:

    wheels = 4

    def __init__(self, brand, model):
        self.brand = brand
        self.model = model

    def drive(self):
        print(f"The {self.brand} {self.model} is now driving.")


car1 = Car("Toyota", "Corolla")
car2 = Car("Honda", "Civic")

car1.drive()
car2.drive()

print(f"Car 1 brand: {car1.brand}")
print(f"Car 2 brand: {car2.brand}")

print(f"Number of wheels: {Car.wheels}")
```

---

## Output

```text
The Toyota Corolla is now driving.
The Honda Civic is now driving.

Car 1 brand: Toyota
Car 2 brand: Honda

Number of wheels: 4
```

---

## Key Concepts

### Class

A blueprint used to create objects.

### Object

An instance of a class.

### Constructor

```python
__init__()
```

Automatically initializes object attributes.

### Instance Attributes

Attributes unique to each object.

```python
self.brand
self.model
```

### Class Attributes

Attributes shared among all objects.

```python
wheels = 4
```

### Methods

Functions defined inside a class.

```python
def drive(self):
```

---

## Real-World Applications

* Software development
* Automation frameworks
* Cybersecurity tools
* Network scanners
* Data processing systems
* Web applications

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program output.

---

## Skills Learned

* Creating classes
* Creating objects
* Using constructors
* Using instance attributes
* Using class attributes
* Defining methods
* Understanding OOP fundamentals

---

## Conclusion

This lab introduced the fundamentals of Object-Oriented Programming in Python. Classes, objects, methods, and attributes were implemented to demonstrate how OOP helps organize and structure code efficiently. These concepts serve as the foundation for more advanced Python programming and software development.
