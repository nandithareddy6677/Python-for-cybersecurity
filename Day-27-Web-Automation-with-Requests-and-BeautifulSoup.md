# Day 27: Web Automation with requests & BeautifulSoup

> Understanding web automation, HTTP requests, HTML parsing, web scraping, and extracting information using Python.

---

# 🎯 Learning Objectives

- Understand Web Automation.
- Learn requests.
- Learn BeautifulSoup.
- Parse HTML.
- Extract Website Information.
- Prepare for automation projects.

---

# 📖 Introduction

Many repetitive web tasks can be automated using Python.

Python can retrieve web pages, extract useful information, and automate data collection from websites that permit automated access.

---

# 🌐 What is Web Automation?

Web Automation refers to using programs to interact with websites automatically.

Common tasks:

- Retrieve Web Pages
- Extract Information
- Monitor Websites
- Generate Reports

---

# requests Library

Install:

```bash
pip install requests
```

Example:

```python
import requests

response = requests.get("https://example.com")

print(response.status_code)
```

---

# BeautifulSoup

Install:

```bash
pip install beautifulsoup4
```

Import:

```python
from bs4 import BeautifulSoup
```

---

# Parse HTML

```python
soup = BeautifulSoup(response.text,"html.parser")
```

---

# Extract Title

```python
print(soup.title.text)
```

---

# Extract Links

```python
for link in soup.find_all("a"):
    print(link.get("href"))
```

---

# Extract Paragraphs

```python
for p in soup.find_all("p"):
    print(p.text)
```

---

# Cybersecurity Uses

- Security Monitoring
- Public Information Collection
- Threat Intelligence
- Website Availability Monitoring

---

# Best Practices

- Respect website Terms of Service.
- Avoid excessive requests.
- Handle exceptions.
- Verify collected information.

---

# 📌 Key Takeaways

- requests retrieves web pages.
- BeautifulSoup parses HTML.
- Python automates repetitive web tasks.
- Web automation supports monitoring and reporting.

---

# ❓ Interview Questions

### 1. What does requests do?

Sends HTTP requests.

### 2. What is BeautifulSoup?

A Python library for parsing HTML.

### 3. Which parser is commonly used?

html.parser

### 4. Which function extracts links?

find_all("a")

### 5. Why automate web tasks?

To save time and collect information efficiently.

---

# 📝 Summary

Today I learned about Web Automation, requests, BeautifulSoup, HTML parsing, and extracting website information using Python. These tools are widely used for automation, monitoring, and data collection.
