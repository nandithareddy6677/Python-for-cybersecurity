# Day 25: Network Information Gathering

> Understanding network reconnaissance, hostname resolution, IP address lookup, and collecting basic network information using Python.

---

# 🎯 Learning Objectives

- Understand Network Reconnaissance.
- Resolve Hostnames.
- Retrieve IP Addresses.
- Learn Basic Information Gathering.
- Prepare for cybersecurity interviews.

---

# 📖 Introduction

Before securing a network, administrators first identify available hosts and services.

Information gathering is the first phase of many security assessments and troubleshooting workflows.

---

# 🌐 What is Network Information Gathering?

Network Information Gathering is the process of collecting publicly available or locally accessible network information about systems.

Examples include:

- Hostname
- IP Address
- Domain Name
- Open Services

---

# Hostname Resolution

Convert a hostname into an IP address.

---

# Mini Project

## Python Code

```python
import socket

host = input("Enter Website: ")

ip = socket.gethostbyname(host)

print("IP Address:", ip)
```

---

# Reverse Lookup

```python
socket.gethostbyaddr(ip)
```

---

# Get Local Hostname

```python
socket.gethostname()
```

---

# Get Local IP Address

```python
socket.gethostbyname(socket.gethostname())
```

---

# Cybersecurity Uses

- Network Discovery
- Asset Identification
- Troubleshooting
- Security Audits

---

# Best Practices

- Collect only authorized information.
- Verify results.
- Respect privacy and organizational policies.

---

# 📌 Key Takeaways

- Hostnames map to IP addresses.
- Python's socket module performs DNS lookups.
- Information gathering supports administration and security.

---

# ❓ Interview Questions

### 1. What is Network Information Gathering?

Collecting information about network systems.

### 2. Which module performs hostname lookups?

socket

### 3. Which function converts a hostname to an IP?

socket.gethostbyname()

### 4. What is DNS?

The Domain Name System that translates hostnames into IP addresses.

### 5. Why is information gathering important?

It helps understand network infrastructure and supports troubleshooting and security assessments.

---

# 📝 Summary

Today I learned about network information gathering, hostname resolution, DNS lookups, and Python's socket module. These techniques help administrators and security professionals better understand and manage network environments.
