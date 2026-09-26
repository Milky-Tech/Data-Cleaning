# Cricket Test Match Data - Cleaning & EDA

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Cleaning-150458?logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-Data%20Visualization-3776AB?logoColor=white)

This repository contains a comprehensive Python script (`task_23.py`) originally developed as a Jupyter Notebook on Google Colab. The project focuses on Data Cleaning, Feature Engineering, and Exploratory Data Analysis (EDA) on a dataset comprising Cricket Test Match records.

## 📌 Project Overview

Raw data often contains inconsistencies, missing values, and formatting issues. This project demonstrates a complete data preprocessing workflow using **Pandas**, transforming messy cricket statistics into a structured, analysis-ready format. Once cleaned, the script dives into Exploratory Data Analysis (EDA) to uncover insights about player performances, career spans, and batting statistics using **Matplotlib** and **Seaborn**.

## ✨ Features & Workflow

### 1. Data Cleaning
- **Standardizing Columns:** Renames multiple cryptic columns (e.g., `NO` to `Not_Cuts`, `SR` to `Betting_Strike_Rate`) for better readability.
- **Handling Nulls & Duplicates:** Identifies and resolves missing values and removes duplicate player entries to ensure data integrity.
- **String Parsing & Formatting:** Cleans symbols (like `*` and `+`) from numerical columns and properly formats text data.

### 2. Feature Engineering
- **Career Span Extraction:** Splits the original `Span` column into distinct `Rookie_Year` and `Last_Year` numerical features.
- **Career Length Calculation:** Derives a new `Career_Length` feature based on rookie and last years.
- **Country Extraction:** Dynamically parses the `Player` column to extract the player's national team/country into its own dedicated feature.

### 3. Exploratory Data Analysis (EDA)
- **Univariate Analysis:** Explores individual features via descriptive statistics, value counts, and histograms (e.g., distribution of centuries `100`).
- **Bivariate Analysis & Visualization:** 
  - Scatter plots visualizing the relationship between centuries (`100`) and half-centuries (`50`).
  - Bar charts highlighting the Top 10 Players.
- **Correlation:** Computes and visualizes the correlation matrix between different scoring metrics using a Seaborn Heatmap.

## 🛠️ Technologies Used
- **Python** (Core logic)
- **Pandas** (Data manipulation and cleaning)
- **Matplotlib / Seaborn** (Data visualization)

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Milky-Tech/Data-Cleaning.git
   cd Data-Cleaning
   ```

2. **Install dependencies:**
   Ensure you have Pandas, Matplotlib, and Seaborn installed. You can install them via pip:
   ```bash
   pip install pandas matplotlib seaborn
   ```

3. **Provide the Dataset:**
   Ensure the `Cricket Test Match Data.csv` file is placed in the root directory before running the script.

4. **Execute the script:**
   ```bash
   python task_23.py
   ```
   *(Alternatively, run the code in a Jupyter/Colab Notebook for a more interactive experience).*

## 📈 Example Insights Generated
- Average career lengths across test players.
- Highest individual scores grouped by country.
- Correlation matrices identifying relationships between different batting milestones.
