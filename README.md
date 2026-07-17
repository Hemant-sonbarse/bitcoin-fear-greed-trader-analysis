# Bitcoin Fear Greed Trader Analysis

## Overview

This project analyzes the relationship between **Bitcoin Market Sentiment (Fear & Greed Index)** and **trader behavior on the Hyperliquid platform**.

The objective is to understand how different market sentiment conditions influence trading performance, trading activity, position sizing, and trader behavior. Based on these findings, actionable trading strategies are proposed.

---

## Objective

- Analyze the relationship between market sentiment and trader performance.
- Compare trading behavior during Fear, Greed, and Neutral market conditions.
- Segment traders based on their trading characteristics.
- Generate insights and strategy recommendations from the analysis.

---

## Dataset

### 1. Bitcoin Fear & Greed Index

**Columns**
- Date
- Sentiment Value
- Market Classification (Fear, Greed, Extreme Fear, Extreme Greed, Neutral)

### 2. Hyperliquid Historical Trading Data

Contains trade-level information including:

- Account
- Coin
- Execution Price
- Trade Size
- Buy/Sell Side
- Closed PnL
- Fees
- Timestamp
- Order Information

---

## Project Workflow

### 1. Data Preparation

- Loaded both datasets
- Checked dataset dimensions
- Verified missing values and duplicates
- Converted timestamps into daily dates
- Merged trading data with daily market sentiment

### 2. Feature Engineering

Created the following metrics:

- Daily PnL per trader
- Daily Win Rate
- Average Trade Size
- Number of Trades per Day
- Long/Short Ratio
- Trader Segments

### 3. Exploratory Data Analysis

Performed analysis on:

- Daily PnL by Market Sentiment
- Win Rate by Market Sentiment
- Trade Frequency by Market Sentiment
- Average Trade Size by Market Sentiment
- Long vs Short Position Ratio
- Trader Segmentation Analysis

---

## Key Insights

- Trader profitability varies across different market sentiment conditions.
- Fear periods showed higher trading activity than Greed periods.
- Larger position traders generated higher average profits than smaller traders.
- Frequent traders executed more trades, while consistent winners maintained stronger win rates across different market conditions.

---

## Strategy Recommendations

- Use market sentiment as an additional risk management indicator before opening positions.
- During Fear markets, prioritize disciplined position sizing instead of increasing trade frequency.
- During Extreme Greed periods, avoid excessive risk-taking and maintain disciplined position management.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Repository Structure

```
Trader-Performance-vs-Market-Sentiment/
│
├── Trader_Performance_Analysis.ipynb
├── README.md
├── requirements.txt
│
├── data/
│   ├── fear_greed_index.csv
│   └── historical_data.csv
│
└── charts/
    ├── average_daily_pnl.png
    ├── trade_frequency.png
    ├── average_trade_size.png
    ├── long_short_ratio.png
    └── trader_segments.png

```

---

## How to Run

1. Clone this repository.

```bash
git clone <repository-url>
```

2. Navigate to the project directory.

```bash
cd Trader-Performance-vs-Market-Sentiment
```

3. Install the required libraries.

```bash
pip install -r requirements.txt
```

4. Open the notebook.

```bash
jupyter notebook
```

5. Run all notebook cells from top to bottom.

---
