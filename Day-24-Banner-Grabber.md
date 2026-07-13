# Day 24: Banner Grabber (Mini Project)

> Understanding Banner Grabbing, service identification, and using Python sockets to retrieve service information.

---

# 🎯 Learning Objectives

- Understand Banner Grabbing.
- Learn Service Enumeration.
- Build a Banner Grabber.
- Identify Running Services.
- Prepare for cybersecurity interviews.

---

# 📖 Introduction

Many servers send a banner when a client connects.

The banner may reveal:

- Software Name
- Version
- Service Type

Security professionals use this information to identify systems during authorized assessments.

---

# 🌐 What is Banner Grabbing?

Banner Grabbing retrieves information provided by a network service when a connection is established.

---

# Example Banner

```
SSH-2.0-OpenSSH_9.0
```

---

# Mini Project

## Python Code

```python
import socket

target = input("Enter Target IP: ")

port = 22

client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
client.connect((target, port))

banner = client.recv(1024)

print(banner.decode())

client.close()
```

---

# How It Works

- Connects to a server.
- Receives the service banner.
- Displays server information.

---

# Cybersecurity Uses

- Service Identification
- Asset Inventory
- Security Audits
- Vulnerability Assessment

---

# Best Practices

- Perform banner grabbing only on authorized systems.
- Validate results.
- Document discovered services.

---

# 📌 Key Takeaways

- Banners reveal service information.
- Banner grabbing helps identify systems.
- Python sockets simplify network communication.

---

# ❓ Interview Questions

### 1. What is Banner Grabbing?

Retrieving information from a network service.

### 2. Which Python module is used?

socket

### 3. Why do servers send banners?

To identify the service and protocol.

### 4. What information may be revealed?

Software name and version.

### 5. Why is banner grabbing useful?

To identify services running on a system.

---

# 📝 Summary

Today I built a simple Banner Grabber using Python sockets. Banner grabbing helps identify services running on authorized systems and supports security assessments.
