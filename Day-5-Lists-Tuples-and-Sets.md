# Day 5: Lists, Tuples, and Sets

> Understanding Python Collections including Lists, Tuples, and Sets, their properties, operations, methods, and real-world applications in cybersecurity and automation.

---

# 🎯 Learning Objectives

- Understand Python Collections.
- Learn about Lists.
- Learn about Tuples.
- Learn about Sets.
- Compare Lists, Tuples, and Sets.
- Learn commonly used methods.
- Prepare for Python interviews.

---

# 📖 Introduction

Python provides several built-in data structures called **Collections**.

Collections allow us to store multiple values in a single variable.

The three most commonly used collections are:

- List
- Tuple
- Set

Each has different characteristics and use cases.

---

# 📚 What is a List?

A List is an ordered, mutable (changeable) collection of items.

Lists can store:

- Integers
- Strings
- Floats
- Boolean values
- Objects
- Even other Lists

Example:

```python
fruits = ["Apple", "Banana", "Orange"]

print(fruits)
```

Output

```
['Apple', 'Banana', 'Orange']
```

---

# Characteristics of Lists

- Ordered
- Mutable
- Allows Duplicate Values
- Indexed
- Dynamic Size

---

# Accessing List Elements

```python
numbers = [10,20,30,40]

print(numbers[0])

print(numbers[2])
```

Output

```
10

30
```

---

# Negative Indexing

```python
numbers = [10,20,30,40]

print(numbers[-1])
```

Output

```
40
```

---

# Modifying Lists

```python
colors = ["Red","Blue","Green"]

colors[1] = "Black"

print(colors)
```

Output

```
['Red', 'Black', 'Green']
```

---

# Adding Elements

Using append()

```python
numbers = [1,2,3]

numbers.append(4)

print(numbers)
```

Output

```
[1,2,3,4]
```

---

Using insert()

```python
numbers.insert(1,100)
```

Output

```
[1,100,2,3,4]
```

---

# Removing Elements

Using remove()

```python
numbers.remove(2)
```

Using pop()

```python
numbers.pop()
```

Using del

```python
del numbers[0]
```

---

# List Slicing

```python
numbers = [10,20,30,40,50]

print(numbers[1:4])
```

Output

```
[20,30,40]
```

---

# Useful List Methods

| Method | Purpose |
|---------|----------|
| append() | Add element |
| insert() | Insert element |
| remove() | Remove value |
| pop() | Remove by index |
| sort() | Sort list |
| reverse() | Reverse list |
| count() | Count occurrences |
| clear() | Remove all elements |

---

# What is a Tuple?

A Tuple is an ordered but immutable (unchangeable) collection.

Example

```python
student = ("Nanditha",21,"India")

print(student)
```

Output

```
('Nanditha',21,'India')
```

---

# Characteristics of Tuples

- Ordered
- Immutable
- Allows Duplicates
- Indexed
- Faster than Lists

---

# Accessing Tuple Elements

```python
student = ("Nanditha",21)

print(student[0])
```

Output

```
Nanditha
```

---

# Why Use Tuples?

Use Tuples when data should not change.

Examples

- Coordinates
- Months
- Days of Week
- Configuration Values

---

# Tuple Methods

Only two methods are available.

```python
count()

index()
```

---

# What is a Set?

A Set is an unordered collection of unique elements.

Example

```python
numbers = {1,2,3,4}

print(numbers)
```

---

# Characteristics of Sets

- Unordered
- Mutable
- No Duplicate Values
- Fast Searching

---

# Adding Elements

```python
numbers.add(5)
```

---

# Removing Elements

```python
numbers.remove(3)
```

or

```python
numbers.discard(3)
```

---

# Set Operations

Union

```python
A = {1,2,3}

B = {3,4,5}

print(A | B)
```

Output

```
{1,2,3,4,5}
```

---

Intersection

```python
print(A & B)
```

Output

```
{3}
```

---

Difference

```python
print(A - B)
```

Output

```
{1,2}
```

---

# List vs Tuple vs Set

| Feature | List | Tuple | Set |
|---------|------|--------|------|
| Ordered | Yes | Yes | No |
| Mutable | Yes | No | Yes |
| Duplicates | Yes | Yes | No |
| Indexed | Yes | Yes | No |

---

# 🌍 Real-Life Example

Suppose you're writing a cybersecurity script.

A List stores detected IP addresses:

```python
ips = ["192.168.1.1","10.0.0.5"]
```

A Tuple stores fixed server information:

```python
server = ("WebServer",443)
```

A Set stores unique suspicious IP addresses:

```python
blocked = {"192.168.1.100","10.0.0.20"}
```

Each collection serves a different purpose.

---

# 💡 Best Practices

- Use Lists when data changes frequently.
- Use Tuples for fixed values.
- Use Sets to remove duplicates.
- Choose the correct collection based on the problem.
- Keep collections organized and readable.

---

# 📌 Key Takeaways

- Lists are ordered and mutable.
- Tuples are ordered and immutable.
- Sets are unordered and contain unique values.
- Lists support many useful methods.
- Sets are excellent for removing duplicates.
- Tuples are faster and safer for fixed data.

---

# ❓ Interview Questions

### 1. What is a List?

A List is an ordered and mutable collection of items.

---

### 2. What is a Tuple?

A Tuple is an ordered and immutable collection.

---

### 3. What is a Set?

A Set is an unordered collection of unique elements.

---

### 4. Can Lists contain duplicate values?

Yes.

---

### 5. Can Sets contain duplicate values?

No.

---

### 6. Which collection is immutable?

Tuple.

---

### 7. Which collection is best for removing duplicates?

Set.

---

### 8. Which collection is most commonly used in Python?

List.

---

# 📝 Summary

Today I learned about Python Collections including Lists, Tuples, and Sets. I explored their characteristics, methods, operations, and practical use cases. Lists are ideal for mutable data, Tuples are useful for fixed information, and Sets efficiently store unique values. These collections are fundamental in Python programming and are widely used in automation, cloud computing, cybersecurity, and software development.
