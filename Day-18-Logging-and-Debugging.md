# Day 18: Logging & Debugging

> Understanding Python logging, debugging techniques, error tracking, and application monitoring.

---

# 🎯 Learning Objectives

- Understand Logging.
- Learn Debugging.
- Track Errors.
- Improve Program Reliability.
- Prepare for Python interviews.

---

# 📖 Introduction

Debugging helps developers identify and fix errors.

Logging records application events for troubleshooting and monitoring.

Both are essential in cybersecurity and production systems.

---

# What is Logging?

Logging records events generated while a program runs.

Examples:

- Errors
- Warnings
- Login Attempts
- System Events

---

# logging Module

```python
import logging
```

---

# Basic Logging

```python
logging.basicConfig(level=logging.INFO)
```

---

# Log Levels

- DEBUG
- INFO
- WARNING
- ERROR
- CRITICAL

---

# Writing Logs

```python
logging.info("Program Started")
```

```python
logging.error("Invalid Input")
```

---

# Save Logs to File

```python
logging.basicConfig(filename="app.log")
```

---

# What is Debugging?

Debugging is the process of finding and fixing errors in code.

---

# Common Debugging Methods

- print()
- Logging
- IDE Debugger
- Exception Handling

---

# Cybersecurity Uses

- Monitor Login Attempts
- Track Malware Activity
- Audit Applications
- Investigate Incidents

---

# Best Practices

- Use meaningful log messages.
- Never log passwords.
- Rotate log files.
- Log important events only.

---

# 📌 Key Takeaways

- Logging records program activity.
- Debugging identifies software bugs.
- Log levels organize messages.
- Logging improves monitoring.

---

# ❓ Interview Questions

### 1. What is Logging?

Recording application events.

### 2. Which module provides logging?

logging

### 3. Name two log levels.

INFO and ERROR.

### 4. Why is logging important?

To monitor and troubleshoot applications.

### 5. Should passwords be logged?

No.

---

# 📝 Summary

Today I learned about Logging, Debugging, log levels, error tracking, and application monitoring. Logging is essential for troubleshooting and auditing cybersecurity applications.
