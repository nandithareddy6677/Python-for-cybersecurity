# Day 9: Exception Handling

> Understanding Python Exceptions, handling runtime errors, using try-except blocks, raising exceptions, and writing robust programs.

---

# 🎯 Learning Objectives

- Understand Exceptions.
- Learn why Exception Handling is important.
- Use try and except blocks.
- Learn else and finally.
- Raise custom exceptions.
- Handle multiple exceptions.
- Prepare for Python interviews.

---

# 📖 Introduction

Errors are a normal part of programming.

Sometimes a program crashes because of:

- Invalid user input
- Missing files
- Division by zero
- Network problems

Python provides **Exception Handling** to prevent programs from crashing unexpectedly.

---

# 🚨 What is an Exception?

An Exception is an error that occurs while a program is running.

Example:

```python
print(10/0)
```

Output

```
ZeroDivisionError
```

---

# Why Exception Handling?

Without Exception Handling:

- Program crashes.
- Remaining code is not executed.

With Exception Handling:

- Program continues execution.
- Errors are handled gracefully.

---

# try and except

Example

```python
try:
    num = 10/0

except ZeroDivisionError:
    print("Cannot divide by zero.")
```

Output

```
Cannot divide by zero.
```

---

# Handling Multiple Exceptions

```python
try:
    number = int(input("Enter Number:"))

except ValueError:
    print("Invalid Number")

except KeyboardInterrupt:
    print("Program Interrupted")
```

---

# else Block

Runs only if no exception occurs.

```python
try:
    num = 20/5

except:
    print("Error")

else:
    print("Success")
```

Output

```
Success
```

---

# finally Block

Always executes.

```python
try:
    file = open("sample.txt")

except:
    print("File Not Found")

finally:
    print("Program Finished")
```

---

# Raising Exceptions

Use `raise` to create your own exceptions.

```python
age = 15

if age < 18:
    raise Exception("Not Eligible")
```

---

# Common Python Exceptions

| Exception | Description |
|------------|-------------|
| ZeroDivisionError | Divide by zero |
| ValueError | Invalid value |
| TypeError | Wrong data type |
| NameError | Variable not found |
| IndexError | Invalid list index |
| KeyError | Invalid dictionary key |
| FileNotFoundError | File not found |

---

# 🌍 Real-Life Example

Login System

```python
try:
    password = input("Password: ")

    if password != "admin123":
        raise Exception("Invalid Password")

except Exception as e:
    print(e)
```

---

# Exception Handling in Cybersecurity

Used for:

- Log Analysis
- Network Connections
- API Requests
- File Processing
- Malware Analysis

---

# Exception Handling in Cloud Computing

Used for:

- AWS API Errors
- Server Failures
- File Upload Errors
- Database Connections

---

# 💡 Best Practices

- Catch specific exceptions.
- Avoid using bare except.
- Use finally for cleanup.
- Write meaningful error messages.
- Don't ignore exceptions silently.

---

# 📌 Key Takeaways

- Exceptions are runtime errors.
- try handles risky code.
- except catches errors.
- else runs when no error occurs.
- finally always executes.
- raise creates custom exceptions.

---

# ❓ Interview Questions

### 1. What is an Exception?

An Exception is an error that occurs during program execution.

---

### 2. Why is Exception Handling important?

It prevents programs from crashing and allows graceful error handling.

---

### 3. Which keyword handles exceptions?

```python
except
```

---

### 4. Which block always executes?

```python
finally
```

---

### 5. Which keyword creates custom exceptions?

```python
raise
```

---

### 6. What is ZeroDivisionError?

It occurs when a number is divided by zero.

---

### 7. What is FileNotFoundError?

It occurs when Python cannot find the specified file.

---

### 8. What is the purpose of finally?

It executes cleanup code regardless of whether an exception occurs.

---

# 📝 Summary

Today I learned about Python Exception Handling. I explored try, except, else, finally, raising custom exceptions, and common runtime errors. Exception Handling improves program reliability and is widely used in cybersecurity, cloud computing, automation, and software development.
