## ✨ PIAIC Lecture 12: Sunday Session Recap by Warda Rehman
Welcome to the Twelfth session of the PIAIC Certified Cloud Native AI Program! Object-Oriented Programming (OOP) is a powerful way to structure code, making it more reusable and scalable. Instead of writing code around functions, OOP focuses on **objects**, which represent real-world entities like a car, a person, or even a bank account. Each object has **attributes** (data) and **methods** (functions) that define its behavior.  

In this session, we explored the core concepts of OOP in Python, including **encapsulation, inheritance, polymorphism, and abstraction**. We also learned how to define classes, create objects, use special methods, and work with constructors and destructors. Let’s break it down step by step! 🚀  

---

## **🧩 Understanding Object-Oriented Programming (OOP)**
OOP is a programming style that focuses on objects rather than just functions and procedures. In Python, everything is an object!  

### **🔹 Key Terms in OOP**
- **Class** → A blueprint for creating objects  
- **Object** → An instance of a class with specific data and behavior  
- **Attributes** → Variables that hold an object’s data  
- **Methods** → Functions that define what an object can do  

---

## **🔑 Four Pillars of OOP**
### **1️⃣ Encapsulation 🔒 (Data Protection)**
Encapsulation means **hiding** data within a class and only allowing controlled access to it. This keeps our code secure and well-organized.  

#### **Example: Private and Public Attributes**
```python
class Car:
    def __init__(self, brand, model):
        self.brand = brand      # Public attribute
        self.__model = model    # Private attribute

    def get_model(self):
        return self.__model  # Accessing private attribute using a method

car1 = Car("Toyota", "Corolla")
print(car1.brand)        #  Allowed
print(car1.get_model())  #  Allowed via method
print(car1.__model)      #  Not Allowed (AttributeError)
```
👉 **Why use encapsulation?** To protect sensitive data and prevent direct modification.

---

### **2️⃣ Inheritance 🧬 (Code Reusability)**
Inheritance allows a new class (**child class**) to inherit methods and attributes from an existing class (**parent class**).  

#### **Example: Simple Inheritance**
```python
class Vehicle:
    def start_engine(self):
        print("Engine started!")

class Car(Vehicle):  # Car class inherits from Vehicle
    pass

my_car = Car()
my_car.start_engine()  # Inherits method from Vehicle
```
👉 **Why use inheritance?** To avoid rewriting code and create a logical hierarchy between classes.

---

### **3️⃣ Polymorphism 🎭 (Same Function, Different Behavior)**
Polymorphism allows different objects to use the **same method name** but behave differently.  

#### **Example: Different Classes with the Same Method**
```python
class Bird:
    def sound(self):
        return "Chirp"

class Dog:
    def sound(self):
        return "Bark"

def make_sound(animal):
    print(animal.sound())

make_sound(Bird())  # Output: Chirp
make_sound(Dog())   # Output: Bark
```
👉 **Why use polymorphism?** It makes code more flexible and scalable.

---

### **4️⃣ Abstraction 🎩 (Hiding Complexity)**
Abstraction means **hiding the details** and showing only the important parts of an object. This makes the code easier to use and understand.  

#### **Example: Abstract Class**
```python
from abc import ABC, abstractmethod

class Animal(ABC):  # Abstract Class
    @abstractmethod
    def sound(self):
        pass  # Must be implemented by subclasses

class Cat(Animal):
    def sound(self):
        return "Meow"

print(Cat().sound())  # Output: Meow
```
👉 **Why use abstraction?** To keep the code simple and focus only on what’s necessary.

---

## **🛠️ Creating Classes and Objects**
Classes help us **define a template** for objects. Objects are then created from these templates.  

#### **Example: Defining a Class and Creating an Object**
```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def greet(self):
        return f"Hello, my name is {self.name}."

person1 = Person("Alice", 30)
print(person1.greet())  # Output: Hello, my name is Alice.
```
👉 **Why use classes and objects?** They help organize and structure code in a better way.

---

## **🛠️ Constructors and Destructors**
- **Constructor (`__init__`)** → Runs automatically when an object is created  
- **Destructor (`__del__`)** → Runs when an object is deleted  

#### **Example: Constructor and Destructor in Action**
```python
class MyClass:
    def __init__(self):
        print("Object created!")

    def __del__(self):
        print("Object deleted!")

obj = MyClass()  # Object is created
del obj          # Object is deleted
```
👉 **Why use them?** To handle setup and cleanup tasks automatically.

---

## **🎩 Magic (Dunder) Methods**
Magic methods (also called **dunder methods**) allow objects to interact with built-in Python operations.

#### **Example: `__str__()` for Custom String Representation**
```python
class Book:
    def __init__(self, title, pages):
        self.title = title
        self.pages = pages

    def __str__(self):
        return f"{self.title}, {self.pages} pages"

book = Book("Python Guide", 300)
print(book)  # Output: Python Guide, 300 pages
```
👉 **Why use magic methods?** They make objects work like built-in data types.

---

## Wrap-Up
In this session, we explored the fundamentals of Object-Oriented Programming in Python, covering **classes, objects, encapsulation, inheritance, polymorphism, abstraction, constructors, destructors, and magic methods**. By mastering these concepts, you can write more efficient and modular code that scales well.  

 **🚀Write less, do more, let objects handle the work!**
