# Day 15: OS, sys & subprocess Modules

> Understanding Python's os, sys, and subprocess modules for interacting with the operating system and automating system tasks.

---

# 🎯 Learning Objectives

- Learn os module.
- Understand sys module.
- Execute commands with subprocess.
- Automate operating system tasks.
- Prepare for cybersecurity scripting.

---

# 📖 Introduction

Cybersecurity professionals frequently interact with the operating system.

Python provides built-in modules that simplify system administration and automation.

---

# OS Module

```python
import os
```

Functions:

- Create folders
- Delete files
- Rename files
- Get current directory

---

# Current Directory

```python
os.getcwd()
```

---

# List Files

```python
os.listdir()
```

---

# Create Directory

```python
os.mkdir("test")
```

---

# Remove Directory

```python
os.rmdir("test")
```

---

# sys Module

```python
import sys
```

Useful Functions:

```python
sys.version
```

```python
sys.platform
```

```python
sys.argv
```

---

# subprocess Module

```python
import subprocess
```

Run a command:

```python
subprocess.run(["ls"])
```

Windows Example:

```python
subprocess.run(["ipconfig"])
```

Linux Example:

```python
subprocess.run(["ifconfig"])
```

---

# Cybersecurity Uses

- Execute Security Tools
- Automate Commands
- Collect System Information
- Incident Response Scripts

---

# Best Practices

- Validate user input.
- Avoid executing untrusted commands.
- Handle exceptions.
- Use subprocess instead of os.system().

---

# 📌 Key Takeaways

- os interacts with files and directories.
- sys provides system information.
- subprocess executes operating system commands.
- These modules are heavily used in automation.

---

# ❓ Interview Questions

### 1. What does the os module do?

Interacts with the operating system.

### 2. Which module executes system commands?

subprocess

### 3. Which module provides command-line arguments?

sys

### 4. Which function lists files?

os.listdir()

### 5. Why use subprocess?

To safely execute external commands.

---

# 📝 Summary

Today I learned about Python's os, sys, and subprocess modules. These modules enable automation, system administration, and cybersecurity scripting by interacting with the operating system.
