# News Sentiment Analysis for Stock Market Prediction

## Overview

This project is part of the **10 Academy Artificial Intelligence Mastery – Week 1 Challenge**.

The goal of the project is to investigate the relationship between financial news sentiment and stock market price movements. The project combines Natural Language Processing (NLP), exploratory data analysis, financial technical indicators, and statistical correlation analysis to determine whether news sentiment can help predict stock behavior.

---

# Business Objective

Nova Financial Solutions aims to improve financial forecasting accuracy by integrating qualitative financial news with quantitative stock market data.

This project focuses on:

- Performing sentiment analysis on financial news headlines
- Computing financial technical indicators from historical stock prices
- Measuring correlations between sentiment and stock returns
- Generating actionable insights for investment strategy development

---

# Project Structure

```text
news-sentiment-analysis/
│
├── .github/
│   └── workflows/
│       └── unittests.yml
│
├── data/
│   └── raw/
│
├── notebooks/
│   ├── task1_eda.ipynb
│   ├── task2_quantitative.ipynb
│   └── task3_correlation.ipynb
│
├── src/
│
├── tests/
│
├── scripts/
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

# Tasks Completed

## Task 1 — Exploratory Data Analysis (EDA)

Performed exploratory analysis on the financial news dataset, including:

* Headline length distribution analysis
* Publisher activity analysis
* Time-series analysis of article publication frequency
* Keyword extraction using TF-IDF
* Visualization of news trends and patterns

### Key Insights

* Certain publishers dominate financial news generation
* News publication frequency varies over time with noticeable spikes
* Financial headlines commonly include terms related to earnings, stock targets, and market performance

---

## Task 2 — Quantitative Financial Analysis

Performed technical analysis using historical stock price data.

### Technical Indicators Computed

* Simple Moving Average (SMA)
* Exponential Moving Average (EMA)
* Relative Strength Index (RSI)
* Moving Average Convergence Divergence (MACD)

### Objectives

* Understand stock price trends
* Detect momentum shifts
* Identify overbought and oversold conditions

---

## Task 3 — Sentiment and Correlation Analysis

Performed sentiment analysis on financial news headlines and measured relationships with stock returns.

### Methods Used

* VADER sentiment analysis
* Daily sentiment aggregation
* Daily stock return calculation
* Pearson correlation analysis

### Goals

* Determine whether positive or negative sentiment aligns with stock movements
* Analyze the predictive potential of financial news sentiment

---

# Technologies Used

## Programming Language

* Python 3.11

## Libraries

* pandas
* numpy
* matplotlib
* scikit-learn
* nltk
* vaderSentiment
* TA-Lib
* yfinance
* pynance
* jupyter

---

# Installation

## Clone Repository

```bash
git clone <repository-url>
cd news-sentiment-analysis
```

## Create Virtual Environment

### Windows

```bash
python -m venv .venv
.venv\Scripts\activate
```

### Mac/Linux

```bash
python3 -m venv .venv
source .venv/bin/activate
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Running the Project

## Start Jupyter Notebook

```bash
jupyter notebook
```

Open the notebooks directory and run:

* `task1_eda.ipynb`
* `task2_quantitative.ipynb`
* `task3_correlation.ipynb`

---

# Data Sources

## Financial News Dataset

Financial News and Stock Price Integration Dataset (FNSPID)

Dataset fields include:

* headline
* publisher
* date
* stock
* url

## Historical Stock Data

Historical stock prices obtained using the `yfinance` library.

Fields include:

* Open
* High
* Low
* Close
* Adj Close
* Volume

---

# Example Visualizations

The project includes visualizations for:

* Headline length distributions
* Top publishers
* Daily news volume trends
* TF-IDF keyword importance
* Stock price trends with moving averages
* RSI and MACD indicators
* Sentiment vs stock return correlation scatter plots

---

# Challenges Encountered

* Mixed datetime formats in news data
* Timezone normalization issues
* Handling missing values
* Aligning non-trading day news with stock trading dates
* TA-Lib installation compatibility issues

---

# Future Improvements

Potential future enhancements include:

* Advanced transformer-based sentiment analysis (FinBERT)
* Lagged sentiment impact analysis
* Event-driven trading strategies
* Multi-stock comparative analysis
* Predictive machine learning models

---

# CI/CD

GitHub Actions is configured for continuous integration and automated testing.

Workflow file:

```text
.github/workflows/unittests.yml
```

---

# Author

Hemen

10 Academy — Artificial Intelligence Mastery Program

---

# License

This project is for educational and research purposes.

```

