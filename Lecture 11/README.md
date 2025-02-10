## ✨ PIAIC Lecture 11: Sunday Session Recap by Warda Rehman

Welcome to the eleventh session of the **PIAIC Certified Cloud Native AI Program!**. In this session, we continued exploring essential programming concepts in Python. We reviewed loops, functions, error handling, and control structures to build a strong foundation in problem-solving. Understanding these topics helps write clean, efficient, and reusable code. Let’s break down the key lessons in a simple way! 🚀  

---

## **1️⃣ Revisiting For Loops 🔄**  
A **for loop** is used to repeat a block of code over a sequence (like a list, tuple, or string).  

### **Example:**  
```python
numbers = [1, 2, 3, 4]
for num in numbers:
    print(num)
```
### **Output:**  
```
1  
2  
3  
4  
```

---

## **2️⃣ Handling Errors in Loops 🚨**  
Loops can sometimes run into errors, especially when working with unpredictable data. **try-except** helps prevent program crashes by catching errors.  

### **Example:**  
```python
for i in range(5):
    try:
        result = 10 / (i - 2)  # Division by zero when i is 2
    except ZeroDivisionError:
        print(f"Error: Division by zero at i = {i}")
    else:
        print(result)
```

---

## **3️⃣ Try, Except, and Finally for Error Handling ⚠️**  
- **try**: Runs the code that might cause an error.  
- **except**: Catches errors and prevents the program from crashing.  
- **finally**: Runs no matter what happens.  

### **Example:**  
```python
try:
    number = int(input("Enter a number: "))
    result = 10 / number
except ZeroDivisionError:
    print("You can't divide by zero!")
except ValueError:
    print("Please enter a valid number!")
finally:
    print("This will always run, no matter what!")
```

---

## **4️⃣ Creating Custom Errors (User-Defined Exceptions) ✨**  
We can create our own **custom error classes** for better control over error handling.  

### **Example:**  
```python
class NegativeNumberError(Exception):
    """Raised when the number is negative."""
    def __init__(self, value):
        self.message = f"Negative number detected: {value}"
        super().__init__(self.message)

def check_positive_number(num):
    if num < 0:
        raise NegativeNumberError(num)
    return f"{num} is positive."

try:
    print(check_positive_number(-10))
except NegativeNumberError as e:
    print(e)
```

---

## **5️⃣ Control Flow in Python 🛤️**  
Control flow defines how a program makes decisions and runs code in a structured way.  

### **Example:**  
```python
x = 10
if x > 5:
    print("x is greater than 5")
else:
    print("x is 5 or less")
```
### **Output:**  
```
x is greater than 5
```

---

## **6️⃣ Loops: Repeating Code Easily 🔁**  
Loops let us run the same code multiple times instead of writing it over and over.  

---

## **7️⃣ Functions: Reusable Blocks of Code 🧑‍💻**  
Functions help avoid code duplication by storing reusable logic.  

### **Example:**  
```python
def greet():
    print("Hello!")

greet()  # Calls the function
```
### **Output:**  
```
Hello!
```

---

## **8️⃣ Built-in Python Functions 🔧**  
Python has many useful built-in functions like `print()`, `len()`, and `sum()`.  

### **Example:**  
```python
numbers = [1, 2, 3]
print(len(numbers))  # Outputs: 3
```

---

## **9️⃣ Function Parameters and Arguments 🎯**  
A function can take **parameters** (placeholders for values). When calling the function, you provide **arguments** (actual values).  

### **Example:**  
```python
def add_numbers(a, b):
    return a + b

result = add_numbers(3, 5)
print(result)  # Outputs: 8
```

---

## **🔟 Return vs. Non-return Functions ↩️**  
- **Return functions** send back a value.  
- **Non-return functions** only perform an action.  

### **Example:**  
```python
def square(num):
    return num ** 2

result = square(4)
print(result)  # Outputs: 16
```

---

## **1️⃣1️⃣ Types of Function Arguments 📥**  
Python supports different ways to pass arguments:  
✅ **Positional Arguments**: Must be passed in order.  
✅ **Keyword Arguments**: Order doesn’t matter.  

### **Example:**  
```python
def greet(name):
    print(f"Hello, {name}!")

greet("Warda")  # Positional argument
greet(name="Warda")  # Keyword argument
```

### **Using `*args` for Multiple Positional Arguments:**  
```python
def print_numbers(*args):
    for num in args:
        print(num)

print_numbers(1, 2, 3, 4)
```

### **Using `**kwargs` for Multiple Keyword Arguments:**  
```python
def display_info(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

display_info(name="Warda", age=25, country="Pakistan")
```

---

## **1️⃣2️⃣ Lambda Functions (One-Line Functions) 🌀**  
Lambda functions are small, anonymous functions written in a single line.  

### **Example:**  
```python
square = lambda x: x ** 2
print(square(5))  # Outputs: 25
```

---

## **1️⃣3️⃣ Recursive Functions 🔁**  
A **recursive function** calls itself to break a problem into smaller parts.  

### **Example:**  
```python
def factorial(n):
    if n == 1:
        return 1
    else:
        return n * factorial(n - 1)

print(factorial(5))  # Outputs: 120
```

---

## **1️⃣4️⃣ Required vs. Optional Parameters ⚙️**  
- **Required parameters**: Must be provided.  
- **Optional parameters**: Have default values.  

### **Example:**  
```python
def greet(name, message="Hello"):
    print(f"{message}, {name}!")

greet("Warda")  # Uses default message "Hello"
greet("Warda", "Good morning")  # Custom message
```

---

## Wrap-Up  
In this session, we explored fundamental Python concepts like loops, error handling, functions, arguments, recursion, and control flow. These topics are **essential for writing efficient, readable, and bug-free programs**. Keep practicing and experimenting with these concepts to strengthen your Python skills! 🚀  

**Code smart, debug less, and let Python do the rest! 🐍⚡**

---  

