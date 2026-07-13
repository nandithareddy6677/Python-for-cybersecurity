# Day 11: Object-Oriented Programming (OOP)

> Understanding Object-Oriented Programming (OOP), classes, objects, constructors, inheritance, encapsulation, and polymorphism in Python.

---

# 🎯 Learning Objectives

- Understand OOP.
- Learn Classes and Objects.
- Understand Constructors.
- Learn Inheritance.
- Explore Encapsulation and Polymorphism.
- Prepare for Python interviews.

---

# 📖 Introduction

Object-Oriented Programming (OOP) organizes code into reusable objects.

It makes programs easier to maintain, reuse, and scale.

---

# What is OOP?

OOP is a programming paradigm based on objects.

Objects contain:

- Data (Attributes)
- Functions (Methods)

---

# Class

A Class is a blueprint for creating objects.

Example:

```python
class Laptop:
    pass
```

---

# Object

```python
laptop = Laptop()
```

---

# Constructor

A constructor initializes object data.

```python
class Student:
    def __init__(self, name):
        self.name = name
```

---

# Methods

```python
class Student:
    def greet(self):
        print("Hello")
```

---

# Four Principles of OOP

- Encapsulation
- Inheritance
- Polymorphism
- Abstraction

---

# Inheritance

Allows one class to inherit another.

```python
class Animal:
    pass

class Dog(Animal):
    pass
```

---

# Encapsulation

Protects object data.

---

# Polymorphism

Different objects respond differently to the same method.

---

# Advantages

- Code Reusability
- Easy Maintenance
- Better Organization
- Scalability

---

# 📌 Key Takeaways

- Classes create objects.
- Constructors initialize objects.
- Inheritance promotes reuse.
- OOP improves software design.

---

# ❓ Interview Questions

### What is OOP?

Programming based on objects.

### Difference between Class and Object?

A class is a blueprint; an object is its instance.

### What is Inheritance?

Creating a new class from an existing one.

---

# 📝 Summary

Today I learned about Object-Oriented Programming, classes, objects, constructors, inheritance, encapsulation, and polymorphism. OOP helps build reusable and maintainable Python applications.
