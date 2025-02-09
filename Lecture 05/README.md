# ✨ PIAIC Class 05: Sunday Session Recap by Warda Rehman
Welcome to the recap of PIAIC Class 05, held on September 1, 2024. This session focused on essential programming tools and concepts, including GitHub setup, VS Code shortcuts, and the differences between dynamic and static data types.

Key topics included string manipulation (case conversions, concatenation), ID and directory functions, and practical steps for managing repositories. Perfect for beginners or those refining their skills, this session provided a strong foundation for efficient programming and development workflows.

---

# 🚀 GitHub Setup

GitHub is a powerful platform for managing and sharing code repositories. Here's a step-by-step guide to getting started:

## Step 1: Sign Up on GitHub
Visit [GitHub](https://github.com/) and create an account if you don’t already have one.

## Step 2: Install GitHub Desktop
Download and install [GitHub Desktop](https://desktop.github.com/), a user-friendly application to manage your repositories.

## Step 3: Log in to GitHu
Open GitHub Desktop and log in using your GitHub credentials.

## Step 4: Create a New Repository Locally
1. Open GitHub Desktop and create a new repository on your local system.
2. Choose a **unique name** for your repository to avoid conflicts.
3. Navigate to your repository folder using the terminal:
   ```bash
   cd <repository-folder>
   ```
4. Open the repository in VS Code:
```plaintext
code .
```
5. Create a new file in the repository named `main.py` to write your code.

## Step 5: Save Changes (Commit)
Use GitHub Desktop to commit changes. Committing saves your updates locally to the repository.

## Step 6: Push Changes to GitHub
Push your local changes to GitHub to create a remote repository and secure your work:
```plaintext
git push origin main
```
## Step 7: Restore Files with Checkout
Use the `git checkout` command to restore files or switch to a previous state of your repository. For example:
```plaintext
git checkout <file-name>
```
You can also restore specific files using the commit hash from GitHub.

---

## 🆚 VS Code Shortcuts
* **CTRL + Enter:** Run the current code.
* **SHIFT + Enter:** Run code in a new line.
* **ALT + Enter:** Run code in the terminal.

---

## 👾 Data Types
1. **Dynamic Data Types:** Variables can store any type of data without explicitly specifying the type.
```plaintext
x = 10        # x is an integer
x = "Hello"   # x is now a string
x = 3.14      # x is now a float
```
2. **Static Data Types:** Variables are explicitly assigned a specific data type that cannot change.
```plaintext
age: int = 20      # age can only be an integer
name: str = "Ali"  # name can only be a string
```
---

## Upper Case Example
```plaintext
text = "hello world"
print(text.upper())  # Output: "HELLO WORLD"
```
---

## Lower Case Example
```plaintext
text = "HELLO WORLD"
print(text.lower())  # Output: "hello world"
```
---

## Title Case Example
```plaintext
text = "hello world"
print(text.title())  # Output: "Hello World"
```
---

## Variables and Data Types
```plaintext
name: str = "Warda"
print(type(name))  # Output: <class 'str'>
```
---

## ID and Directory Functions
```plaintext
print(id(name))
print(dir(name))
```

## String Concatenation
```plaintext
A = "Warda"
B = "Rehman"
C = A + B
print(C)  # Output: "WardaRehman"
```
---

##  Wrap-Up  
This session covered GitHub setup, VS Code shortcuts, data types, string manipulation, and key programming tools, providing a solid foundation for efficient coding and development workflows.

**Keep learning, keep coding, and keep building!** 🚀
