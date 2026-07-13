# Day 23: Port Scanner (Mini Project)

> Understanding Port Scanning, TCP ports, socket programming, and building a basic Port Scanner using Python.

---

# 🎯 Learning Objectives

- Understand Port Scanning.
- Learn Open and Closed Ports.
- Build a Simple Port Scanner.
- Understand TCP Connections.
- Prepare for cybersecurity interviews.

---

# 📖 Introduction

Every network service runs on a specific port.

A Port Scanner checks whether a port is open, closed, or filtered.

Security professionals use port scanners to identify exposed services and verify system configurations.

---

# 🌐 What is a Port?

A Port is a communication endpoint used by applications.

Examples:

- HTTP → 80
- HTTPS → 443
- SSH → 22
- FTP → 21
- DNS → 53

---

# What is Port Scanning?

Port Scanning is the process of checking whether network ports are open.

It helps identify running services.

---

# Mini Project

## Python Code

```python
import socket

target = input("Enter Target IP: ")

for port in range(20, 31):
    s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
    s.settimeout(1)

    result = s.connect_ex((target, port))

    if result == 0:
        print(f"Port {port} is OPEN")

    s.close()
```

---

# How It Works

- Creates a TCP socket.
- Tries connecting to each port.
- Reports open ports.
- Closes the connection.

---

# Cybersecurity Uses

- Security Audits
- Network Administration
- Vulnerability Assessment
- Service Discovery

---

# Best Practices

- Scan only systems you own or have permission to test.
- Use responsible scanning techniques.
- Document scan results.

---

# 📌 Key Takeaways

- Every service listens on a port.
- Port scanners identify exposed services.
- Python sockets enable network scanning.

---

# ❓ Interview Questions

### 1. What is Port Scanning?

Checking whether network ports are open.

### 2. Which module is used?

socket

### 3. Which protocol is commonly used?

TCP

### 4. Why is port scanning important?

To identify available network services.

### 5. Which port does SSH use?

22

---

# 📝 Summary

Today I built a simple Port Scanner using Python sockets. It demonstrates how security professionals identify running services and verify network configurations.
