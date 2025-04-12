# 🏠 Airbnb Data Cleaning with Python

## 📌 Project Overview
This project demonstrates practical data cleaning techniques on a real-world public dataset. The goal is to prepare the dataset for analysis by applying common data wrangling methods such as handling missing values, fixing data types, and removing duplicates.

---

## 📎 Dataset Information
- **Source**: [Kaggle - NYC Airbnb Open Data](https://www.kaggle.com/datasets/arianazmoudeh/airbnbopendata)  
- **Data Dictionary**[Link](https://docs.google.com/spreadsheets/d/1b_dvmyhb_kAJhUmv81rAxl4KcXn0Pymz/edit?gid=1967362979#gid=1967362979)

- **Description**: 102,599 Airbnb listings with details like price, host identity, reviews, availability, and location.

> 🔄 Cleaned data available as a sample: [`cleaned_sample.csv`](#)  
> 📁 Full cleaned dataset hosted on [Google Drive](https://docs.google.com/spreadsheets/d/1b6iS2Avj_a0ZmeY5rOyIxYSrMi31SKy_4HhuNeVttCo/edit?usp=sharing) (not uploaded due to GitHub's 25MB limit)
---

## 🧼 Data Cleaning Summary
** 🔍 Objectives:**
- Handle missing/null values
- Standardize column names and data types
- Remove duplicates
- Fix inconsistent values
- Drop irrelevant columns
- Convert fields (e.g. `price` to float, date parsing)
  
📓 [Notebook:](notebooks/1_data_cleaning_airbnb.ipynb) 
---
## 📊 Exploratory Data Analysis (EDA)
📓 [Notebook:](notebooks/2_eda_visualization_airbnb.ipynb) 

Key Visualizations:
- **Count Plots**: Host verification, room types, and review scores
- **Box Plots**: Identified outliers in several numerical fields
- **Top 30 Neighborhoods**: Based on listing volume
- **Stacked Histograms**: Price distributions by neighborhood group
- **Bar Charts**: Distribution of listing age and room type across locations
- **Correlation Heatmap**: Relationships between price, reviews, and availability
- **Scatter Plot**: Price vs. service fee (reveals 3 charging models)
- **Word Cloud**: Most common house rules

---
## 📌 Key Insights

### Host & Review Patterns
- ~ 50% of hosts are not identity-verified — potential safety concern
- Most listings are entire homes or private rooms
- Reviews mostly fall in the 2–5 range

### Outlier Detection
- Outliers found in: `minimum_nights`, `number_of_reviews`, `reviews_per_month`
- `calculated_host_listings_count`, `availability_365`.

### Listing Price Distribution
- Listing prices are fairly evenly distributed across all neighborhood groups.

### Price vs. Service Fee Patterns
- Price and service fee are strongly correlated
- 3 service fee models observed:
  - **Fixed Fees** (flat rate)
  - **Proportional Fees** (price × rate)
  - **Specific Price Point Fees** (e.g., $620 cluster)
---
## 🛠 Tools Used
- Python (Pandas, NumPy, Matplotlib, seaborn, wordcloud)
- Jupyter Notebook

---
## ⚙️ How to Reproduce
1. Download raw dataset from [Kaggle](#)
2. Run the notebooks in the `notebooks/` folder:
   - `1_data_cleaning.ipynb`
   - `2_eda_visualizations.ipynb`


