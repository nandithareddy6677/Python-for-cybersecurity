# Day 10: Modules and Packages

> Understanding Python Modules, Packages, importing code, creating reusable programs, and organizing large Python projects.

---

# 🎯 Learning Objectives

- Understand Modules.
- Learn Packages.
- Import Modules.
- Create Custom Modules.
- Understand Python Libraries.
- Learn pip.
- Prepare for Python interviews.

---

# 📖 Introduction

Imagine writing the same code in every program.

Python solves this problem using **Modules** and **Packages**.

They allow programmers to organize code into reusable files, making applications easier to develop and maintain.

---

# 📦 What is a Module?

A Module is a Python file containing functions, variables, or classes.

Example

```
math.py
```

A module can be imported into another program.

---

# Importing Modules

Example

```python
import math

print(math.sqrt(25))
```

Output

```
5.0
```

---

# Import Specific Functions

```python
from math import sqrt

print(sqrt(16))
```

Output

```
4.0
```

---

# Import with Alias

```python
import math as m

print(m.pi)
```

Output

```
3.1415926535
```

---

# Common Built-in Modules

| Module | Purpose |
|----------|----------|
| math | Mathematical operations |
| random | Random numbers |
| os | Operating system tasks |
| sys | System information |
| datetime | Date & Time |
| json | JSON processing |
| csv | CSV files |

---

# What is a Package?

A Package is a collection of related modules.

Example

```
Project

↓

Utilities Package

↓

math.py

email.py

database.py
```

Packages help organize large projects.

---

# Creating Your Own Module

Create

```
calculator.py
```

```python
def add(a,b):
    return a+b
```

Main Program

```python
import calculator

print(calculator.add(10,20))
```

Output

```
30
```

---

# Installing Packages

Python uses **pip**.

Install Requests Library

```bash
pip install requests
```

Upgrade Package

```bash
pip install --upgrade requests
```

Uninstall

```bash
pip uninstall requests
```

---

# Popular Python Packages

- requests
- numpy
- pandas
- matplotlib
- flask
- django
- boto3
- scapy

---

# What is PyPI?

PyPI (Python Package Index) is the official repository for Python packages.

Thousands of libraries are available through PyPI.

---

# 🌍 Real-Life Example

Cybersecurity Script

```python
import requests

response = requests.get("https://example.com")

print(response.status_code)
```

Cloud Script

```python
import boto3

ec2 = boto3.client("ec2")
```

Automation Script

```python
import os

print(os.getcwd())
```

---

# Modules in Cybersecurity

Common Modules

- hashlib
- socket
- scapy
- requests
- os
- subprocess

---

# Modules in Cloud Computing

Common Modules

- boto3
- json
- os
- datetime
- requests

---

# 💡 Best Practices

- Organize code into modules.
- Use meaningful module names.
- Install packages only from trusted sources.
- Keep packages updated.
- Avoid duplicate code.

---

# 📌 Key Takeaways

- Modules are Python files.
- Packages are collections of modules.
- import allows code reuse.
- pip installs packages.
- PyPI hosts thousands of Python libraries.
- Modules improve code organization.

---

# ❓ Interview Questions

### 1. What is a Module?

A Module is a Python file containing reusable code.

---

### 2. What is a Package?

A Package is a collection of related Python modules.

---

### 3. Which keyword imports a module?

```python
import
```

---

### 4. Which tool installs Python packages?

```text
pip
```

---

### 5. What is PyPI?

PyPI is the official repository of Python packages.

---

### 6. Which module is used for mathematical operations?

```python
math
```

---

### 7. Which module is commonly used for AWS?

```python
boto3
```

---

### 8. Why are Modules important?

They improve code reusability, organization, and maintainability.

---

# 📝 Summary

Today I learned about Python Modules and Packages. I explored importing modules, creating custom modules, installing libraries using pip, and organizing Python projects efficiently. Modules and Packages are essential for building scalable applications and are heavily used in cloud computing, cybersecurity, automation, and software development.
