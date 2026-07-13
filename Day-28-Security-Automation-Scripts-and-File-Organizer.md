# Day 28: Security Automation Scripts & File Organizer

> Building simple automation scripts using Python to organize files, improve productivity, and automate repetitive security-related tasks.

---

# 🎯 Learning Objectives

- Understand Security Automation.
- Build a File Organizer.
- Automate Repetitive Tasks.
- Improve Productivity.
- Prepare for Python automation projects.

---

# 📖 Introduction

Automation reduces repetitive manual work.

Python enables administrators and security professionals to automate file management, log processing, reporting, and system maintenance.

---

# What is Security Automation?

Security Automation uses scripts to perform repetitive administrative or security tasks automatically.

Examples:

- Organizing Files
- Processing Logs
- Renaming Files
- Backup Automation
- Report Generation

---

# Mini Project: File Organizer

This script moves files into folders based on their file extension.

---

# Python Code

```python
import os
import shutil

source = "Downloads"

for file in os.listdir(source):

    path = os.path.join(source, file)

    if os.path.isfile(path):

        extension = file.split(".")[-1]

        destination = os.path.join(source, extension)

        os.makedirs(destination, exist_ok=True)

        shutil.move(path, os.path.join(destination, file))
```

---

# How It Works

- Reads all files in a folder.
- Detects file extensions.
- Creates folders automatically.
- Moves files into matching folders.

---

# Example

Before:

```
Downloads

↓

photo.jpg

report.pdf

notes.txt
```

After:

```
Downloads

↓

jpg/

↓

photo.jpg

pdf/

↓

report.pdf

txt/

↓

notes.txt
```

---

# Other Automation Ideas

- Backup Script
- Log File Organizer
- Duplicate File Finder
- Password Generator
- Network Health Checker

---

# Cybersecurity Uses

- Organize Log Files
- Backup Reports
- Incident Response
- Evidence Collection
- Report Automation

---

# Best Practices

- Test scripts on sample data first.
- Create backups before moving files.
- Handle errors gracefully.
- Log important actions.

---

# 📌 Key Takeaways

- Python simplifies automation.
- File organization improves efficiency.
- Automation reduces manual work.
- Security teams rely heavily on scripting.

---

# ❓ Interview Questions

### 1. What is Security Automation?

Using scripts to automate repetitive security or administrative tasks.

### 2. Which module moves files?

shutil

### 3. Which module accesses directories?

os

### 4. Why automate file organization?

To improve efficiency and consistency.

### 5. Name one cybersecurity use of automation.

Log management.

---

# 📝 Summary

Today I learned about Security Automation and built a File Organizer using Python. Automation helps reduce manual effort, improve productivity, and streamline administrative and cybersecurity workflows.
