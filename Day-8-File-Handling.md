# Day 8: File Handling

> Understanding Python File Handling, reading and writing files, file modes, working with text files, CSV files, and real-world applications in automation, cloud computing, and cybersecurity.

---

# 🎯 Learning Objectives

- Understand File Handling.
- Learn how to open files.
- Read data from files.
- Write data to files.
- Understand File Modes.
- Learn the with statement.
- Work with CSV files.
- Prepare for Python interviews.

---

# 📖 Introduction

Most real-world Python applications work with files.

Examples include:

- Reading log files
- Saving reports
- Reading configuration files
- Processing CSV data
- Writing automation logs

Python provides simple and powerful tools to work with files.

---

# 📂 What is File Handling?

File Handling is the process of creating, opening, reading, writing, updating, and deleting files.

Python supports many file types, including:

- Text Files (.txt)
- CSV Files (.csv)
- JSON Files (.json)
- Log Files (.log)
- XML Files (.xml)

---

# Opening a File

The `open()` function is used to open a file.

Syntax

```python
file = open("sample.txt", "r")
```

---

# File Modes

| Mode | Description |
|------|-------------|
| r | Read |
| w | Write (Creates or Overwrites) |
| a | Append |
| x | Create New File |
| r+ | Read and Write |
| b | Binary Mode |

---

# Reading a File

```python
file = open("sample.txt", "r")

print(file.read())

file.close()
```

Output

```
Hello Python
Welcome to File Handling
```

---

# Reading Line by Line

```python
file = open("sample.txt", "r")

print(file.readline())

file.close()
```

Reads only one line.

---

# Reading All Lines

```python
file = open("sample.txt", "r")

print(file.readlines())

file.close()
```

Output

```python
['Hello\n', 'Welcome\n']
```

---

# Writing to a File

Mode:

```
w
```

Example

```python
file = open("sample.txt", "w")

file.write("Hello Python")

file.close()
```

If the file already exists, its previous content will be replaced.

---

# Appending to a File

Mode

```
a
```

Example

```python
file = open("sample.txt", "a")

file.write("\nPython Automation")

file.close()
```

Output

```
Hello Python
Python Automation
```

---

# Creating a New File

Mode

```
x
```

Example

```python
file = open("notes.txt", "x")
```

Python creates a new file.

If the file already exists, an error occurs.

---

# Closing a File

Always close files after use.

```python
file.close()
```

Closing releases system resources.

---

# The with Statement

The recommended way to work with files.

Example

```python
with open("sample.txt", "r") as file:

    print(file.read())
```

Advantages

- Automatically closes the file
- Cleaner code
- Prevents resource leaks

---

# Working with CSV Files

Python provides the `csv` module.

Example

```python
import csv

with open("students.csv", "r") as file:

    reader = csv.reader(file)

    for row in reader:

        print(row)
```

CSV files are widely used for reports and datasets.

---

# Checking if a File Exists

```python
import os

print(os.path.exists("sample.txt"))
```

Output

```
True
```

---

# File Handling Errors

Trying to open a missing file results in:

```python
FileNotFoundError
```

Example

```python
open("abc.txt","r")
```

Output

```
FileNotFoundError
```

---

# 🌍 Real-Life Example

Suppose a cybersecurity analyst wants to read login logs.

```python
with open("logs.txt","r") as file:

    for line in file:

        print(line)
```

The script reads every log entry automatically.

---

# File Handling in Cybersecurity

File Handling is used for:

- Reading Log Files
- Malware Analysis
- Password Lists
- Security Reports
- Configuration Files
- Threat Intelligence Data

---

# File Handling in Cloud Computing

Cloud Engineers use File Handling for:

- Reading Configuration Files
- Managing Logs
- Processing CSV Reports
- Reading JSON Files
- Deployment Scripts

---

# 💡 Best Practices

- Use the `with` statement whenever possible.
- Always close files if not using `with`.
- Handle missing files gracefully.
- Use meaningful file names.
- Avoid overwriting important files unintentionally.

---

# 📌 Key Takeaways

- `open()` opens files.
- Different file modes serve different purposes.
- `read()`, `readline()`, and `readlines()` retrieve file contents.
- `write()` overwrites content.
- `append()` adds new content.
- `with` automatically closes files.
- File Handling is essential for automation and cybersecurity.

---

# ❓ Interview Questions

### 1. What is File Handling?

File Handling is the process of creating, reading, writing, updating, and deleting files.

---

### 2. Which function opens a file?

```python
open()
```

---

### 3. Which mode is used for reading?

```python
r
```

---

### 4. Which mode appends data?

```python
a
```

---

### 5. Which mode creates a new file?

```python
x
```

---

### 6. Why is the `with` statement recommended?

It automatically closes the file and prevents resource leaks.

---

### 7. Which module is commonly used to work with CSV files?

```python
csv
```

---

### 8. Which exception occurs when a file does not exist?

```python
FileNotFoundError
```

---

# 📝 Summary

Today I learned about Python File Handling and how to work with files using different modes. I explored reading, writing, appending, creating files, using the `with` statement, and working with CSV files. File Handling is an essential skill in Python because it is widely used for processing logs, reports, configuration files, and automation tasks in cloud computing, cybersecurity, and software development.
