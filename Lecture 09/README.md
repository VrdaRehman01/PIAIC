## # ✨ PIAIC Lecture 2: Sunday Session Recap by Warda Rehman
Welcome to the second session of the **PIAIC Certified Cloud Native AI Program!** held on held on September 29, 2024. 
In this session, we explored essential concepts in Python and cloud-based development, helping us build a strong foundation for AI programming. We started by setting up **Google Colab**, an online coding environment that makes Python coding easier and more accessible. Then, we learned how to **download external Python files**, import helper functions, and even generate an **API key** for Google’s **Gemini AI**.  

Moving further, we dived into **functions**, understanding their importance, how to define them, and the difference between `print()` and `return()`. We also explored **dynamic vs. static functions**, learned how to store functions in variables, and discussed how Python uses **modules** to break large programs into smaller, reusable parts.  

Additionally, we covered the differences between **compiled and interpreted languages**, helping us appreciate Python’s flexibility. We also introduced **dependencies and dev dependencies**, comparing them to real-life scenarios like cooking! Lastly, we discussed **Large Language Models (LLMs)**, their capabilities, and their limitations when it comes to real-time data access.  

---

## 💻 Setting Up Google Colab  

Google Colab is an **online coding platform** where we can write and run Python code. It’s widely used because:  
✔️ It provides free **cloud-based GPUs and TPUs**, making it perfect for **machine learning** and **AI**.  
✔️ No need to install Python on your computer—it runs in the browser!  
✔️ It allows easy **collaboration** and **file sharing**.  

---

## 🛠️ Running the First Command  

The first command we executed was:  

```python
!curl -o helper_functions.py https://raw.githubusercontent.com/panaversity/learn-cloud-native-modern-ai-python/main/07_natural_language_programming/02_ai_python_for_beginners/course1_basics/Lesson_9/helper_functions.py
```  

### 🔍 What does this command do?  
- `!curl`: The **exclamation mark (!)** tells Colab that this is a **shell command**, not Python.  
- `curl`: A tool used to **download files from the internet**.  
- `-o helper_functions.py`: This means **"save the downloaded file as helper_functions.py"**.  
- `URL`: This is the web address where the file is stored on **GitHub**.  

🔹 **In summary**: This command **downloads a Python file** from the internet and saves it in our coding environment. 📥  

---

## 🧩 Importing Functions from the File  

After downloading the file, we used the following command:  

```python
from helper_functions import *
```  

### 🔍 What does this command do?  
- `from helper_functions`: Refers to the downloaded file.  
- `import *`: This means **"import everything from the file"**, so we can use all its functions in our code.  

Now, we can use **pre-built functions** without rewriting them!  

---

## 🔑 Creating a Gemini API Key  

To use Google’s **Gemini AI**, we needed an **API key**. Here’s how we got it:  

1️⃣ **Go to Google AI Studio** 🌍  
2️⃣ **Sign in with your Google account** 🔐  
3️⃣ **Create a new project** 🚧  
4️⃣ **Enable the Gemini API** 📊  
5️⃣ **Go to "Credentials" and click "Create API Key"** 🔑  
6️⃣ **Copy and save the API key** 📝  

This API key allows us to **connect Python with Google's AI services**.  

---

## 🏗️ Understanding Python Functions  

Functions are **reusable blocks of code** that perform specific tasks. Instead of writing the same code repeatedly, we can **call a function** whenever needed.  

### ✅ Creating a Simple Function  

```python
def greet():
    print("Hello, World!")
```  

- `def greet()`: Defines a function called `greet`.  
- `print("Hello, World!")`: The function prints a message when called.  
- `greet()`: Calls the function.  

📌 **Output:**  

```
Hello, World! 🌎
```  

---

## 🥚 Dependencies vs. Dev Dependencies  

🔹 **Dependencies** are like **ingredients** in cooking. If you’re making an omelet, you need **eggs, salt, and oil**. Similarly, a Python project needs libraries like **NumPy** or **Pandas** to run properly.  

🔹 **Dev Dependencies** are like **cooking tools**—you need a frying pan 🥘 to cook an omelet, but you don’t serve it. In Python, **dev dependencies** (like debugging tools) are needed **only during development**.  

---

## 🔁 Storing Functions in Variables  

Python allows us to **store functions inside variables**:  

```python
greet_function = greet
greet_function()  # This will print "Hello, World!"
```  

Here, `greet_function` **stores** the function `greet`, so calling it works the same way!  

---

## 🔄 Return vs. Print in Functions  

✔️ `print()`: Displays something on the screen but **doesn’t return a value**.  
✔️ `return`: Gives a value back that can be **used later** in the program.  

Example:  

```python
def add(a, b):
    return a + b

sum = add(5, 3)
print(sum)  # Output: 8 🎯
```  

---

## ⚖️ Compiling vs. Interpreting  

✔️ **Compiled languages (C, C++)** convert the entire code into machine language **before running it**.  
✔️ **Interpreted languages (Python, JavaScript)** run **line by line**, making debugging easier.  

---

## 🧩 Modular Programming in Python  

Python allows us to break large programs into **modules**:  

```python
import math
print(math.sqrt(16))  # Output: 4.0
```  

Here, `math` is a **module** that provides mathematical functions. This **modular approach** makes code reusable and well-organized!  

---

## ⚠️ Limitations of Large Language Models (LLMs)  

LLMs like **ChatGPT** and **Gemini AI** are **not connected to live data**. They work by predicting text based on their training data. So, if you ask about the **latest news**, they might not give real-time information.  

---

## 🔍 Research Tasks  

📌 **What is an AI agent?**  
📌 **What is LangChain and how is it used?**  
📌 **What is LangGraph?**  

---

## 🎯 Wrap-Up  

This session helped us strengthen our **Python skills** by understanding **functions, modules, API keys, and cloud-based environments**. We explored how to make our code more **efficient and reusable** while learning about **AI-powered tools like Gemini AI**. With this knowledge, we are now better equipped to build **powerful, scalable, and intelligent applications** using Python.  

**Master the basics, and the future of AI is in your hands! 🚀**  
