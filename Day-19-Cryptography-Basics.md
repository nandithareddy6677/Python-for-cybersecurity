# Day 19: Cryptography Basics

> Understanding Cryptography, hashing, encoding, Base64, hashlib, encryption concepts, and secure data protection.

---

# 🎯 Learning Objectives

- Understand Cryptography.
- Learn Hashing.
- Explore Base64 Encoding.
- Use hashlib.
- Prepare for cybersecurity interviews.

---

# 📖 Introduction

Cryptography protects sensitive information from unauthorized access.

It is widely used for passwords, digital signatures, secure communication, and authentication.

---

# 🔐 What is Cryptography?

Cryptography is the practice of securing information using mathematical techniques.

Goals:

- Confidentiality
- Integrity
- Authentication
- Non-Repudiation

---

# Hashing

Hashing converts data into a fixed-length value.

Characteristics:

- One-way process
- Fixed Output
- Used for Password Storage

---

# hashlib Module

```python
import hashlib
```

---

# SHA-256 Example

```python
hashlib.sha256()
```

---

# MD5

Older hashing algorithm.

Not recommended for secure applications.

---

# SHA Family

- SHA-1 (Deprecated)
- SHA-256
- SHA-384
- SHA-512

---

# Base64 Encoding

Base64 converts binary data into readable text.

It is **encoding**, not encryption.

---

# base64 Module

```python
import base64
```

---

# Encoding

```python
base64.b64encode()
```

---

# Decoding

```python
base64.b64decode()
```

---

# Difference

| Hashing | Encoding |
|----------|-----------|
| One-way | Reversible |
| Used for Integrity | Used for Data Representation |

---

# Cybersecurity Uses

- Password Storage
- File Verification
- Digital Signatures
- Certificates
- Secure Authentication

---

# Best Practices

- Use SHA-256 or stronger.
- Avoid MD5 for sensitive data.
- Never confuse Base64 with encryption.
- Store hashes securely.

---

# 📌 Key Takeaways

- Cryptography protects information.
- Hashing verifies integrity.
- Base64 is encoding.
- hashlib provides hashing functions.

---

# ❓ Interview Questions

### 1. What is Cryptography?

The practice of securing information.

### 2. What does hashlib provide?

Hashing algorithms.

### 3. Is Base64 encryption?

No, it is encoding.

### 4. Which hashing algorithm is commonly recommended?

SHA-256.

### 5. Why is MD5 discouraged?

It is vulnerable to collisions and no longer considered secure for cryptographic use.

---

# 📝 Summary

Today I learned about Cryptography, hashing, Base64 encoding, SHA-256, and Python's hashlib module. These concepts form the foundation of secure authentication, integrity checking, and data protection in cybersecurity applications.
