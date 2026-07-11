# Crypto Trading Behavior Analysis using Market Sentiment

## Project Overview

This project analyzes historical cryptocurrency trading data to understand how trader performance and behavior change under different market sentiment conditions. The analysis combines historical trade records with the Bitcoin Fear & Greed Index to identify patterns in profitability, trading activity, and trader behavior.

The project was completed using Python in Google Colab with data analysis and visualization libraries.

---

## Objective

The primary objectives of this project are to:

- Analyze historical cryptocurrency trading data.
- Integrate the Bitcoin Fear & Greed Index with trading records.
- Compare trading performance across different market sentiment conditions.
- Study changes in trader behavior during Fear and Greed markets.
- Segment traders based on trading characteristics.
- Generate actionable trading insights supported by data.

---

## Dataset

### 1. Historical Trader Data

The trading dataset contains information such as:

- Account ID
- Coin
- Execution Price
- Trade Size (Tokens & USD)
- Buy/Sell Direction
- Closed Profit & Loss (PnL)
- Fees
- Transaction Details
- Timestamp

### 2. Bitcoin Fear & Greed Index

The sentiment dataset includes:

- Date
- Fear & Greed Score
- Sentiment Classification

Examples of sentiment categories:

- Extreme Fear
- Fear
- Neutral
- Greed
- Extreme Greed

---

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## Project Workflow

### 1. Data Preparation

- Loaded both datasets
- Checked missing values
- Removed duplicate records
- Converted timestamps into datetime format
- Extracted trading dates
- Merged trading data with the Fear & Greed Index

---

### 2. Feature Engineering

Created additional features including:

- Daily Profit & Loss
- Win/Loss indicator
- Daily Win Rate
- Average Trade Size
- Number of Trades per Day
- Long/Short Ratio (using Open Long and Open Short positions)

---

### 3. Exploratory Data Analysis

The following analyses were performed:

- Average Daily PnL by Market Sentiment
- Average Win Rate by Market Sentiment
- Average Number of Trades
- Average Trade Size
- Correlation Analysis
- Profit Distribution across Market Sentiments

---

### 4. Trader Segmentation

Traders were categorized into different groups:

- Frequent vs Infrequent Traders
- High Profit vs Low Profit Traders
- High Win Rate vs Low Win Rate Traders

---

## Key Findings

- Average daily profitability was highest during Extreme Fear market conditions.
- Extreme Greed recorded the highest average win rate.
- Trading activity increased significantly during Fear-based markets.
- Larger average trade sizes were observed during Neutral and Fear periods.
- Profitability varied considerably across all market sentiment categories.

---

## Actionable Strategies

### Strategy 1

Increase trading opportunities selectively during Fear and Extreme Fear markets while maintaining proper risk management, as these periods showed higher average profitability.

### Strategy 2

During Greed and Extreme Greed markets, prioritize high-quality trade setups rather than increasing trade frequency, since higher win rates did not necessarily produce higher overall profits.

---

## Limitations

- The dataset does not contain leverage information; therefore, leverage analysis could not be performed.
- Portfolio equity data was unavailable, making drawdown analysis impossible.
- Results are based on historical data and may not generalize to future market conditions.

---

## Conclusion

This project demonstrates that market sentiment influences trading behavior and profitability. Traders showed noticeable differences in profit, trading activity, and position sizes across Fear and Greed market conditions. While sentiment provides useful context, it should be combined with disciplined risk management and trading strategies for better decision-making.

---

## Repository Structure

```
Crypto-Trading-Analysis/
│
├── Crypto_Trading_Analysis.ipynb
├── historical_data.csv
├── fear_greed_index.csv
├── README.md
└── images/
    ├── avg_pnl.png
    ├── win_rate.png
    ├── trade_frequency.png
    ├── trade_size.png
    ├── correlation_heatmap.png
    └── pnl_distribution.png
```

---

## Author

**Akshita Gupta**

Data Analysis Internship Assignment
