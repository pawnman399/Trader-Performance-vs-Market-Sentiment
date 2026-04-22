# Trader-Performance-vs-Market-Sentiment Analysis

## Overview

This project analyzes the relationship between market sentiment (Fear vs Greed) and trader behavior and performance using Hyperliquid trading data. The objective is to identify patterns in trading activity and derive actionable strategies that can improve trading decisions under different market conditions.

---

## Datasets

### 1. Bitcoin Market Sentiment Dataset

* Contains daily sentiment classification (Fear, Greed, etc.)
* Used to represent overall market conditions

### 2. Historical Trader Data (Hyperliquid)

* Trade-level dataset including:

  * Account
  * Trade size (USD)
  * Execution price
  * Trade side (BUY/SELL)
  * Closed PnL
  * Timestamp

---

## Methodology

### Data Preparation

* Cleaned and standardized column names
* Converted timestamps from milliseconds to datetime format
* Extracted date for daily-level analysis
* Merged trading data with sentiment dataset based on date

### Feature Engineering

* Created a binary win indicator (profit or loss per trade)
* Segmented trades into:

  * Low-size trades
  * High-size trades
* Derived key metrics:

  * Win rate
  * Trade frequency
  * Long vs Short ratio

---

## Analysis

The analysis focuses on understanding how trader behavior and performance change across different sentiment conditions:

* Performance comparison between Fear and Greed
* Trade activity analysis (number of trades)
* Behavioral patterns (BUY vs SELL distribution)
* Segment analysis based on trade size

---

## Key Insights

1. High-size trades underperform during Greed phases
   Large trades show lower win rates during Greed, indicating overconfidence and excessive risk-taking.

2. Trading activity is significantly higher during Fear
   The number of trades during Fear is much higher than during Greed, suggesting panic-driven or reactive behavior.

3. Sell-side dominance across sentiments
   SELL trades dominate in both Fear and Greed conditions, with stronger dominance during Greed, indicating profit-taking behavior.

4. Smaller trades perform better in Greed
   Low-size trades achieve higher win rates compared to high-size trades, suggesting disciplined strategies outperform aggressive ones.

5. Increased activity does not imply better performance
   Despite higher trading activity during Fear, performance does not improve proportionally, indicating inefficiency in trading decisions.

---

## Strategy Recommendations

1. Reduce position size during Greed phases
   Avoid large trades as they are associated with lower success rates.

2. Avoid overtrading during Fear
   High trading frequency does not necessarily lead to better outcomes.

3. Focus on disciplined, risk-managed strategies
   Smaller and controlled trades tend to perform better across market conditions.

4. Consider sell-side opportunities
   Profit-taking and short strategies can be effective during strong sentiment phases.

---

## Visualizations

The notebook includes the following visualizations:

* Win rate by sentiment and trade size
* Trade distribution across sentiment conditions
* Long vs short ratio by sentiment

---

## How to Run

1. Clone the repository
2. Install required libraries:
   pip install pandas matplotlib seaborn
3. Open the notebook:
   jupyter notebook
4. Run all cells

---

## Conclusion

Market sentiment has a significant impact on trader behavior and performance. The analysis shows that disciplined trading strategies and proper risk management consistently outperform aggressive trading, especially during Greed phases.

---

## Author

Pawan
Data Science Intern Candidate
