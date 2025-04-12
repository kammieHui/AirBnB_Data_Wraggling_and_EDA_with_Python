# 🏠 Airbnb Data Cleaning with Python

### 📌 Project Overview
This project demonstrates practical data cleaning techniques on a real-world public dataset. The goal is to prepare the dataset for analysis by applying common data wrangling methods such as handling missing values, fixing data types, and removing duplicates.

---

### 📎 Dataset Information
- **Source**: Kaggle  
🔗 [Airbnb Open Dataset](https://www.kaggle.com/datasets/arianazmoudeh/airbnbopendata)  
🔗 [Data Dictionary](https://docs.google.com/spreadsheets/d/1b_dvmyhb_kAJhUmv81rAxl4KcXn0Pymz/edit?gid=1967362979#gid=1967362979)

- **Description**:  
  Airbnb listings in New York City, including details like price, ratings, availability, host info, and more.

- **Original Size**: 102,599 rows × 26 columns  
- **Purpose**: To clean and structure the data for further exploratory data analysis (EDA) and insights.

---

### 🧼 Data Cleaning Summary

#### 🔍 Objectives
1. Handle missing and null values  
2. Standardize column names and data types  
3. Remove duplicates  
4. Fix incorrect or inconsistent values  
5. Drop irrelevant or redundant columns  
6. Prepare data for analysis (e.g., convert `price` to float, parse dates)

---
### 📊 EDA Summary
•	📌 **Count Plot Subplots**<br>
&emsp;Visualized distributions of key categorical variables.<br>
<br>
•	📦 **Box Plot Subplots**<br>
&emsp;Examined spread and outliers in numerical variables.<br>
<br>
•	🏙️ **Bar Chart: Top 30 Neighborhoods by Listings**<br>
&emsp;Highlighted the most active areas based on listing counts.<br>
<br>
•	💰 **Stacked Histogram: Listing Price Distribution by Neighborhood Group**<br>
&emsp;Compared price ranges across different neighborhood groups.<br>
<br>
•	🏗️ **Stacked Bar Chart: Listings by Year Built (per Neighborhood Group)**<br>
&emsp;Analyzed the age distribution of listings geographically.<br>
<br>
•	🛏️ **Stacked Bar Chart: Room Type Distribution by Neighborhood Group**<br>
&emsp;Observed how room types vary across locations.<br>
<br>
•	🧊 **Correlation Heatmap (sns.heatmap)**<br>
&emsp;Explored relationships between numeric features such as price, reviews, availability, and more.<br>
<br>
•	📍 **Scatter Plot: Price vs. Service Fee**<br>
&emsp;Investigated the relationship between listing price and service fees.<br>
<br>
•	☁️ **Word Cloud: House Rules**<br>
&emsp;Visualized most common phrases in the house rules section.<br>

---
### 🧠 Insights or business takeaways
## 📊 Key Insights from Data Visualizations

### Host & Review Patterns
- Nearly 50% of hosts are not identity-verified, raising potential safety concerns.
- Majority of listings are *entire homes* or *private rooms*.
- Guest reviews mostly fall within the 2–5 star range.

### Outlier Detection
- Outliers found in: `minimum_nights`, `number_of_reviews`, `reviews_per_month`,  
  `calculated_host_listings_count`, and `availability_365`.

### Listing Price Distribution
- Listing prices are fairly evenly distributed across all neighborhood groups.

### Home Age by Neighborhood
- The age of homes (year built) is similarly distributed across neighborhoods.

### Correlation Insights
- Strong correlation found between *listing price* and *service fee*.

### Price vs. Service Fee Patterns
- Identified three service fee calculation models:
  - **Fixed Fees** – Flat fee regardless of price (vertical lines).
  - **Proportional Fees** – Fee scales with price (diagonal trend).
  - **Flat Fees at Specific Price Points** – Notably around $620 (horizontal clusters).
- Most listings appear to use proportional service fees.
---
### 📓 Jupyter Notebook
- 🧹 [Data Cleaning Notebook](notebooks/1_data_cleaning_airbnb.ipynb)  
- 📊 [EDA & Visualization Notebook](notebooks/2_eda_visualization_airbnb.ipynb) 

---
### 🛠 Tools Used
- Python (Pandas, NumPy, Matplotlib, seaborn, wordcloud)

