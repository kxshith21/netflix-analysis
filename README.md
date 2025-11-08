# netflix-analysis
# 🎬 Netflix Data Cleaning & Exploratory Data Analysis (EDA)

## 📖 Project Overview
This project focuses on **data cleaning** and **exploratory data analysis (EDA)** of the Netflix dataset to uncover insights about the platform’s content library, genres, countries, and release trends.  
The goal is to understand how Netflix’s catalog has evolved over the years and which content types and genres dominate its collection.

---

## 🧰 Tools & Technologies
- **Programming Language:** Python  
- **Libraries Used:**  
  - `pandas` – for data cleaning and manipulation  
  - `numpy` – for numerical operations  
  - `matplotlib` & `seaborn` – for data visualization  
  - `datetime` – for handling date columns  
- **IDE:** Jupyter Notebook  

---

## 🧹 Data Cleaning Steps
1. **Loaded** the dataset and explored its structure (rows, columns, datatypes).  
2. **Handled missing values** — filled or dropped based on relevance.  
3. **Removed duplicates** to ensure data accuracy.  
4. **Standardized column formats** (dates, categorical text, etc.).  
5. **Created new derived columns** such as content age, release year, and content type indicators.  

---

## 📊 Exploratory Data Analysis (EDA)
Performed detailed visual and statistical analysis to answer key questions:

### 1️⃣ Content Distribution
- Netflix hosts **more Movies than TV Shows**, with movies making up ~70% of total titles.

### 2️⃣ Country Insights
- **The United States** dominates in content production, followed by India and the UK.

### 3️⃣ Yearly Trends
- Netflix adds around **1500–1750 new titles each year**, showing rapid content growth since 2015.

### 4️⃣ Ratings Analysis
- The most common rating is **TV-MA**, indicating mature audience content is popular.

### 5️⃣ Genre Trends
- **Drama** and **International Movies** are the most frequent genres in the dataset.

---

## 📈 Key Insights
- Netflix’s content library leans heavily toward movies.  
- Global diversity is increasing, with international titles growing each year.  
- Most titles are suitable for adults (TV-MA).  
- There’s a noticeable rise in content after 2015 due to Netflix’s global expansion.  

---

## 🧩 Challenges Faced
- Handling missing data for country and director fields.  
- Normalizing inconsistent categorical entries.  
- Deciding when to drop vs. fill missing data values.

---

## 📂 Dataset
- **Source:** [Netflix Movies and TV Shows Dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows)  
- **Size:** ~8,800 rows and 12 columns  
- **Attributes Include:**  
  `show_id`, `type`, `title`, `director`, `cast`, `country`, `date_added`, `release_year`, `rating`, `duration`, `listed_in`, `description`

---

## 📷 Visuals
> *(Add your generated plots here as images — e.g. content type count, yearly release trend, top countries, rating distribution)*

Example:
```python
plt.figure(figsize=(8,5))
sns.countplot(data=df, x='type', palette='Set2')
plt.title("Movies vs TV Shows on Netflix")
plt.show()
