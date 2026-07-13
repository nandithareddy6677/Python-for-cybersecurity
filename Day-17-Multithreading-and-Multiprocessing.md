# Day 17: Multithreading & Multiprocessing

> Understanding Multithreading, Multiprocessing, concurrency, parallel execution, and their use in cybersecurity automation.

---

# 🎯 Learning Objectives

- Understand Threads.
- Learn Processes.
- Compare Multithreading and Multiprocessing.
- Improve Program Performance.
- Prepare for Python interviews.

---

# 📖 Introduction

Some Python programs need to perform multiple tasks simultaneously.

Examples include scanning multiple IP addresses, downloading files, or monitoring network traffic.

Python supports this using Multithreading and Multiprocessing.

---

# What is Multithreading?

Multithreading allows multiple threads to run within the same process.

Example:

```
Program

↓

Thread 1

Thread 2

Thread 3
```

---

# Thread

A Thread is the smallest unit of execution within a process.

Threads share:

- Memory
- Variables
- Resources

---

# threading Module

```python
import threading
```

---

# Creating a Thread

```python
thread = threading.Thread(target=function)
```

Start thread:

```python
thread.start()
```

---

# What is Multiprocessing?

Multiprocessing creates multiple independent processes.

Each process has its own memory.

---

# multiprocessing Module

```python
import multiprocessing
```

---

# Creating a Process

```python
process = multiprocessing.Process(target=function)
```

Start:

```python
process.start()
```

---

# Multithreading vs Multiprocessing

| Multithreading | Multiprocessing |
|---------------|----------------|
| Shared Memory | Separate Memory |
| Lightweight | More Resource Usage |
| Faster Context Switching | Better CPU Utilization |
| Best for I/O Tasks | Best for CPU Tasks |

---

# Cybersecurity Uses

- Port Scanners
- Password Testing
- Network Monitoring
- Vulnerability Scanning
- Log Processing

---

# Best Practices

- Avoid unnecessary threads.
- Synchronize shared resources.
- Use multiprocessing for CPU-intensive work.
- Handle exceptions.

---

# 📌 Key Takeaways

- Threads share memory.
- Processes have separate memory.
- Multithreading is ideal for I/O tasks.
- Multiprocessing improves CPU performance.

---

# ❓ Interview Questions

### 1. What is Multithreading?

Running multiple threads within one process.

### 2. What is Multiprocessing?

Running multiple independent processes.

### 3. Which module creates threads?

threading

### 4. Which module creates processes?

multiprocessing

### 5. When is multiprocessing preferred?

For CPU-intensive tasks.

---

# 📝 Summary

Today I learned about Multithreading, Multiprocessing, concurrency, and parallel execution. These techniques improve the performance of automation scripts and cybersecurity tools.
