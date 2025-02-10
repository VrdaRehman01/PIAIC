# 📌 Lecture 08: AI and Variables – Explained by Warda Rehman

## 🎯 Purpose of This Lesson  

This lesson teaches how to **interact with AI using variables** in Python. Instead of manually entering information every time, you can store details like names, ages, and preferences in variables. This makes coding more **dynamic and interactive**, helping you customize AI responses effortlessly.  

For example, rather than typing out full descriptions, you can use variables to provide AI with **structured input**. This skill is essential for building smart, **personalized applications** in programming and AI.  

---

## 📥 Step 1: Download the Helper Functions 🧙‍♂️✨  

To get started, we need a **special helper file** that allows us to communicate with AI, like a chatbot. Run the following command to download it:  

```python
!curl -o helper_functions.py https://raw.githubusercontent.com/panaversity/learn-cloud-native-modern-ai-python/main/07_natural_language_programming/02_ai_python_for_beginners/course1_basics/Lesson_9/helper_functions.py
```  

🔹 **Click "Run"** in your Jupyter Notebook or Google Colab to download the necessary tools!  

---

## 🪄 Step 2: Import the AI Function  

Now that we have the helper functions, we need to **import** them to use AI in our code.  

```python
from helper_functions import print_llm_response
```  

This allows us to **send messages to AI** and receive responses instantly. 🚀  

---

## 💬 Step 3: Ask the AI a Question 🤔  

Now, let’s try asking the AI a **simple question**. Think of it like chatting with a smart assistant!  

```python
print_llm_response("What is the capital of France?")
```  

🗼 **AI’s Response:**  
```
The capital of France is Paris.
```  

Just like that, AI gives us instant answers! 🎉  

---

## 📦 Step 4: Understanding Variables in Python  

A **variable** is like a **container** that stores information such as names, numbers, or words. Instead of typing the same thing repeatedly, you store the value in a variable and use it whenever needed.  

Example:  

```python
name = "Otto Matic"
dog_age = 21 / 7  # Otto is 3 years old in dog years!
```  

Now, instead of writing `"Otto Matic"` multiple times, we can simply use `name`.  

---

## 🐶 Step 5: Use Variables to Ask AI Questions  

Let's make AI describe **Otto’s life as a dog** using the variables we created!  

```python
print_llm_response(f"If {name} were a dog, he would be {dog_age} years old. Describe his energy level, interests, and behavior.")
```  

🐾 **AI’s Response:**  
```
Otto would be in his early adulthood, full of energy and curiosity!
```  

By using **variables**, we can quickly modify the input and **get different answers** without rewriting the entire prompt.  

---

## ❌ Step 6: Fixing Incorrect Variable Names  

Sometimes, we make **mistakes** while naming variables, like using spaces or special characters. Python does **not** allow spaces, special symbols (except `_`), or starting a variable name with a number.  

🔴 **Incorrect Code:**  
```python
driver's vehicle = "dinosaur car"  # ❌ Apostrophes aren't allowed!
```  

✅ **Fixed Code:**  
```python
drivers_vehicle = "dinosaur car"  # ✔ No special characters, and uses underscore!
```  

Always use **clear and readable names** to avoid errors!  

---

## 🌈 Step 7: Create Fun Stories with AI  

Now, let's **write a fun story** using variables! 🚀  

```python
driver = "unicorn"
vehicle = "dinosaur car"
favorite_planet = "Pluto"

print_llm_response(f"Write a 300-word story about a {driver} racing a {vehicle} on {favorite_planet}.")
```  

🌍 **AI’s Response:**  
```
Once upon a time, a unicorn zoomed across Pluto in a dinosaur car, leaving behind a trail of stardust...
```  

This shows how **variables** can help create dynamic AI-generated content!  

---

## 🛠️ Step 8: Practice Fixing Broken Code  

Let’s fix a common coding mistake where a variable **starts with a number**.  

🔴 **Incorrect Code:**  
```python
1favorite-book = "1001 Ways to Wear a Hat"  # ❌ Variables can't start with numbers!
```  

✅ **Fixed Code:**  
```python
favorite_book = "1001 Ways to Wear a Hat"  # ✔ Renamed correctly!
```  

By following proper **variable naming rules**, we avoid errors in Python.  

---

## 🎵 Step 9: Get AI Recommendations Based on Your Favorites  

Now, let’s create some **personalized recommendations** by telling AI what we like!  

```python
favorite_game = "Minecraft"
favorite_movie = "Harry Potter"
favorite_food = "Pizza"

print_llm_response(f"Based on my love for {favorite_game}, {favorite_movie}, and {favorite_food}, recommend me a new song to listen to.")
```  

🎧 **AI’s Response:**  
```
You might enjoy "Viva La Vida" by Coldplay, based on your interests!
```  

Using **variables**, we can easily change our preferences and get different recommendations every time!  

---
