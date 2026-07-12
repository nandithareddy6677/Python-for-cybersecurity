# Day 4: Python Functions

> Understanding Python Functions, parameters, arguments, return values, scope, lambda functions, and why functions are essential for writing reusable and organized code.

---

# 🎯 Learning Objectives

- Understand what Functions are.
- Learn why Functions are used.
- Create your own Functions.
- Understand Parameters and Arguments.
- Learn Return Values.
- Understand Variable Scope.
- Learn Lambda Functions.
- Prepare for Python interviews.

---

# 📖 Introduction

As programs become larger, writing the same code repeatedly becomes inefficient.

Functions help organize code into reusable blocks that perform specific tasks.

Instead of rewriting code, we simply call the function whenever needed.

Functions make programs:

- Cleaner
- Easier to Read
- Easier to Debug
- Easier to Reuse

---

# 🔹 What is a Function?

A Function is a reusable block of code designed to perform a particular task.

Example:

```python
def greet():
    print("Hello, World!")

greet()
```

Output:

```
Hello, World!
```

---

# Why Use Functions?

Functions help to:

- Avoid code duplication.
- Improve readability.
- Simplify debugging.
- Make programs modular.
- Reuse code.

---

# Creating a Function

Syntax:

```python
def function_name():
    print("Function Executed")
```

Example:

```python
def welcome():
    print("Welcome to Python!")

welcome()
```

Output:

```
Welcome to Python!
```

---

# Function Parameters

Parameters allow functions to accept data.

Example:

```python
def greet(name):
    print("Hello", name)

greet("Nanditha")
```

Output:

```
Hello Nanditha
```

---

# Multiple Parameters

Example:

```python
def add(a, b):
    print(a + b)

add(10, 20)
```

Output:

```
30
```

---

# Arguments

Arguments are the actual values passed to a function.

Example:

```python
def student(name, age):
    print(name, age)

student("Nanditha", 21)
```

---

# Return Statement

The `return` keyword sends a value back to the caller.

Example:

```python
def square(num):
    return num * num

result = square(5)

print(result)
```

Output:

```
25
```

---

# Difference Between print() and return

Using `print()`:

```python
def add(a, b):
    print(a + b)
```

Using `return`:

```python
def add(a, b):
    return a + b
```

`return` is preferred because the returned value can be reused.

---

# Default Parameters

Functions can have default values.

Example:

```python
def greet(name="Guest"):
    print("Hello", name)

greet()

greet("Nanditha")
```

Output:

```
Hello Guest

Hello Nanditha
```

---

# Keyword Arguments

Example:

```python
def student(name, age):
    print(name, age)

student(age=21, name="Nanditha")
```

---

# Variable Scope

Variables created inside a function are called **Local Variables**.

Example:

```python
def demo():
    x = 10
    print(x)

demo()
```

`x` cannot be accessed outside the function.

Variables created outside functions are called **Global Variables**.

Example:

```python
name = "Python"

def show():
    print(name)

show()
```

---

# Lambda Functions

A Lambda Function is a small anonymous function.

Syntax:

```python
lambda arguments: expression
```

Example:

```python
square = lambda x: x*x

print(square(6))
```

Output:

```
36
```

---

# Recursive Functions

A function can call itself.

Example:

```python
def countdown(n):

    if n == 0:
        return

    print(n)

    countdown(n-1)

countdown(5)
```

Output:

```
5

4

3

2

1
```

---

# Built-in Functions

Python provides many built-in functions.

Examples:

```python
print()

len()

max()

min()

sum()

type()

input()
```

---

# 🌍 Real-Life Example

Suppose you build a Login System.

Instead of writing login code multiple times, you create a function.

```python
def login(username):

    print("Welcome", username)

login("Nanditha")
```

Whenever a user logs in, the same function is reused.

---

# 💡 Best Practices

- Keep functions small.
- Give meaningful names.
- Use parameters whenever possible.
- Prefer `return` over `print`.
- Avoid unnecessary global variables.
- Write reusable functions.

---

# 📌 Key Takeaways

- Functions organize code into reusable blocks.
- Parameters receive input.
- Arguments pass values.
- `return` sends data back.
- Local variables exist only inside functions.
- Global variables are accessible throughout the program.
- Lambda functions provide concise syntax.

---

# ❓ Interview Questions

### 1. What is a Function?

A Function is a reusable block of code that performs a specific task.

---

### 2. What is the difference between Parameters and Arguments?

Parameters are variables defined in the function, while Arguments are the actual values passed during the function call.

---

### 3. What does the `return` keyword do?

It sends a value back to the caller.

---

### 4. What is a Local Variable?

A variable declared inside a function.

---

### 5. What is a Global Variable?

A variable declared outside all functions and accessible throughout the program.

---

### 6. What is a Lambda Function?

A Lambda Function is a small anonymous function written using the `lambda` keyword.

---

### 7. What is Recursion?

Recursion is when a function calls itself to solve a problem.

---

### 8. Why are Functions important?

Functions improve code reusability, readability, maintainability, and reduce duplication.

---

# 📝 Summary

Today I learned about Python Functions and how they help organize programs into reusable blocks of code. I explored function creation, parameters, arguments, return values, variable scope, lambda functions, recursion, and built-in functions. Functions are one of the most important concepts in Python and are widely used in automation, cybersecurity, cloud computing, and software development.
