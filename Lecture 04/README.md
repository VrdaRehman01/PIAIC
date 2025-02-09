# ✨ PIAIC Lecture 4: Sunday Session Recap by Warda Rehman

Welcome to the recap of PIAIC Sunday Lecture, held on August 28, 2024. This session focused on some really important building blocks for Python programming, how to set up your computer for development, and how to use containers.

## 🔡 Explanation of Variable and Data Types

Variables are essential components in programming, serving as containers for storing data values. Here's a quick rundown of common data types in Python:

Think of variables as labeled boxes where you can store information.  Each box can hold a specific type of information, called a data type.  Here are the common data types in Python:

**Integers:** These are whole numbers, `like 10, -3, or 0`. No fractions or decimals allowed!

**Floats:** These are numbers that can have decimal points, `like 3.14 or -0.01`. They're used for representing numbers with fractional parts.

**Strings:** These are sequences of characters, basically text. They're enclosed in quotes, `like "hello" or "PIAIC"`

**Datetime:** This special type is for storing dates and times, `like August 25th, 2024, at 10:00 AM`

**Collections:** These are ways to group multiple pieces of data together:
* **Lists:** Lists are ordered collections of items. You can change them after they're created (they're mutable). Think of a shopping list – you can add or remove items. `Example: [1, 2, 3]`
* **Tuples:** Tuples are also ordered collections, but they're immutable, meaning you can't change them once they're created. They're like a list of ingredients in a recipe – you can't change the recipe itself. `Example: (1, 2, 3)`
* **Dictionaries:** Dictionaries store data in key-value pairs. Each key is like a label, and its corresponding value is the information you want to store. Think of a real dictionary – the word is the key, and the definition is the value. `Example: {"name": "Alice", "age": 30}`

---
 
## 📈 Data Formats: How we organize Data
When we work with data, we often need to store it or send it between different programs.  Data formats are like agreed-upon ways of organizing that data.  Here are a few common ones:

*   **XML (eXtensible Markup Language):** A markup language that defines rules for encoding documents in a format readable by humans and machines.
*   **JSON (JavaScript Object Notation):** A lightweight data interchange format that's easy to read and write.
*   **Protocol Buffers (protobuf):** A language-neutral mechanism for serializing structured data.

## 💾 Databases: Where we keep our Data

*   **Structured Databases:**
    *   **Relational Databases (RDBMS):**
     
       Store data in tables. Use SQL to manage data. Examples: MySQL, PostgreSQL.
      
       Use Case: Detecting repeated values, enforcing data integrity, and managing structured data.
*   **NoSQL Databases:**
    *   **Non-Relational Databases:**

       Store unstructured or semi-structured data. Example: MongoDB.
    
       Use Case: Handling large volumes of unstructured data like JSON documents.
*   **Graph Databases:**
    *   **Graph Databases:**
       Store and query data with complex relationships.

       Example: Neo4j. Use Case: Social networks, recommendation engines, and knowledge graphs.

## 🔢 Primitive Data Types

*   **Integers:** Whole numbers, positive or negative, without decimals.
*   **Characters:** Single letters, digits, or symbols.

## 🌱 Development Environment and Containers

*   **Installing the Dev Containers Extension:** Begin by installing the "Dev Containers" extension within VS Code. This extension is key to using pre-built development environments.
*   **Understanding Dev Containers:** A dev container is a complete coding environment, packaged as a Docker container. This ensures everyone working on a project uses the same tools and configurations, preventing compatibility issues.
*   **Building the Docker Image (One Time):** You only need to create the Docker image that holds your dev container setup once. After that, you can reuse it for live coding and testing, saving time and effort.
*   **Enhancing Python Development with Pylance and Mypy:**
     * **Pylance (VS Code Extension):** Install the Pylance extension in VS Code. It provides helpful code suggestions and error checking as you write.
     * **Mypy (Static Type Checker):** Mypy is a tool that checks your Python code for type errors before you run it. This can help catch bugs early. Install it using the command `pip install mypy` in your terminal.
---

## 🐬 Creating a "Hello World" Application Using Docker and DevContainers

**Step-by-Step Guide:**

1.  **Set Up Docker Environment:**
   
   Install Docker and the "Dev Containers" extension in VS Code.
   
2.  **Create a Jupyter Notebook Project:** 

   Create a new directory for your project and initialize it.
   
3.  **Create a Dockerfile:**

```dockerfile
FROM python:3.9-slim                                                                       
WORKDIR /app                                                                              
COPY . /app                                                                                
RUN pip install jupyter                                                                    
CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"] 
```

## Creating a  DevContainer Configuration:
`devcontainer.json` This file tells VS Code how to use your Dockerfile.
```plaintext
{
  "name": "Hello-World Dev Container",
  "dockerFile": "Dockerfile",
  "appPort": [8888],
  "extensions": ["ms-python.python"]
}
```
## Building and Running the Dev Container:

Open the project in VS Code and use the "Reopen in Container" option. Run the Jupyter Notebook:

## Jupyter Notebook: 

Create a file named `hello_world.ipynb` and add the following Python code:

```plaintext
print("Hello, World!")
```
## Access Jupyter: 

VS Code will forward `port 8888`, so you can access your Jupyter Notebook in your web browser.

---

## Wrap-Up
This class gave a practical introduction to setting up a Python development environment with Docker and Jupyter Notebook.  We covered important concepts like data types, data formats, databases, and containerization, all of which are essential for modern software development.

🚀 **Keep learning, keep growing!** 😊
