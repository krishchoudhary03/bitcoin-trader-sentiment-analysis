# Trader Behavior vs Bitcoin Market Sentiment

## Overview

This project explores the relationship between **trader performance and Bitcoin market sentiment** using historical trading data from Hyperliquid and the Bitcoin Fear & Greed Index.

The goal of this analysis is to understand how **market psychology (fear vs greed)** influences trader behavior, profitability, trade direction, and overall trading activity.

By combining sentiment data with actual trading records, the project identifies patterns that could help improve **trading strategy design and risk management**.

---

## Datasets

### 1. Hyperliquid Historical Trader Data

This dataset contains individual trade information including:

* Account (Trader ID)
* Coin traded
* Execution price
* Trade size (tokens and USD)
* Trade side (Buy/Sell)
* Timestamp
* Closed PnL
* Transaction metadata

This dataset allows analysis of **real trader behavior and profitability**.

---

### 2. Bitcoin Fear & Greed Index

The Fear & Greed dataset provides daily sentiment classification of the Bitcoin market.

Sentiment categories include:

* **Fear**
* **Greed**
* **Extreme Fear**
* **Extreme Greed**
* **Neutral**

Market sentiment is widely used in trading to understand **investor psychology and market momentum**.

---

## Objective

The main objective of this project is to investigate how **market sentiment affects trader behavior and trading outcomes**.

Key questions explored include:

* Do traders perform better during **fear or greed markets**?
* Does trading activity increase during certain sentiment phases?
* How does sentiment influence **trade size and risk-taking**?
* Which coins generate the most trader profits?
* Do a small number of traders dominate overall profitability?

---

## Methodology

The analysis was performed using **Python and Google Colab**, following a standard data analysis workflow:

### 1. Data Cleaning

* Converted timestamp fields to datetime format
* Extracted trade dates from timestamps
* Converted profit/loss values to numeric format
* Removed extreme outliers from Closed PnL values

### 2. Data Integration

The trader dataset was merged with the Fear & Greed dataset using the **date field** so that each trade is associated with the corresponding market sentiment.

### 3. Exploratory Data Analysis

Several analyses were performed to identify patterns in trader behavior:

* Profit distribution across sentiment categories
* Trade direction vs sentiment
* Trading activity during different market phases
* Top traders by total profit
* Profitability by coin
* Win rate analysis
* Average trade size during different sentiment conditions

### 4. Visualization

Charts were generated using **Matplotlib and Seaborn** to highlight patterns in the data.

---

## Key Insights

### 1. Market Sentiment Influences Trading Behavior

Trading activity tends to increase during **Greed market phases**, indicating higher market participation and confidence among traders.

### 2. Profitability Varies Across Sentiment Conditions

Trader profits show noticeable variation across different sentiment phases, suggesting that market psychology may influence trading outcomes.

### 3. Risk-Taking Behavior Changes With Sentiment

Average trade size increases during **Greed markets**, suggesting traders are willing to take larger positions when market sentiment is positive.

### 4. Profit Concentration Among Traders

A relatively small group of traders accounts for a large share of total profits, which is commonly observed in trading ecosystems.

### 5. Coin-Level Profitability Differences

Some coins generate significantly higher cumulative profits than others, indicating that traders may prefer specific assets depending on market conditions.

---

## Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Google Colab

---

## Repository Structure

```
trader-sentiment-analysis
│
├── trader_sentiment_analysis.ipynb
├── historical_data.csv
├── fear_greed_index.csv
└── README.md
```

---

## Conclusion

This project demonstrates how combining **market sentiment data with trader activity data** can provide valuable insights into trading behavior and profitability patterns.

Understanding how traders react to different sentiment phases can help inform **better trading strategies, risk management frameworks, and market analysis models**.

---

## Author

Krish Choudhary
