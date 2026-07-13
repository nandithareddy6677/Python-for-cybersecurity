# Day 14: Working with APIs & Requests

> Understanding APIs, HTTP requests, REST APIs, JSON responses, and using Python's requests module to interact with web services.

---

# 🎯 Learning Objectives

- Understand APIs.
- Learn REST APIs.
- Use the requests module.
- Send HTTP Requests.
- Process JSON Responses.
- Prepare for automation projects.

---

# 📖 Introduction

Modern applications communicate through APIs (Application Programming Interfaces).

Python can interact with APIs to retrieve data, automate tasks, and integrate different services.

---

# 🌐 What is an API?

An API allows one application to communicate with another.

Example:

```
Python Script

↓

API Request

↓

Server

↓

Response
```

---

# REST API

REST APIs communicate using HTTP methods.

Common Methods:

- GET
- POST
- PUT
- DELETE

---

# requests Module

Install:

```bash
pip install requests
```

Import:

```python
import requests
```

---

# GET Request

```python
response = requests.get("https://api.example.com")
```

---

# POST Request

```python
requests.post(url,data=data)
```

---

# Status Code

```python
response.status_code
```

Common Codes:

- 200 OK
- 201 Created
- 400 Bad Request
- 401 Unauthorized
- 404 Not Found
- 500 Internal Server Error

---

# JSON Response

```python
response.json()
```

---

# Headers

```python
headers={"Authorization":"Bearer Token"}
```

---

# Cybersecurity Uses

- Threat Intelligence APIs
- VirusTotal
- Shodan
- AbuseIPDB
- Automation Scripts

---

# Best Practices

- Validate responses.
- Handle exceptions.
- Protect API keys.
- Respect rate limits.

---

# 📌 Key Takeaways

- APIs connect applications.
- requests simplifies HTTP communication.
- JSON is commonly used.
- APIs are widely used in cybersecurity automation.

---

# ❓ Interview Questions

### 1. What is an API?

A method for applications to communicate.

### 2. Which Python library is commonly used for APIs?

requests

### 3. Name two HTTP methods.

GET and POST.

### 4. Which status code indicates success?

200

### 5. Which method converts JSON to Python?

response.json()

---

# 📝 Summary

Today I learned about APIs, REST APIs, HTTP requests, JSON responses, and Python's requests module. APIs are essential for automation, cloud computing, and cybersecurity.
