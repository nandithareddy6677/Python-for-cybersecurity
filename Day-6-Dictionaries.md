# Day 6: Python Dictionaries

> Understanding Python Dictionaries, key-value pairs, dictionary methods, nested dictionaries, and their real-world applications in automation, cloud computing, and cybersecurity.

---

# 🎯 Learning Objectives

- Understand Dictionaries.
- Learn Key-Value Pairs.
- Create and Modify Dictionaries.
- Access Dictionary Values.
- Learn Dictionary Methods.
- Understand Nested Dictionaries.
- Prepare for Python interviews.

---

# 📖 Introduction

A Dictionary is one of Python's most powerful data structures.

Unlike Lists, which store values using indexes, Dictionaries store data using **keys**.

Example:

Instead of:

```
Student

↓

Index 0 = Nanditha

Index 1 = 21
```

We can store:

```
Name → Nanditha

Age → 21
```

This makes data much easier to understand and manage.

---

# 📚 What is a Dictionary?

A Dictionary is an unordered, mutable collection of **key-value pairs**.

Example:

```python
student = {
    "name": "Nanditha",
    "age": 21,
    "country": "India"
}

print(student)
```

Output

```
{
'name':'Nanditha',
'age':21,
'country':'India'
}
```

---

# Characteristics of Dictionaries

- Mutable
- Stores Key-Value Pairs
- Keys are Unique
- Fast Searching
- Dynamic Size

---

# Accessing Dictionary Values

```python
student = {
    "name":"Nanditha",
    "age":21
}

print(student["name"])
```

Output

```
Nanditha
```

---

Using get()

```python
print(student.get("age"))
```

Output

```
21
```

---

# Adding New Items

```python
student["college"] = "JNTUH"

print(student)
```

Output

```
{
'name':'Nanditha',
'age':21,
'college':'JNTUH'
}
```

---

# Updating Values

```python
student["age"] = 22
```

Output

```
Age updated successfully.
```

---

# Removing Items

Using pop()

```python
student.pop("age")
```

---

Using del

```python
del student["country"]
```

---

Using clear()

```python
student.clear()
```

Removes all items.

---

# Dictionary Methods

| Method | Purpose |
|---------|----------|
| keys() | Returns all keys |
| values() | Returns all values |
| items() | Returns key-value pairs |
| get() | Returns value safely |
| update() | Updates dictionary |
| pop() | Removes item |
| clear() | Removes everything |

---

# Looping Through Dictionaries

Loop through Keys

```python
for key in student:

    print(key)
```

---

Loop through Values

```python
for value in student.values():

    print(value)
```

---

Loop through Both

```python
for key,value in student.items():

    print(key,value)
```

---

# Nested Dictionaries

A Dictionary can contain another Dictionary.

Example

```python
students = {

"student1":{

"name":"Nanditha",

"age":21

},

"student2":{

"name":"Rahul",

"age":22

}

}
```

Nested Dictionaries are widely used in APIs and JSON.

---

# Dictionary vs List

| Dictionary | List |
|------------|------|
| Uses Keys | Uses Index |
| Faster Search | Slower Search |
| Key-Value Pair | Values Only |
| Unique Keys | Duplicate Values Allowed |

---

# 🌍 Real-Life Example

Suppose you are building a login system.

```python
user = {

"username":"nanditha",

"password":"Python123",

"role":"Admin"

}
```

Instead of remembering indexes, we access values using meaningful keys.

---

# Dictionaries in Cybersecurity

A Dictionary can store user credentials.

```python
users = {

"admin":"admin123",

"user":"user123"

}
```

Authentication scripts frequently use dictionaries.

---

# Dictionaries in Cloud Computing

AWS responses are often returned as Dictionaries.

Example:

```python
instance = {

"InstanceId":"i-123456",

"State":"Running",

"Region":"ap-south-1"

}
```

Cloud Engineers work with dictionaries every day.

---

# Dictionaries in JSON

JSON objects are almost identical to Python Dictionaries.

Example JSON

```json
{

"name":"Nanditha",

"city":"Hyderabad"

}
```

Python

```python
{

"name":"Nanditha",

"city":"Hyderabad"

}
```

This is why dictionaries are essential for APIs.

---

# 💡 Best Practices

- Use meaningful key names.
- Avoid duplicate keys.
- Use get() instead of direct indexing when possible.
- Use nested dictionaries for structured data.
- Keep dictionaries readable.

---

# 📌 Key Takeaways

- Dictionaries store data using keys.
- Keys must be unique.
- Values can be duplicated.
- Dictionaries are mutable.
- Dictionaries provide fast lookup.
- APIs and JSON use dictionary-like structures.

---

# ❓ Interview Questions

### 1. What is a Dictionary?

A Dictionary is a mutable collection of key-value pairs.

---

### 2. Are Dictionary Keys unique?

Yes.

---

### 3. Which method safely retrieves a value?

```python
get()
```

---

### 4. Which method returns all keys?

```python
keys()
```

---

### 5. Which method returns key-value pairs?

```python
items()
```

---

### 6. Can Dictionaries contain Lists?

Yes.

---

### 7. Can Dictionaries contain other Dictionaries?

Yes.

---

### 8. Why are Dictionaries important?

Because they provide fast data retrieval and are widely used in APIs, JSON, cloud computing, automation, and cybersecurity.

---

# 📝 Summary

Today I learned about Python Dictionaries, one of the most powerful data structures in Python. I explored key-value pairs, dictionary methods, updating and deleting items, looping through dictionaries, nested dictionaries, and their use in APIs and JSON. Dictionaries are widely used in cloud computing, automation, cybersecurity, and software development because they provide fast and organized access to structured data.
