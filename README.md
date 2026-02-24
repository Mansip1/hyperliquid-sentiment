# Hyperliquid Trader Behavior vs Bitcoin Fear & Greed Index

## Objective

Analyze how Bitcoin market sentiment (Fear vs Greed) relates to trader behavior and performance on Hyperliquid.

The goal is to uncover patterns that can inform smarter trading strategies.

---

## Datasets Used

### 1️⃣ Bitcoin Market Sentiment (Fear & Greed Index)
Columns:
- timestamp
- value (index score)
- classification (Fear, Greed, Extreme Fear, etc.)
- date

### 2️⃣ Hyperliquid Historical Trader Data
Columns include:
- Account
- Coin
- Execution Price
- Size USD
- Side
- Closed PnL
- Timestamp IST
- Fee
- etc.

---

##  Setup Instructions

### 1. Clone the repository

```bash
git clone <your-repo-link>
cd hyperliquid-sentiment

