# 🍷 Wine Reviews & YouTube Trends Analysis (Kaggle Practice Hub)

[![Python 3.8+](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.0%2B-blue.svg)](https://pandas.pydata.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![Kaggle](https://img.shields.io/badge/Kaggle-Datasets-20BEFF.svg)](https://www.kaggle.com/)

## 📌 About the Project

This project is a comprehensive data analysis practice using the **Pandas** library on real-world Kaggle datasets. The main goal is to demonstrate proficiency in data manipulation, filtering, grouping, merging tables, and solving business problems using Python.

Three main datasets are used in this project:
1.  **Wine Reviews** — for practicing indexing, filtering, and aggregation.
2.  **YouTube Trending Videos** (Canada & UK) — for practicing data concatenation, joining, and time series analysis.
3.  **Reddit Products** & **Powerlifting Database** — to demonstrate working with MultiIndex and complex data slicing.

## 🎯 Tasks & Implementation

The project is organized into logical sections, each solving specific analytical tasks:

### 1. Pandas Basics (DataFrame & Series)
*   **Creating Structures:** Generating DataFrames and Series from dictionaries with custom indices.
*   **Data Attributes:** Determining data types (`dtype`), record counts, and unique values.

### 2. Indexing & Filtering (loc, iloc, boolean indexing)
*   **Precise Selection:** Using `loc` to select rows by labels and columns (e.g., `df.loc[[0,1,10], ['country', 'points']]`).
*   **Conditional Filtering:** Selecting Italian wines with ratings above 90 points (`(country == 'Italy') & (points >= 90)`).
*   **Handling Missing Values:** Filtering rows where price is not specified (`price.notnull()`).

### 3. Aggregation & Analytics (groupby, agg, value_counts)
*   **Statistics:** Calculating mean, median, and descriptive statistics (`describe`).
*   **Top Analysis:** Identifying the country with the most reviews (`value_counts`).
*   **Customization:** Creating a function to convert ratings into stars (3 stars for 95+ points or wine from Canada).

### 4. String Operations & Date Handling
*   **Text Analysis:** Counting occurrences of the words "fruity" and "tropical" in wine descriptions (using `map` and `lambda`).

### 5. Data Combination (Concatenation & Joins)
*   **Vertical Concatenation:** Merging videos from Canada and the UK (`pd.concat`).
*   **Horizontal Joining:** Creating a combined dataframe for gamers and movie enthusiasts on Reddit.

## 🛠 Technologies & Skills Used

*   **Language:** Python 3.
*   **Libraries:** Pandas (core), KaggleHub (data download).
*   **Pandas Techniques:**
    *   `pd.DataFrame`, `pd.Series`
    *   `.loc[]`, `.iloc[]`, `.isin()`
    *   `.groupby()`, `.agg()`, `.apply()`
    *   `pd.concat()`, `df.join()`
    *   Handling missing data (`.fillna()`, `.isnull()`)
    *   Renaming columns and indexes (`.rename()`)

## 📊 Key Insights (Examples)

During the execution of this notebook, the following insights were discovered:
*   **Winemaking:** The most expensive bottle in the dataset costs $3,300 (France), while the highest-rated wine (100 points) is an Australian "Chambers Rosewood Vineyards NV Rare Muscat".
*   **YouTube:** Trending content in Canada and the UK is dominated by music videos and comedy content.
*   **Linguistics:** The word "fruity" appears in wine descriptions nearly three times more often than "tropical".

## 🚀 How to Run the Project

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/kaggle_practice_hub.git
    ```
2.  **Install dependencies:**
    ```bash
    pip install pandas kagglehub
    ```
    *(Using a virtual environment is recommended)*
3.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook kaggle_practice_pandas.ipynb
    ```

## 📁 Repository Structure

```
kaggle_practice_hub/
├── kaggle_practice_pandas.ipynb  # Main analysis file
├── README.md                     # Project description (this file)
└── requirements.txt              # Dependencies (pandas, kagglehub)
```

## 📈 Conclusions & Future Improvements

This project demonstrates solid proficiency in basic and advanced Pandas functionality for Exploratory Data Analysis (EDA).

**Planned improvements:**
*   Add visualizations (Matplotlib/Seaborn) for price and rating distribution charts.
*   Perform data cleaning to remove duplicates and outliers.
*   Implement simple scripts to download the latest versions of datasets via `kagglehub`.

---
⭐️ *If you like this project or find it useful for your learning, please give it a star on GitHub!*