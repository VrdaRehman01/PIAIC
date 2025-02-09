## ✨ PIAIC Lecture 6: Sunday Session Recap by Warda Rehman
Welcome to the PIAIC Class 06 recap, held at the Bahria Auditorium on **September 8, 2024**. This session explored the powerful features and tools of **Google Colab**, a cloud-based platform for **Python programming**, **data science**, and **machine learning**. Here's a detailed breakdown of everything covered in this exciting session:

---
## 🚀 Why Choose Google Colab?
Google Colab is a free, cloud-based coding environment that simplifies programming, making it accessible for learners and professionals alike. Here are some reasons why Colab is the go-to platform:

* **No Local Errors 🔧:** With Colab running in the cloud, you won’t face issues caused by your local system or hardware.
* **Virtual Computing Environment 💻:** No high-end hardware? No problem! Colab provides free access to virtual machines capable of running complex code.
* **16 GB VRAM 🖥️:** Need a GPU for machine learning? Colab offers GPUs with up to 16 GB VRAM, ideal for AI and deep learning tasks.
* **1 GB/s Network Speed ⚡:** Download datasets and interact with APIs seamlessly with lightning-fast internet speeds.
* **Pre-installed Python 🐍:** Python comes pre-installed with essential libraries, saving you the hassle of manual setup.
* **Colab Pro and Colab Pro+ 💼:**
For those requiring even more power and flexibility, Google offers premium plans:
   * **Colab Pro ($9.99/month):** Faster GPUs, longer runtimes, and priority access to resources.
   * **Colab Pro+ ($49.99/month):** Enhanced performance with even faster GPUs, more memory, and extended runtimes for large-scale tasks.

---

## 🖥️ Google Colab Interface Overview
We explored the user-friendly interface of Google Colab. Here are the main components and their uses:

* **Play Button ▶️:** Executes the code in a cell.
* **+Code Button ➕:** Adds a new code cell to your notebook.
* **Generate with AI 🤖:** Offers AI assistance to generate code snippets, helping you overcome coding challenges efficiently.
* **Creating a New Notebook 📝:**
  
   * Go to `File` > `New Notebook` within Colab.
   * Or, in Google Drive, click `New` > `More` > `Google Colaboratory` to create a notebook.
 
---

## 📑 Notebook Interface Components
* **Menu Bar:** Manage your notebook—save, edit, or run your code seamlessly.
* **Toolbar:** Add/delete cells, run all cells, or stop execution if needed.
* **Notebook Cells:** Write Python code or add formatted text using Markdown.

---

## ⚡ Accelerating Tasks with GPU/TPU
Google Colab allows you to enable GPUs or TPUs for faster computations. This is particularly useful for deep learning and machine learning tasks.

**Steps to Enable GPU/TPU:**
* Navigate to Runtime > Change runtime type.
* Select GPU or TPU under the Hardware Accelerator dropdown.
* Click Save.
To verify GPU access, run this code:
```python
import tensorflow as tf  
print("Num GPUs Available: ", len(tf.config.experimental.list_physical_devices('GPU')))
```
**💻 Writing Your First Python Program**
We wrote a simple program as a warm-up exercise:
```python
print("Hello Warda")
```

We also encountered some common errors and learned how to troubleshoot them:
🐛 Common Errors and How to Fix Them
* **Syntax Error 🛑:** Caused by structural mistakes in code, like missing punctuation or incorrect indentation.
* **Name Error ⚠️:** Happens when trying to use an undefined variable or function.

---

## 📦 Installing External Libraries
Need additional libraries? Install them using pip:
```plaintext
!pip install package_name
```
**Example: To install NumPy, run:**
```plaintext
!pip install numpy
```

---

## 💾 Accessing Files and Google Drive
Google Colab supports file uploads and Google Drive integration for seamless access to datasets.

**Mounting Google Drive:**
```plaintext
from google.colab import drive  
drive.mount('/content/drive')
```
After authentication, your Drive files will be accessible in Colab.

---

## 🔗 Using External Data Sources
Google Colab is excellent for accessing data from external sources, such as GitHub repositories or Google Sheets. Here’s how we can interact with them:
1. **Cloning GitHub Repositories:**
```plaintext
!git clone https://github.com/username/repository.git
```
2. Reading Data from Google Sheets:
```plaintext
import pandas as pd  
url = 'your_google_sheet_url'  
sheet = pd.read_csv(url)
```
---

## 👥 Sharing and Collaboration
* Click the **Share** button in the top-right corner.
* Set permissions (view-only or edit).
* Share the link with collaborators for real-time editing.

---

📧 Sending Emails from Google Colab
We explored how to send emails using the `smtplib` library:
```python
import smtplib  

# Email details  
sender = 'your_email@gmail.com'  
receiver = 'receiver_email@gmail.com'  
password = 'your_password'  
message = """Subject: Test Email from Google Colab  

This is a test email sent from Google Colab."""  

# Setup server connection  
server = smtplib.SMTP('smtp.gmail.com', 587)  
server.starttls()  

# Login and send the email  
server.login(sender, password)  
server.sendmail(sender, receiver, message)  
server.quit()  

print('Email sent successfully!')
```

---

## Wrap-Up
This session provided a hands-on introduction to Google Colab, covering its features, interface, and tools to make coding efficient and accessible. Explore, experiment, and harness the full potential of Colab for your Python programming, machine learning, and data science projects.

**Keep learning, and keep exploring!** 🌟







