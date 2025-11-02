# Netflix-data-analysis
This repository contains a Netflix Data Analysis project that focuses on data cleaning, exploratory data analysis (EDA), and visualization. Using Python libraries like Pandas, Matplotlib, and Seaborn, the project extracts valuable insights to understand viewing trends and improve user experience on the platform.

# 🎬 Data Analysis | Netflix Data Analysis

## 📌 Project Overview  
This project focuses on analyzing Netflix's dataset to uncover patterns, trends, and insights that can help **enhance user experience**. The analysis includes **data cleaning, exploratory data analysis (EDA), and data visualization** using Python.  

## 🔍 Key Features  
✔️ **Cleaned & pre-processed the dataset** to ensure accuracy and consistency.  
✔️ **Performed Exploratory Data Analysis (EDA)** to discover insights about content trends.  
✔️ **Created visualizations** using **Matplotlib & Seaborn** to represent data meaningfully.  
✔️ **Addressed problem statements** to enhance recommendations and user engagement.  

## 🛠️ Technologies Used  
- **Python**  
- **Pandas** (for data manipulation)  
- **Matplotlib & Seaborn** (for visualization)  
- **NumPy**  
- **Jupyter Notebook**  

## 📊 Sample Analysis  
Here are some key insights from the analysis:  

### 🔹 Content Trends Over the Years  
```python
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd

# Load dataset
df = pd.read_csv("netflix_data.csv")

# Convert date to datetime format
df['release_year'] = pd.to_datetime(df['release_year'], errors='coerce')

# Plot content distribution by year
plt.figure(figsize=(10,5))

sns.histplot(df['release_year'].dropna(), bins=20, kde=True, color='red')
plt.title("Netflix Content Released Over the Years")
plt.xlabel("Year")
plt.ylabel("Count")
plt.show()
```

<hr>
<p align="center">
  <img src="Netflix.jpg" alt="Netflix" width="800">
</p>

