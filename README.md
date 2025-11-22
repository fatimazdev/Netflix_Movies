# 🎬 Netflix Movies Exploratory Data Analysis (EDA)

![Netflix Logo](https://upload.wikimedia.org/wikipedia/commons/0/08/Netflix_2015_logo.svg)

## 📌 Project Overview
This project performs a comprehensive **Exploratory Data Analysis (EDA)** on the Netflix Movies dataset. The primary objective is to clean raw, unstructured data and derive meaningful insights regarding content distribution, duration, and genre popularity.

This script specifically handles real-world data challenges, such as parsing **stringified lists** (e.g., `"['US', 'GB']"`) and correcting column mismatches found in raw datasets.

## 🚀 Key Features

### 1️⃣ Advanced Data Cleaning
*   **Regex Parsing:** Utilizes Regular Expressions to clean messy string formats containing brackets and quotes.
*   **Column Mapping:** Automatically detects and maps correct column names (e.g., mapping `runtime` to Duration).
*   **Data Sanitization:** Handles missing values and formats country/genre data for accurate aggregation.

### 2️⃣ Feature Engineering
*   **Genre Explosion:** Uses `pandas.explode` to separate movies with multiple genres into distinct rows for accurate counting.
*   **Primary Country Extraction:** Isolates the main production country for multi-national films to simplify visualization.

### 3️⃣ Visualizations & Insights
*   🌍 **Top Producing Countries:** Identifies the top 10 countries contributing to Netflix's movie library.
*   ⏱️ **Runtime Distribution:** A histogram analysis of movie lengths.
*   🎭 **Genre Analysis:** A breakdown of the most popular movie genres.
*   📅 **Content Growth:** A time-series analysis of movie releases over the years.
*   ⏳ **Duration by Genre:** Analyzes which genres tend to have the longest runtimes.

## 🛠️ Tech Stack
*   **Python** 3.x
*   **Pandas** (Data Manipulation)
*   **NumPy** (Numerical Operations)
*   **Matplotlib & Seaborn** (Data Visualization)
*   **Re** (Regular Expressions)

## 📊 Visualizations Included
The script generates the following plots:
1.  **Bar Chart:** Top 10 Countries (Primary Producers).
2.  **Histogram:** Distribution of Movie Runtimes (KDE enabled).
3.  **Bar Chart:** Top 10 Most Popular Genres.
4.  **Line Plot:** Trend of Movie Releases over the years (1940-2024).
5.  **Bar Chart:** Average Duration per Genre.

## 💻 How to Run

1.  Clone the repository:
    ```bash
    git clone https://github.com/YOUR_USERNAME/Netflix-EDA.git
    ```
2.  Install the required dependencies:
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```
3.  Run the script (or Jupyter Notebook):
    ```bash
    python netflix_analysis.py
    ```
    *(Note: The dataset is fetched automatically from the online source within the script.)*

---
<div align="center">
  <sub>Developed with ❤️ by [Your Name]</sub>
</div>
