# Project 01 — Zomato Restaurant EDA & Insights Report

> **Pluto Academy AI & ML Internship Program**  
> Domain: Data Analysis & Visualization | Tech Stack: Python · Pandas · Matplotlib · Seaborn

---

## 📋 Project Overview

This project performs a complete **Exploratory Data Analysis (EDA)** on the Zomato Restaurants dataset sourced from Kaggle. The goal is to uncover patterns in restaurant ratings, cuisines, pricing, and city-wise distribution across India — and derive **5 actionable business insights** backed by data.

---

## 📁 Repository Structure

```
├── Project01_Zomato_EDA.ipynb   # Main Jupyter notebook (all code + outputs)
├── zomato.csv                   # Dataset (download from Kaggle link below)
├── charts/
│   ├── chart1_top_cities.png
│   ├── chart2_rating_distribution.png
│   ├── chart3_top_cuisines.png
│   ├── chart4_rating_by_price.png
│   ├── chart5_delivery_pie.png
│   ├── chart6_votes_vs_rating.png
│   └── chart7_heatmap_city_price.png
└── README.md
```

---

## 📊 Dataset

| Detail | Info |
|---|---|
| **Source** | [Kaggle — Zomato Restaurants Data](https://www.kaggle.com/datasets/shrutimehta/zomato-restaurants-data) |
| **File** | `zomato.csv` |
| **Size** | 9,551 rows × 21 columns |
| **India subset** | 8,652 restaurants |
| **Missing values** | 9 (only in `Cuisines` column) |

---

## 🔧 Tech Stack

| Library | Purpose |
|---|---|
| `pandas` | Data loading, cleaning, and EDA |
| `numpy` | Numerical operations |
| `matplotlib` | Chart creation |
| `seaborn` | Statistical visualizations and heatmaps |
| Google Colab | Cloud-based Python runtime |

---

## 🪜 Steps Followed

### Step 1 — Load & Inspect
- Loaded CSV with `encoding='latin-1'`
- Checked shape, column names, data types, missing values, and duplicates
- Written a 5-line data summary

### Step 2 — Clean the Data
- Dropped duplicate rows
- Removed irrelevant columns (`Address`, `Locality Verbose`, `Rating color`, etc.)
- Filled 9 missing `Cuisines` values with `'Unknown'`
- Filtered to **India only** (Country Code = 1) for consistent INR currency comparisons
- Fixed data types for numeric columns

### Step 3 — EDA (5 Questions)
1. Which cities have the most restaurants?
2. What is the distribution of aggregate ratings?
3. What are the most popular cuisines?
4. Does price range affect ratings?
5. Do restaurants with online delivery earn better ratings?

### Step 4 — Visualizations (7 Charts)
| # | Chart Type | Topic |
|---|---|---|
| 1 | Bar Chart | Top 10 Cities by Restaurant Count |
| 2 | Histogram | Rating Distribution with Mean & Median |
| 3 | Horizontal Bar | Top 15 Cuisines |
| 4 | Line Chart | Average Rating vs. Price Range |
| 5 | Pie Chart | Online Delivery Availability |
| 6 | Scatter Plot | Votes vs. Rating (coloured by Price Range) |
| 7 | Heatmap | Average Rating by City & Price Range |

### Step 5 — Insights Report
5 numbered business insights derived from analysis, each referencing a specific chart.

---

## 🔍 Key Findings

1. **New Delhi dominates** — 63% of all India listings (5,473 restaurants)
2. **Most ratings cluster between 3.0–4.0** — achieving 4.0+ is a real differentiator
3. **North Indian & Chinese cuisines oversaturate the market** — niche cuisines face less competition
4. **Premium restaurants (Price Range 4) consistently rate higher** — budget segment must compete harder on quality
5. **Restaurants with online delivery attract more votes and better ratings**

---

## 💡 Most Surprising Finding

New Delhi alone accounts for ~63% of all India Zomato listings, while large metros like Mumbai and Bangalore have very few entries. This reflects Zomato's early geographic expansion history — a stark reminder that datasets are always products of their collection context.

---

## ▶️ How to Run

1. Open [Google Colab](https://colab.research.google.com)
2. Upload `Project01_Zomato_EDA.ipynb`
3. Upload `zomato.csv` to the Colab session files
4. Click **Runtime → Run All**
5. All charts render inline in the notebook

---

## 👩‍💻 Author
**Vaibhav Araikar**
