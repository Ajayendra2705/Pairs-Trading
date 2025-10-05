# Pairs Trading (Statistical Arbitrage)

## Overview

Pairs trading is a market-neutral trading strategy widely used in quantitative finance and statistical arbitrage. The fundamental idea involves identifying two historically correlated or cointegrated securities whose price relationship tends to revert to a mean over time. When the price relationship deviates significantly, the strategy opens opposing positions — long one security and short the other — betting that the spread will revert back to its historical average.

---

## Key Concepts

- **Cointegration:** Unlike simple correlation, cointegration captures the long-term equilibrium between two non-stationary time series. Pairs trading relies on finding such pairs whose price spreads are mean-reverting.
  
- **Spread:** The difference or a weighted combination of two cointegrated asset prices. This spread is expected to oscillate around a stable mean.
  
- **Trading Signals:** Created by measuring deviations of the spread from its mean, often using z-scores. Entry signals trigger trades when the spread moves beyond a threshold, and exit signals close those trades as the spread normalizes.
  
- **Market-Neutral:** Because the strategy holds equal and opposite positions, it attempts to neutralize market risk and profit mainly from the relative price movements between selected pairs.

---

## Why Use Pairs Trading?

- Reduces exposure to broad market fluctuations
- Leverages statistical relationships to generate systematic trades
- Can be applied across different asset classes including stocks, commodities, and ETFs
- Employs mean reversion principles, which are robust across many markets

---

## Project Summary

This project implements an enhanced pairs trading statistical arbitrage strategy with features including:

- Automatic discovery of cointegrated pairs across a universe of stocks
- Spread modeling via cointegration and hedge ratios using econometric models
- Signal generation based on z-score thresholds for entry and exits
- A backtesting engine accounting for transaction costs and realistic trade execution
- Extensive visualizations for price series, spreads, trading signals, and strategy performance
- Scalability to multiple pairs for portfolio-level analysis

---

## How to Use

1. Download historical price data for multiple securities.
2. Compute cointegration statistics and select viable pairs.
3. Model spreads and generate z-score based trading signals.
4. Backtest your strategy over historical data with realistic assumptions.
5. Analyze results and refine parameters or pair selections.

