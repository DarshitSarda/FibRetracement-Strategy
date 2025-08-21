Unexpected Move Concept (UMC) — Automated Stock Screening & Fibonacci Strategy

This project automates the identification of strong bullish streaks across hundreds of NSE-listed stocks. Using Yahoo Finance APIs, the script fetches historical price data and analyzes consecutive green candles to detect “unexpected moves” (≥13–14% rallies from low to high). Once such moves are identified, the system automatically records the starting low (minimum of the breakout candle’s low or the previous candle’s low) and the rally’s peak, then constructs a Fibonacci retracement chart.

The key trading insight is that when price retraces to the 0.786 Fibonacci level, it forms a high-probability buying zone. The strategy defines:

Entry: Near 0.786 retracement.

Stop Loss (SL): The 1.0 retracement level (low of the breakout).

Target: 1.5× the risk (distance between 0.786 and 1.0 levels).

This forms a 1:1.5 risk-reward setup, historically yielding a 70–75% success rate. The project automates screening, detection, and signal generation across multiple equities, saving manual effort and producing results in a consolidated Excel output for traders and analysts.

The strategy works well for the stocks in the FnO segment of the Indian Stock Market
