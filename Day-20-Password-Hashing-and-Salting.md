# Day 20: Password Hashing & Salting

> Understanding password hashing, salting, secure password storage, and Python libraries used for authentication.

---

# 🎯 Learning Objectives

- Understand Password Hashing.
- Learn Salting.
- Explore Secure Password Storage.
- Use hashlib and bcrypt.
- Prepare for cybersecurity interviews.

---

# 📖 Introduction

Passwords should never be stored in plain text.

Modern applications store password hashes instead of the original password to improve security.

---

# 🔐 What is Password Hashing?

Password Hashing converts a password into a fixed-length hash.

Example:

```
Password

↓

Hash Function

↓

Hashed Password
```

The original password cannot be easily recovered from the hash.

---

# Why Hash Passwords?

Benefits:

- Protects user credentials
- Prevents plain-text storage
- Improves authentication security

---

# What is Salting?

A Salt is random data added to a password before hashing.

Example:

```
Password

+

Random Salt

↓

Hash
```

---

# Benefits of Salting

- Prevents Rainbow Table Attacks
- Makes identical passwords produce different hashes
- Improves security

---

# hashlib Example

```python
import hashlib

password = "Secure123"

hash_value = hashlib.sha256(password.encode()).hexdigest()

print(hash_value)
```

---

# bcrypt

bcrypt automatically adds a random salt.

Install:

```bash
pip install bcrypt
```

---

# Hash Password

```python
import bcrypt

password = b"Secure123"

hashed = bcrypt.hashpw(password, bcrypt.gensalt())
```

---

# Verify Password

```python
bcrypt.checkpw(password, hashed)
```

---

# Cybersecurity Uses

- Login Systems
- User Authentication
- Identity Management
- Secure Applications

---

# Best Practices

- Never store plain-text passwords.
- Use bcrypt or Argon2.
- Always use unique salts.
- Enforce strong passwords.

---

# 📌 Key Takeaways

- Passwords should always be hashed.
- Salting increases security.
- bcrypt is recommended for password storage.
- Hashing protects user credentials.

---

# ❓ Interview Questions

### 1. What is Password Hashing?

Converting a password into a fixed-length hash.

### 2. What is Salting?

Adding random data before hashing.

### 3. Why is bcrypt preferred?

It automatically uses salts and is resistant to brute-force attacks.

### 4. Should passwords be encrypted or hashed?

They should be hashed for storage.

### 5. Why avoid storing plain-text passwords?

Because they can be stolen if the database is compromised.

---

# 📝 Summary

Today I learned about password hashing, salting, bcrypt, hashlib, and secure password storage. Proper password handling is essential for protecting user accounts and preventing credential theft.
