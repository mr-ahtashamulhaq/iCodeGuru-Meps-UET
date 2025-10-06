# Class 26 – Different Libraries of Python  
**Topic:** Overview of Popular Python Libraries and Their Real-World Applications  

---

## 🧠 Introduction  
Python’s true power lies in its vast collection of **libraries** and **frameworks**, which simplify complex tasks and allow developers to focus on logic rather than implementation details.  
A **library** is a collection of pre-written code that provides ready-to-use functions for specific tasks like data analysis, machine learning, visualization, web development, and automation.

---

## 📊 1. Data Analysis & Visualization Libraries  

### 🧮 NumPy (Numerical Python)  
- Core library for **numerical computation** and **array manipulation**.  
- Provides tools for mathematical, logical, and statistical operations.  
- Supports **multi-dimensional arrays (ndarrays)** and operations on them.  

**Example:**  
```python
import numpy as np
arr = np.array([1, 2, 3, 4])
print("Mean:", arr.mean())
print("Sum:", arr.sum())
Use Cases:

Mathematical and statistical analysis

Matrix operations

Data preprocessing for ML models

📈 Pandas
Used for data analysis and manipulation.

Introduces two primary structures:

Series: One-dimensional labeled data.

DataFrame: Two-dimensional labeled data (like a spreadsheet).

Example:

import pandas as pd
data = {'Name': ['Ali', 'Sara'], 'Score': [85, 90]}
df = pd.DataFrame(data)
print(df)
Use Cases:

Data cleaning and transformation

Reading/writing CSV, Excel, or JSON files

Statistical summaries and exploration

📉 Matplotlib
The most widely used data visualization library.

Allows creating line charts, bar graphs, scatter plots, etc.

Example:

import matplotlib.pyplot as plt
plt.plot([1, 2, 3, 4], [10, 20, 25, 30])
plt.title("Simple Line Graph")
plt.xlabel("X-axis")
plt.ylabel("Y-axis")
plt.show()
Use Cases:

Plotting trends and visual data insights

Scientific research and analysis

📊 Seaborn
Built on top of Matplotlib for statistical data visualization.

Provides high-level functions for creating visually appealing charts.

Example:

import seaborn as sns
sns.barplot(x=["A", "B", "C"], y=[10, 20, 15])
Use Cases:

Creating heatmaps, distributions, and category comparisons

Statistical visualization for Data Science

🤖 2. Machine Learning & AI Libraries
⚙️ Scikit-learn
A simple and efficient tool for machine learning and data mining.

Provides algorithms for classification, regression, clustering, and model evaluation.

Example:

from sklearn.linear_model import LinearRegression
model = LinearRegression()
Use Cases:

Predictive analytics

Customer segmentation

Fraud detection

🧠 TensorFlow
Developed by Google for deep learning and AI applications.

Used for building and training neural networks.

Example:

import tensorflow as tf
print(tf.__version__)
Use Cases:

Deep learning and image recognition

Natural Language Processing (NLP)

AI model deployment

🔥 PyTorch
Developed by Meta (Facebook) for dynamic neural networks.

Preferred by researchers for its flexibility and simplicity.

Example:

import torch
x = torch.tensor([[1, 2], [3, 4]])
print(x)
Use Cases:

AI and machine learning research

Computer vision and NLP tasks

Reinforcement learning

🌐 3. Web Development Libraries
🌍 Flask
A lightweight and flexible web framework for creating web applications and APIs.

Example:

from flask import Flask
app = Flask(__name__)

@app.route('/')
def home():
    return "Hello, Flask!"
Use Cases:

REST API development

Web applications for small to medium-scale projects

🏗️ Django
A high-level web framework that supports rapid development and clean, pragmatic design.

Includes built-in ORM, authentication, and admin dashboard.

Example:

from django.http import HttpResponse
def home(request):
    return HttpResponse("Welcome to Django App!")
Use Cases:

Large-scale web apps

CMS, social media platforms, and enterprise apps

⚙️ 4. Automation & Utility Libraries
🤖 Selenium
Automates browsers for testing and web scraping.

Example:

from selenium import webdriver
driver = webdriver.Chrome()
driver.get("https://www.google.com")
Use Cases:

Automated testing

Web scraping

Data extraction

🧾 Requests
Simplifies making HTTP requests (GET, POST, PUT, DELETE).

Example:

import requests
response = requests.get("https://api.github.com")
print(response.status_code)
Use Cases:

API integrations

Web communication between servers

💾 OS and SYS
Provides functionality to interact with the operating system.

Example:

import os
print(os.getcwd())  # Current directory
Use Cases:

File management

Automating system tasks

Environment setup

🧩 5. Specialized Libraries
Domain	Library	Description
Game Development	pygame	Create 2D games and interactive applications.
Advanced Visualization	plotly, bokeh	Create interactive and real-time visualizations.
Natural Language Processing (NLP)	nltk, spaCy	Text analysis, tokenization, and sentiment analysis.
Computer Vision	opencv-python	Image and video analysis.
Finance & Economics	yfinance, QuantLib	Financial modeling and stock market analysis.
Excel Automation	openpyxl, xlrd	Read and write Excel spreadsheets.

🧠 Memory Management in Python
Python uses automatic memory management (Garbage Collection).

Variables with same immutable values (like integers or strings) share the same memory address.

Example:

a = 10
b = 10
print(id(a), id(b))  # Same memory address