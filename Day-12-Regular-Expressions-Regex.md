# Day 12: Regular Expressions (Regex)

> Understanding Regular Expressions (Regex), pattern matching, searching, validation, and text extraction in Python.

---

# 🎯 Learning Objectives

- Understand Regex.
- Learn Pattern Matching.
- Search Text.
- Validate Input.
- Extract Information.

---

# 📖 Introduction

Regular Expressions (Regex) are used to search, validate, and manipulate text using patterns.

They are widely used in cybersecurity for log analysis and input validation.

---

# Regex Module

```python
import re
```

---

# Search

```python
re.search()
```

---

# Find All

```python
re.findall()
```

---

# Replace

```python
re.sub()
```

---

# Common Symbols

| Symbol | Meaning |
|---------|----------|
| . | Any character |
| * | Zero or more |
| + | One or more |
| ? | Optional |
| ^ | Start |
| $ | End |

---

# Example

```python
import re

text="abc123"

re.findall(r"\d+",text)
```

Output

```
['123']
```

---

# Common Uses

- Email Validation
- Password Validation
- Log Parsing
- Malware Detection
- File Searching

---

# Benefits

- Fast Searching
- Flexible Matching
- Automation

---

# 📌 Key Takeaways

- Regex searches text efficiently.
- re module provides regex support.
- Used in cybersecurity and automation.

---

# ❓ Interview Questions

### What is Regex?

A pattern matching language.

### Which module provides Regex?

re

### Name two Regex functions.

re.search()

re.findall()

---

# 📝 Summary

Today I learned about Regular Expressions, pattern matching, searching, validation, and text extraction using Python's re module.
