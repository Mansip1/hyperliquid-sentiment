# Hyperliquid Trader Behavior vs Bitcoin Fear & Greed Index

## Methodology

Two datasets were used:

1. Bitcoin Fear & Greed Index (daily sentiment classification)
2. Hyperliquid historical trader-level transaction data

Steps performed:

- Verified dataset shape, missing values, and duplicates
- Converted timestamps to daily granularity
- Standardized column names for consistency
- Merged sentiment data with trader data using daily date alignment
- Created account-level daily metrics:
  - Daily PnL
  - Trade frequency
  - Average trade size
  - Win rate
  - Long/Short activity
- Segmented traders into:
  - Frequent vs Infrequent
  - Higher win-rate vs Lower win-rate

Primary comparison focused on Fear vs Greed market regimes.

---

## Key Insights

### 1. Traders are more aggressive during Fear periods

- Average trades per day:
  - Fear ≈ 105
  - Greed ≈ 77
- Average trade size:
  - Fear ≈ $8,530
  - Greed ≈ $5,955

This suggests that traders increase both frequency and position size during Fear conditions, likely reacting to heightened volatility.

---

### 2. Profitability does not significantly improve during Greed

- Average daily PnL:
  - Fear ≈ 5,185
  - Greed ≈ 4,144

Despite lower volatility on Greed days, profitability is not materially higher. This indicates that sentiment affects behavior more than performance quality.

---

### 3. Win rate remains relatively stable across regimes

- Fear ≈ 35.7%
- Greed ≈ 36.3%

The similarity in win rates suggests that sentiment does not significantly impact trade accuracy.

---

### 4. Risk exposure increases during Fear periods

PnL volatility is higher during Fear days, implying greater performance swings and risk concentration.

---

## Strategy Recommendations

### Strategy 1 — Risk Control During Fear Periods

Given increased trade frequency and larger position sizes during Fear:

- Limit daily trade count for lower win-rate traders
- Cap maximum position size during Fear regimes
- Implement stricter drawdown thresholds

This reduces volatility exposure during emotionally reactive periods.

---

### Strategy 2 — Selective Scaling During Greed Periods

Since win rate is stable but activity is lower:

- Allow higher win-rate traders to moderately increase position size
- Maintain conservative limits for lower-performing segments
- Emphasize trade quality over trade frequency

Scaling should depend on trader performance segment rather than sentiment alone.

---

## Conclusion

Market sentiment significantly influences trader behavior (frequency and size), but does not materially change win rate. Risk management rules tailored to sentiment regimes can improve performance stability and capital efficiency.