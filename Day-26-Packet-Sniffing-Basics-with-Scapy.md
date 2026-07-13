# Day 26: Packet Sniffing Basics (Scapy Introduction)

> Understanding packet sniffing, network packets, Scapy, packet analysis, and basic network monitoring using Python.

---

# 🎯 Learning Objectives

- Understand Packet Sniffing.
- Learn Scapy.
- Capture Network Packets.
- Analyze Packet Information.
- Prepare for cybersecurity interviews.

---

# 📖 Introduction

Every communication over a network is broken into small units called packets.

Network administrators and security analysts inspect these packets to troubleshoot networks and investigate suspicious activity.

Python's **Scapy** library is one of the most popular tools for packet analysis and network testing.

---

# 🌐 What is Packet Sniffing?

Packet Sniffing is the process of capturing and inspecting network traffic flowing through a network interface.

Captured packets may contain:

- Source IP
- Destination IP
- Protocol
- Port Number
- Packet Size

---

# What is Scapy?

Scapy is a powerful Python library used for:

- Packet Capture
- Packet Analysis
- Packet Creation
- Network Testing
- Security Research

Install:

```bash
pip install scapy
```

---

# Import Scapy

```python
from scapy.all import *
```

---

# Capture Packets

```python
from scapy.all import sniff

sniff(count=5)
```

---

# Display Packet Summary

```python
sniff(count=5, prn=lambda packet: packet.summary())
```

---

# Filter TCP Packets

```python
sniff(filter="tcp", count=10)
```

---

# Common Protocols

- TCP
- UDP
- ICMP
- ARP
- DNS
- HTTP

---

# Cybersecurity Uses

- Network Troubleshooting
- Traffic Monitoring
- Malware Analysis
- Security Auditing
- Incident Response

---

# Best Practices

- Capture traffic only on networks you own or are authorized to monitor.
- Secure packet capture files.
- Respect privacy policies.
- Analyze captured data responsibly.

---

# 📌 Key Takeaways

- Packets carry network data.
- Scapy simplifies packet analysis.
- Packet sniffing supports troubleshooting and security monitoring.
- Network analysis is an essential cybersecurity skill.

---

# ❓ Interview Questions

### 1. What is Packet Sniffing?

Capturing and analyzing network packets.

### 2. What is Scapy?

A Python library for packet manipulation and analysis.

### 3. Which function captures packets?

sniff()

### 4. Name three protocols Scapy can analyze.

TCP, UDP, ICMP.

### 5. Why is packet analysis important?

To troubleshoot networks and investigate security incidents.

---

# 📝 Summary

Today I learned about Packet Sniffing, Scapy, packet capture, packet analysis, and network monitoring. Scapy is a powerful Python library used for understanding and analyzing network traffic in cybersecurity and network administration.
