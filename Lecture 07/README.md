## ✨ PIAIC Lecture 7: Sunday Session Recap by Warda Rehman


![Python](https://img.shields.io/badge/Python-3.x-blue)  
![AI](https://img.shields.io/badge/AI-Important-red)  
![Reinforcement Learning](https://img.shields.io/badge/Reinforcement%20Learning-Active-orange)

Welcome to the recap of PIAIC's Python AI Sunday Lecture, held on September 15, 2024. This session focused on fundamental Python concepts essential for AI development, including ChatGPT and reinforcement learning, string manipulation, data display methods, type conversion, and various Python operators. Whether you are just starting with Python or looking to strengthen your programming skills, this guide simplifies the key takeaways from the session and helps you apply them to practical coding scenarios. 🚀

This class focused on fundamental Python concepts related to AI and programming.

---
## 🧠 Introduction to ChatGPT & AI Learning (Strawberry Project)

### Understanding AI Levels
Artificial Intelligence has multiple levels, and in this session, we mainly discussed chatbots and intelligent agents.

### 🤖 Reinforcement Learning (RL)
- Reinforcement Learning is a method where an AI system **learns by trial and error**.
- It interacts with an environment, performs actions, and **receives rewards** when it makes correct decisions.
- **Example:** A robot 🤖 gets a command, performs a task, and earns a reward 🏆 for completing it successfully.

---

## 🔤 Working with Strings in Python

### Shallow Copy vs. Deep Copy

- **Shallow Copy** 🔗: Copies only the reference (memory location), not the actual object.
- **Deep Copy** 📦: Creates a completely separate copy of an object.

### 📝 Common String Escape Characters
Escape characters are special characters used in strings:

- `\\` → Inserts a backslash (`\`).
- `\n` → Moves text to a new line.
- `\t` → Adds a tab space.

---

## 🖥️ Displaying Data in Python

There are two main ways to display data:

1. **`display(data)`** → Shows raw data (mainly used in Jupyter Notebooks).
2. **`print(data)`** → Formats and presents data in a more readable way.

Example:
```python
data = "Hello, Python!"
display(data)  # Shows raw representation
print(data)  # Prints the string normally
```

---

## 🔄 Converting Data Types (Type Casting)

Python allows converting values from one type to another.

### Example:
```python
num = 10
string_num = str(num)  # Converts 10 (integer) into "10" (string)
```

### Using Placeholders in Strings
Placeholders are used to insert values inside strings:

- `%s` → For inserting strings.
- `%d` → For inserting integers.

Example:
```python
name = "Alice"
age = 25
print("My name is %s and I am %d years old." % (name, age))
```

---

## 🔢 Python Operators

### 1️⃣ Arithmetic Operators
These operators perform basic math operations.

| Operator | Description | Example |
|----------|------------|---------|
| `+` | Addition | `a + b` |
| `-` | Subtraction | `a - b` |
| `*` | Multiplication | `a * b` |
| `/` | Division (returns float) | `a / b` |
| `//` | Floor Division (removes decimal) | `a // b` |
| `%` | Modulus (remainder) | `a % b` |
| `**` | Exponent (power) | `a ** b` |

Example:
```python
a = 10
b = 3
print(a + b)  # 13
print(a ** b)  # 1000 (10^3)
```

---

### 2️⃣ Comparison Operators
These operators compare values and return `True` or `False`.

| Operator | Meaning | Example |
|----------|---------|---------|
| `==` | Equal to | `a == b` |
| `!=` | Not equal to | `a != b` |
| `>` | Greater than | `a > b` |
| `<` | Less than | `a < b` |
| `>=` | Greater than or equal to | `a >= b` |
| `<=` | Less than or equal to | `a <= b` |

Example:
```python
x = 5
y = 10
print(x > y)  # False
print(x != y)  # True
```

---

### 3️⃣ Assignment Operators
These operators assign values to variables.

| Operator | Meaning | Example |
|----------|---------|---------|
| `=` | Assign value | `a = 10` |
| `+=` | Add and assign | `a += 5` (same as `a = a + 5`) |
| `-=` | Subtract and assign | `a -= 5` |
| `*=` | Multiply and assign | `a *= 5` |
| `/=` | Divide and assign | `a /= 5` |

Example:
```python
num = 10
num += 5  # num is now 15
print(num)
```

---

### 4️⃣ Logical Operators
These operators are used to combine multiple conditions.

| Operator | Meaning | Example |
|----------|---------|---------|
| `and` | True if both conditions are true | `(a > 5 and b < 10)` |
| `or` | True if at least one condition is true | `(a > 5 or b < 10)` |
| `not` | Reverses a condition | `not (a > 5)` |

Example:
```python
x = True
y = False
print(x and y)  # False
print(x or y)   # True
print(not x)    # False
```

---

### 5️⃣ Membership Operators
These check if a value exists inside a list, tuple, or string.

| Operator | Meaning | Example |
|----------|---------|---------|
| `in` | Checks if a value is present | `"a" in "apple"` |
| `not in` | Checks if a value is absent | `"z" not in "apple"` |

Example:
```python
fruits = ["apple", "banana", "cherry"]
print("apple" in fruits)  # True
print("mango" not in fruits)  # True
```

---

### 6️⃣ Identity Operators
These check if two variables refer to the same object in memory.

| Operator | Meaning | Example |
|----------|---------|---------|
| `is` | True if both variables refer to the same object | `x is y` |
| `is not` | True if variables are different objects | `x is not y` |

Example:
```python
a = [1, 2, 3]
b = a
c = [1, 2, 3]

print(a is b)  # True (same object)
print(a is c)  # False (different objects with the same content)
```

---

## Wrap-Up
We explored Reinforcement Learning (RL) and how AI learns through rewards, delved into string operations including copy types and escape characters, and covered essential concepts like data display, type casting, and Python operators.

Code, explore, and innovate! 🚀
