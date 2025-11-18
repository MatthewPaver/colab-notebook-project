# 📺 Netflix Content Analysis - Colab Notebook

<div align="center">

### 🎬 Netflix Dataset Analysis | 📊 Content Trends | 📈 Data Visualisation

**Comprehensive analysis of Netflix titles dataset to identify content trends, patterns, and insights**

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WsnSnIngH8xNdBNBWeJgJbKD2uMilVdS?usp=sharing)
[![Python](https://img.shields.io/badge/Python-3.x-3670A0?style=flat-square&logo=python&logoColor=ffdd54)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat-square&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![pandas](https://img.shields.io/badge/pandas-Data_Analysis-150458?style=flat-square&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualisation-11557C?style=flat-square&logo=matplotlib&logoColor=white)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-Visualisation-3776AB?style=flat-square&logo=python&logoColor=white)](https://seaborn.pydata.org/)

</div>

---

## 📋 Overview

This Google Colab notebook performs a comprehensive analysis of the Netflix titles dataset to identify content trends, patterns, and insights. The analysis explores content distribution by country and genre, visualises content additions over time, and identifies unusual patterns in Netflix's content acquisition strategy.

### 🎯 Analysis Objectives

- **🌍 Content Trends by Country** — Identify which countries produce the most Netflix content
- **🎭 Content Trends by Genre** — Analyse genre distribution and popularity
- **📅 Content Additions by Year** — Visualise how Netflix's content library has grown over time
- **🔍 Unusual Patterns Detection** — Identify significant spikes or drops in yearly content additions

---

## 🔍 Key Findings

### Top Countries with Most Netflix Content

1. **United States** — 2,818 titles
2. **India** — 972 titles
3. **Unknown** — 831 titles
4. **United Kingdom** — 419 titles
5. **Japan** — 245 titles

### Top Genres on Netflix

1. **Dramas, International Movies** — 362 titles
2. **Documentaries** — 359 titles
3. **Stand-Up Comedy** — 334 titles
4. **Comedies, Dramas, International Movies** — 274 titles
5. **Dramas, Independent Movies, International Movies** — 252 titles

### Content Addition Trends

- **Overall Trend:** General upward trajectory, accelerating from 2016 onwards
- **Peak Year:** 2019 saw the highest number of content additions
- **Unusual Spikes:** Significant increases in 2017 (+759 titles) and 2018 (+461 titles)
- **Recent Trend:** Slight decrease in 2020 and 2021

---

## 📊 Analysis Components

### 1. Data Loading & Cleaning

- Load Netflix titles dataset from CSV
- Handle missing values in key columns (`director`, `cast`, `country`)
- Replace missing values with "Unknown" placeholder
- Verify data integrity

### 2. Country Analysis

- Count titles per country
- Identify top countries by content volume
- Visualise top 10 countries with bar charts
- Analyse geographic content distribution

### 3. Genre Analysis

- Count titles per genre combination
- Identify most popular genres
- Visualise top 10 genres with bar charts
- Explore genre diversity and trends

### 4. Temporal Analysis

- Extract year from `date_added` column
- Count titles added per year
- Calculate year-over-year changes
- Identify unusual patterns (spikes and drops)

### 5. Visualisations

- **Bar Charts** — Top countries and genres
- **Line Plots** — Content additions over time
- **Statistical Analysis** — Year-over-year change detection

---

## 🛠️ Technologies & Libraries

### Core Technologies

- **Python** — Programming language
- **Google Colab** — Interactive notebook environment
- **Jupyter Notebook** — Notebook format

### Data Science Libraries

- **pandas** — Data manipulation and analysis
- **NumPy** — Numerical computing (implicit)
- **Matplotlib** — Data visualisation
- **Seaborn** — Statistical data visualisation

---

## 📈 Methodology

### Data Preprocessing

1. **Loading:** Import CSV data into pandas DataFrame
2. **Cleaning:** Handle missing values in `director`, `cast`, and `country` columns
3. **Transformation:** Extract year from `date_added` column using `pd.to_datetime()`

### Analysis Techniques

1. **Value Counting** — Use `value_counts()` to identify top categories
2. **Time Series Analysis** — Extract temporal patterns from date columns
3. **Statistical Detection** — Calculate standard deviation to identify outliers
4. **Visualisation** — Create bar charts and line plots for trend analysis

### Pattern Detection

- **Threshold Method:** Use 1.5 × standard deviation to identify unusual patterns
- **Year-over-Year Comparison:** Calculate differences between consecutive years
- **Spike Detection:** Identify years with increases above threshold
- **Drop Detection:** Identify years with decreases below threshold

---

## 🔗 Access the Notebook

- **Open in Google Colab:** [Launch Notebook](https://colab.research.google.com/drive/1WsnSnIngH8xNdBNBWeJgJbKD2uMilVdS?usp=sharing)
- **Dataset:** Netflix titles CSV file (`/content/netflix_titles.csv`)

---

## 📝 Notebook Structure

The notebook follows a structured analysis workflow:

1. **Load the Data** — Import and verify dataset
2. **Clean the Data** — Handle missing values
3. **Analyse Content Trends by Country** — Geographic distribution
4. **Analyse Content Trends by Genre** — Genre popularity
5. **Analyse Content Trends by Year** — Temporal patterns
6. **Highlight Unusual Patterns** — Statistical anomaly detection
7. **Visualise Trends** — Create charts and plots
8. **Summarise Findings** — Present key insights

---

## 💡 Key Insights

### Content Strategy Observations

- **US Dominance:** United States accounts for the largest share of Netflix content
- **International Growth:** Strong presence from India, UK, and Japan
- **Genre Diversity:** Wide variety of genre combinations, with dramas and international content leading
- **Growth Acceleration:** Significant content expansion from 2016-2019
- **Acquisition Spikes:** 2017-2018 saw unusual spikes in content additions

### Potential Next Steps

- Investigate factors contributing to 2017-2018 content spikes
- Analyse the "Unknown" country category to identify potential regions
- Explore relationships between country and genre preferences
- Examine content release patterns by month or season

---

## 📊 Visualisations Included

- **Top 10 Countries Bar Chart** — Visual representation of country distribution
- **Top 10 Genres Bar Chart** — Genre popularity visualisation
- **Yearly Additions Line Plot** — Temporal trend visualisation

---

## 🎓 Learning Outcomes

This notebook demonstrates:

- **Data Cleaning** — Handling missing values and data quality issues
- **Exploratory Data Analysis (EDA)** — Understanding data distributions
- **Statistical Analysis** — Pattern detection and anomaly identification
- **Data Visualisation** — Creating informative charts and plots
- **Time Series Analysis** — Analysing temporal trends and patterns
- **Insight Generation** — Drawing meaningful conclusions from data

---

## 📄 Dataset Information

- **Source:** Netflix titles dataset (`netflix_titles.csv`)
- **Format:** CSV file
- **Key Columns:**
  - `title` — Title of the content
  - `country` — Country of origin
  - `listed_in` — Genre classification
  - `date_added` — Date added to Netflix
  - `director` — Director name
  - `cast` — Cast members

---

## 🔗 Related Projects

- [Profile](https://github.com/MatthewPaver) — View all my projects
- [Marketing ML Lakehouse](https://github.com/MatthewPaver/marketing-ml-lakehouse) — End-to-end analytics pipeline
- [Sentence Similarity Analysis](https://github.com/MatthewPaver/sentence-similarity-analysis) — NLP and embeddings project

---

<div align="center">

**Built with ❤️ using Python, pandas, and data visualisation libraries**

[← Back to Profile](https://github.com/MatthewPaver)

</div>
