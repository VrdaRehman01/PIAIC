## ✨ PIAIC Lecture 10: Sunday Session Recap by Warda Rehman
Welcome to the tenth session of the **PIAIC Certified Cloud Native AI Program!** In this session, we explored key programming concepts that are essential for writing efficient and structured code. We covered **programming paradigms**, how AI models like **ChatGPT** interact, and fundamental control structures such as **loops, conditionals, and functions**. The lesson also included practical applications, like creating a **login/signup system** in Python and handling **errors gracefully**. By understanding these concepts, you’ll be able to write better, more organized programs and solve problems efficiently. Let’s dive into the details! 🚀  

---

## 🧠 Understanding Programming Paradigms  

### **1. What is a Programming Paradigm?**  
A **programming paradigm** is a way of thinking about and structuring code. It defines the style and method used to write and organize programs.  

### **2. Linear Programming**  
Linear programming means writing code in a step-by-step manner, where each instruction runs one after another unless modified by loops or conditions.  

### **3. Structured Programming**  
Structured programming breaks a large program into **smaller, reusable blocks (functions)**. This makes the code easy to read, debug, and maintain.  

---

## 🤖 ChatGPT Model Interaction  
We explored how to **interact with AI models** like ChatGPT. AI can understand and generate text, assist with coding, and help solve problems. This session showed how AI can be used as a powerful tool for learning and automation.  

---

## 🔄 Control Structures in Python  

Control structures **control the flow of execution** in a program.  

### **1. If-Else Conditions**  
Conditions allow the program to make decisions based on given data.  

```python
if True:
    print("Pakistan")
    print("Zindabad ")
```  

This prints **"Pakistan Zindabad"** because `True` is always true.  

### **2. Shortened If-Else (Ternary Operator)**  
```python
result = "Pass" if score >= 50 else "Fail"
```  
This is a **shortcut for if-else statements** in Python.  

---

## 🏆 Grading System in Python  

We learned how to **automate grade calculations** using Python.  

### **Example 1: Simple Grading System**  
```python
percentage = 75

if percentage >= 80:
    print("A+")
elif percentage >= 70:
    print("A")
elif percentage >= 60:
    print("B")
elif percentage >= 50:
    print("C")
elif percentage >= 40:
    print("D")
elif percentage >= 33:
    print("Happy")
else:
    print("Fail")
```  

### **Example 2: Improved Grading System with Ranges**  
```python
percentage = 90

if 0 <= percentage < 40:
    print("Fail")
elif 40 <= percentage < 50:
    print("D")
elif 50 <= percentage < 60:
    print("C")
elif 60 <= percentage < 70:
    print("B")
elif 70 <= percentage < 80:
    print("A")
elif 80 <= percentage <= 100:
    print("A+")
else:
    print("Invalid")
```  
This version ensures that the **input is within a valid range** before assigning a grade.  

---

## 🔄 Loops in Python  

Loops allow us to **repeat actions** efficiently.  

### **1. While Loop**  
```python
counter = 0
while counter <= 10:
    print(counter)
    counter += 1
```
This prints numbers **from 0 to 10**.  

### **2. For Loop**  
```python
for letter in "Warda":
    print(letter)
```
This prints each letter of the string **"Warda"** on a new line.  

---

## 🔗 Using `zip()` and `unzip()` in Python  

- `zip()` **combines multiple lists** into tuples.  
- `unzip()` **separates zipped lists** back into their original form.  

---

## ⚠️ Error Handling in Python  

Error handling prevents **program crashes** when unexpected inputs occur.  

### **Using Try-Except**  
```python
try:
    num = int(input("Enter a number: "))
    print(10 / num)
except ZeroDivisionError:
    print("You can't divide by zero!")
except ValueError:
    print("Please enter a valid number.")
```  
This ensures that the program **doesn't crash** due to invalid input.  

---

## 🔑 Login & Signup System in Python  

We built a **basic authentication system** in Python.  

```python
users = {}

def signup():
    username = input("Enter a new username: ")
    if username in users:
        print("Username already exists. Try again.")
    else:
        password = input("Enter a new password: ")
        users[username] = password
        print("Signup successful!")

def login():
    username = input("Enter your username: ")
    if username in users:
        password = input("Enter your password: ")
        if users[username] == password:
            print("Login successful!")
        else:
            print("Incorrect password.")
    else:
        print("Username not found.")

def main():
    while True:
        choice = input("Do you want to login or signup? (login/signup/exit): ").lower()
        if choice == 'login':
            login()
        elif choice == 'signup':
            signup()
        elif choice == 'exit':
            print("Goodbye!")
            break
        else:
            print("Invalid choice. Please choose login, signup, or exit.")

main()
```  

🔹 Users can **sign up and create an account**.  
🔹 **Existing users can log in** with their username and password.  
🔹 **Error handling** ensures that incorrect passwords or usernames are managed properly.  

---

##  Wrap-Up  

In this class, we explored key programming concepts, including **control structures, loops, grading systems, and authentication systems** in Python. We also discussed **AI models like ChatGPT** and how they interact with users. By learning these concepts, you can now write **more efficient, structured, and interactive programs**. Keep practicing, and soon, you'll be able to build even more advanced projects!  

**🚀Code, Create, Conquer!** ✨
