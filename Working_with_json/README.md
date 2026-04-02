# 📊 Working with JSON in Pandas

## 📌 Introduction
JSON (JavaScript Object Notation) is a lightweight and widely used data format for storing and exchanging data.  
It is commonly used in web APIs and data analysis tasks.

In this section, we use the Pandas library to read and manipulate JSON data.

---

## 🧰 Requirements

Install pandas if not already installed:

pip install pandas

---

## 📂 Reading JSON File

import pandas as pd

df = pd.read_json('train.json')
print(df.head())

### 🔍 Explanation
- pd.read_json() reads a JSON file
- Converts JSON data into a Pandas DataFrame
- Data is displayed in rows and columns format

---

## 🌐 Reading JSON from URL (API)

df = pd.read_json('https://api.exchangerate-api.com/v4/latest/INR')
print(df.head())

### 🔍 Explanation
- Reads JSON data directly from a web API
- Converts API response into a DataFrame
- Useful for real-time data analysis

---

## 📊 Example Structure of JSON Data

Example:

{
  "id": 10259,
  "cuisine": "greek",
  "ingredients": ["lettuce", "olives", "tomatoes"]
}

### 🔍 Explanation
- JSON can contain key-value pairs
- Values can be lists, strings, numbers, etc.
- Nested data can also be handled by Pandas

---

## ⚙️ Important Functions

- df.head() → Displays first 5 rows  
- df.shape → Shows number of rows and columns  
- df.columns → Shows column names  
- pd.read_json() → Reads JSON data  

---

## 🚀 Advantages of JSON

- Easy to read and write  
- Lightweight data format  
- Used in APIs and web services  
- Easy integration with Python  

---

## 🧠 Conclusion

Working with JSON in Pandas helps in handling structured and real-world data easily.  
It is an essential skill for data analysis and data science.
