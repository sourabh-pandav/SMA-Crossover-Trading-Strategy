# SMA-Crossover-Trading-Strategy
# SMA Crossover Trading Strategy with Risk-Reward Analysis


## Overview

The SMA Crossover Trading Strategy with Risk-Reward Analysis is a Python-based project designed to facilitate stock trading decision-making by implementing a Simple Moving Average (SMA) crossover strategy. It focuses on two popular stocks, NVIDIA (NVDA) and AMD (AMD), for the specified time period (2020-2023). This README provides an in-depth understanding of the project's features, installation steps, usage guidelines, and more.

## Features

### 1. Historical Stock Data Retrieval

The project utilizes the Yahoo Finance API through the `yfinance` library to fetch historical stock data for NVIDIA (NVDA) and AMD (AMD) from January 2020 to October 2023.

### 2. SMA Calculation

The script calculates two Simple Moving Averages (SMAs) for each stock:
- 50-day SMA
- 200-day SMA

These SMAs serve as key indicators for generating trading signals.

### 3. SMA Crossover Signals

Based on the calculated SMAs, the project generates buy and sell signals for each stock. The signals are generated as follows:
- When the 50-day SMA crosses above the 200-day SMA, a "Buy" signal is generated.
- When the 50-day SMA crosses below the 200-day SMA, a "Sell" signal is generated.

### 4. Position Management

The project manages positions and trade-related variables, including:
- Initial balance (starting balance) set at $100,000.
- Position size adjustments based on trade reversals.
- Lists to store trade details, such as trade type, timestamp, and price.

### 5. Risk-Reward Analysis

Risk-reward analysis is performed to evaluate the profitability of each trade opportunity. The project implements a 2:1 risk-reward ratio, where the potential reward is twice the potential risk.

### 6. Trade Visualization

The project visualizes trading signals using the `matplotlib` library. It provides graphical representations of stock prices, SMAs, buy signals (green triangles), and sell signals (red triangles) to aid in decision-making.

### 7. Trade Statistics

Key trading statistics are calculated, including:
- Initial balance
- Final balance after executing trades
- Average returns on trades
- Win ratios for successful trades

