# Day 22: Password Strength Checker (Mini Project)

> Building a Password Strength Checker using Python to evaluate password security based on common best practices.

---

# 🎯 Learning Objectives

- Understand Strong Passwords.
- Build a Password Checker.
- Validate Password Rules.
- Improve Authentication Security.

---

# 📖 Introduction

Weak passwords are one of the most common causes of security breaches.

A Password Strength Checker helps users create stronger passwords.

---

# Strong Password Requirements

- Minimum 8 characters
- Uppercase Letter
- Lowercase Letter
- Number
- Special Character

---

# Mini Project

## Python Code

```python
import re

password = input("Enter Password: ")

if (len(password) >= 8 and
    re.search(r"[A-Z]", password) and
    re.search(r"[a-z]", password) and
    re.search(r"[0-9]", password) and
    re.search(r"[!@#$%^&*(),.?\":{}|<>]", password)):
    print("Strong Password")
else:
    print("Weak Password")
```

---

# How It Works

- Checks password length.
- Verifies uppercase letters.
- Verifies lowercase letters.
- Checks numbers.
- Detects special characters.

---

# Cybersecurity Uses

- Login Systems
- User Registration
- Password Policies
- Identity Management

---

# Best Practices

- Use passphrases.
- Avoid dictionary words.
- Enable MFA.
- Never reuse passwords.

---

# 📌 Key Takeaways

- Strong passwords reduce security risks.
- Python can automatically validate passwords.
- Regular expressions simplify password checking.

---

# ❓ Interview Questions

### 1. What makes a password strong?

Length, uppercase, lowercase, numbers, and special characters.

### 2. Which module is used for pattern matching?

re

### 3. Why are weak passwords dangerous?

They are easier to guess or crack.

### 4. Should passwords be reused?

No.

### 5. What additional protection should users enable?

Multi-Factor Authentication (MFA).

---

# 📝 Summary

Today I built a Password Strength Checker using Python and Regular Expressions. This project demonstrates how Python can enforce secure password policies and improve user authentication.
