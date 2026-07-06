# Lab 18: OOP - Inheritance Basics

## Objective

The objective of this lab is to understand inheritance in Object-Oriented Programming (OOP), create subclasses, override methods, and use the super() function to extend parent class functionality.

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

    def __init__(self, make, model, year):
        self.make = make
        self.model = model
        self.year = year

    def describe_car(self):
        print(f"{self.year} {self.make} {self.model}")


class ElectricCar(Car):

    def __init__(self, make, model, year, battery_size=75):
        super().__init__(make, model, year)
        self.battery_size = battery_size

    def describe_battery(self):
        print(f"This car has a {self.battery_size}-kWh battery.")

    def describe_car(self):
        super().describe_car()
        self.describe_battery()


my_tesla = ElectricCar("Tesla", "Model S", 2022)

my_tesla.describe_car()
```

---

## Output

```text
2022 Tesla Model S
This car has a 75-kWh battery.
```

---

## Key Concepts

### Inheritance

Allows a class to inherit attributes and methods from another class.

### Parent Class

```python
class Car:
```

The base class.

### Child Class

```python
class ElectricCar(Car):
```

The derived class.

### super()

Used to access methods and constructors of the parent class.

```python
super().__init__()
```

### Method Overriding

A child class can redefine a method from the parent class.

---

## Real-World Applications

* User and Admin systems
* Network device management
* Security monitoring tools
* Automation frameworks
* Web applications
* Enterprise software systems

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program output.

---

## Skills Learned

* Creating parent classes
* Creating child classes
* Using inheritance
* Using super()
* Method overriding
* Extending class functionality

---

## Conclusion

This lab demonstrated how inheritance promotes code reuse and extensibility in Object-Oriented Programming. By extending the Car class into an ElectricCar class, additional functionality was introduced while maintaining access to the parent class features.
