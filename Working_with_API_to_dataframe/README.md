# 📊 Working with API to DataFrame (Python Project)

## 📌 Overview
This project shows how to fetch data from an API and convert it into a Pandas DataFrame for analysis.

## 🚀 Features
- Fetch data using API
- Convert JSON to DataFrame
- Select useful columns
- Handle multiple pages
- Create structured dataset

## 🛠️ Technologies Used
- Python
- Pandas
- Requests
- JSON

## 📂 Steps

1. Import libraries
import pandas as pd
import requests

2. Fetch API data
response = requests.get("API_URL")
data = response.json()

3. Convert to DataFrame
df = pd.DataFrame(data['results'])

4. Select columns
df = df[['id','title','overview','release_date','popularity','vote_average','vote_count']]

5. Multiple pages
final = pd.DataFrame()

for i in range(1, 429):
    response = requests.get(f"API_URL&page={i}")
    temp_df = pd.DataFrame(response.json()['results'])
    final = final.append(temp_df, ignore_index=True)

## 📊 Output
Clean DataFrame ready for analysis

## ⚠️ Notes
- Replace API_URL with your actual API
- Internet required
- Large data may take time

## 💡 Use Cases
- Data analysis
- Machine learning
- Visualization

## 📎 Conclusion
Helps in converting API data into structured format using Python
