# Day 21: File Integrity Checker (Mini Project)

> Building a simple File Integrity Checker using Python and SHA-256 to verify whether a file has been modified.

---

# 🎯 Learning Objectives

- Understand File Integrity.
- Learn SHA-256 Verification.
- Build a Mini Project.
- Detect File Changes.

---

# 📖 Introduction

Organizations often verify whether files have been modified by malware or unauthorized users.

Hashing allows us to compare a file's current hash with its original hash.

---

# What is File Integrity?

File Integrity ensures that a file has not been modified.

---

# How it Works

```
Original File

↓

SHA-256 Hash

↓

Store Hash

↓

Compare Later

↓

Modified?

Yes / No
```

---

# Mini Project

## Python Code

```python
import hashlib

def calculate_hash(filename):
    sha256 = hashlib.sha256()

    with open(filename, "rb") as file:
        while True:
            chunk = file.read(4096)
            if not chunk:
                break
            sha256.update(chunk)

    return sha256.hexdigest()

print(calculate_hash("sample.txt"))
```

---

# How It Works

- Opens the file
- Reads it in chunks
- Calculates SHA-256
- Displays the hash

---

# Cybersecurity Uses

- Malware Detection
- File Verification
- Digital Forensics
- Software Integrity

---

# Best Practices

- Use SHA-256 or stronger.
- Verify hashes after downloads.
- Store hashes securely.

---

# 📌 Key Takeaways

- Hashes verify file integrity.
- SHA-256 is commonly used.
- File integrity checking detects unauthorized modifications.

---

# ❓ Interview Questions

### 1. What is File Integrity?

Ensuring a file has not been modified.

### 2. Which algorithm is commonly used?

SHA-256.

### 3. Why read files in chunks?

To efficiently process large files.

### 4. Which module provides SHA-256?

hashlib.

### 5. Where is file integrity used?

Malware detection and digital forensics.

---

# 📝 Summary

Today I built a File Integrity Checker using SHA-256. This project demonstrates how cybersecurity professionals verify whether important files have been modified.
