# 📊 Working with CSV Files in Python

## 📌 Overview
This notebook demonstrates how to work with CSV (Comma-Separated Values) files using Python. It covers reading, processing, and analyzing CSV data using powerful libraries like Pandas.

The goal is to help beginners understand how to efficiently handle structured datasets in real-world projects such as Data Analysis and Machine Learning.

---

## 🚀 Features Covered

- Reading CSV files from:
  - Local system
  - URLs (GitHub/raw links)
- Understanding parameters of pd.read_csv()
- Handling missing values
- Selecting specific columns
- Renaming columns using converters
- Chunking large datasets
- Basic data exploration

---

## 🛠️ Technologies Used

- Python
- Pandas
- Requests

---

## 📂 Dataset

The notebook uses datasets from online sources such as:
- GitHub repositories
- Public CSV datasets

---

## 🔑 Key Concepts Explained

### 1. Reading CSV File
import pandas as pd

df = pd.read_csv("file.csv")

### 2. Reading from URL
url = "your_dataset_url"
df = pd.read_csv(url)

### 3. Selecting Columns
df = pd.read_csv(url, usecols=['column1', 'column2'])

### 4. Handling Missing Values
df.isnull().sum()

### 5. Using Converters
df = pd.read_csv(url, converters={'column_name': function_name})

### 6. Reading Large Files in Chunks
for chunk in pd.read_csv(url, chunksize=1000):
    print(chunk.shape)

---

## 📈 Use Cases

- Data preprocessing for Machine Learning
- Data cleaning and transformation
- Exploratory Data Analysis (EDA)
- Handling large datasets efficiently

---

## ⚠️ Common Issues & Fixes

Problem: Wrong URL  
Solution: Use raw GitHub link  

Problem: Encoding error  
Solution: Use encoding='latin-1'  

Problem: Memory issue  
Solution: Use chunksize  

Problem: Missing headers  
Solution: Use header parameter  

---

## 💡 Tips

Always inspect data using:
df.head()  
df.info()  
df.describe()  

- Use chunking for large datasets to avoid memory errors.
- Clean data before applying ML models.

---

## 📚 Conclusion

This notebook provides a strong foundation for working with CSV files in Python. Mastering these concepts is essential for Data Science, Machine Learning, and real-world data handling tasks.

---

## ✨ Author
Khushi Agarwal  
(B.Tech Student | Aspiring Data Scientist 🚀)
