# Unexpected Move Concept (UMC) - Automated Stock Screening & Fibonacci Strategy

## Project Overview
**Unexpected Move Concept (UMC)** is an automated stock screening and trading strategy tool designed to identify strong bullish streaks across hundreds of NSE-listed stocks. This Python-based project uses Yahoo Finance APIs to fetch historical price data and analyze consecutive green candles, detecting “unexpected moves” (≥13–14% rallies from low to high).

Once a strong move is detected, the system records the starting low (minimum of the breakout candle’s low or the previous candle’s low) and the rally’s peak. A Fibonacci retracement chart is then constructed to identify high-probability buying zones.

## Key Trading Insights
The strategy leverages the Fibonacci retracement levels to define entry, stop loss, and target:

- **Entry:** Near 0.786 retracement level  
- **Stop Loss (SL):** 1.0 retracement level (low of the breakout)  
- **Target:** 1.5× the risk (distance between 0.786 and 1.0 levels)  

This forms a **1:1.5 risk-reward setup**, with a historical success rate of 70–75%.  

The system automates screening, detection, and signal generation across multiple equities, producing results in a consolidated Excel output, making it highly efficient for traders and analysts. The strategy is particularly suited for stocks in the FnO segment of the Indian Stock Market.

## Features
- Fetches historical daily data for hundreds of NSE-listed stocks using Yahoo Finance API  
- Detects consecutive green candles with ≥13–14% price movement  
- Automates identification of breakout lows and rally highs  
- Constructs Fibonacci retracement levels and identifies 0.786 retracement as a strong buying zone  
- Generates an Excel output with all detected bullish streaks and relevant details  
- Enables a 1:1.5 risk-reward trading setup  

## Technologies Used
- **Python 3**  
- **yfinance** for fetching historical stock data  
- **pandas** for data manipulation  
- **openpyxl / Excel** for output storage  

## Usage
1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd <repository_folder>
