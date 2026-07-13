# Day 16: Networking with Python (Socket Programming)

> Understanding socket programming, TCP and UDP communication, client-server architecture, and network programming using Python.

---

# 🎯 Learning Objectives

- Understand Socket Programming.
- Learn TCP and UDP.
- Explore Client-Server Communication.
- Build Basic Network Applications.
- Prepare for cybersecurity interviews.

---

# 📖 Introduction

Networking is an important part of cybersecurity.

Python's socket module allows applications to communicate over networks.

---

# 🌐 What is a Socket?

A Socket is an endpoint for communication between two devices over a network.

---

# Client-Server Model

```
Client

↓

Network

↓

Server
```

---

# Socket Module

```python
import socket
```

---

# Create a Socket

```python
socket.socket()
```

---

# TCP

Characteristics:

- Connection-Oriented
- Reliable
- Error Checking
- Ordered Delivery

Examples:

- HTTP
- HTTPS
- FTP
- SSH

---

# UDP

Characteristics:

- Connectionless
- Faster
- Lower Overhead
- No Delivery Guarantee

Examples:

- DNS
- Streaming
- VoIP

---

# Basic Client Example

```python
client = socket.socket()
```

---

# Basic Server Example

```python
server = socket.socket()
```

---

# Cybersecurity Uses

- Port Scanners
- Banner Grabbers
- Network Monitoring
- Vulnerability Assessment
- Security Automation

---

# Best Practices

- Validate input.
- Close sockets properly.
- Handle exceptions.
- Avoid exposing unnecessary services.

---

# 📌 Key Takeaways

- Sockets enable network communication.
- TCP is reliable.
- UDP is faster.
- Python supports networking through the socket module.

---

# ❓ Interview Questions

### 1. What is a Socket?

An endpoint used for network communication.

### 2. Which module provides socket programming?

socket

### 3. Difference between TCP and UDP?

TCP is reliable; UDP is faster but does not guarantee delivery.

### 4. Name one cybersecurity use of sockets.

Port Scanning.

### 5. What architecture does socket programming commonly use?

Client-Server Architecture.

---

# 📝 Summary

Today I learned about socket programming, TCP, UDP, client-server communication, and Python's socket module. Socket programming forms the foundation for many cybersecurity tools such as port scanners, network monitors, and vulnerability assessment scripts.
