# 0004_SP500TR_analysis
# 📈 S&P 500 Total Return (SP500TR) Weekly Analysis

A quantitative financial analysis of historical S&P 500 weekly adjusted data (SP500TR), evaluating distribution statistics, return performance, volatility metrics, and empirical risk bounds[cite: 1].

---

## 📌 Overview

This project processes historical weekly adjusted price data for the S&P 500 from **January 1993** to **September 2026**[cite: 1]. The analysis applies time-series data cleaning techniques, calculates percentage returns, and evaluates descriptive and risk-adjusted return metrics[cite: 1].

---

## 📊 Key Results & Statistical Highlights

Based on the weekly adjusted price data spanning **1993-01-25** to **2026-09-21**[cite: 1]:

* **Analysis Period**: January 25, 1993 – September 21, 2026[cite: 1]
* **Adjusted Close Range**: $\$24.05$ to $\$767.18$[cite: 1]
* **Mean Weekly Return**: `0.225%`[cite: 1]
* **Median Weekly Return**: `0.346%`[cite: 1]
* **Weekly Volatility (Standard Deviation)**: `2.356%`[cite: 1]
* **95% Empirical Interval ($2.5\%$ to $97.5\%$ Quantiles)**: `[-4.642%, +4.735%]`[cite: 1]
* **Weekly Sharpe Ratio Baseline**: `0.096`[cite: 1]

---

## 🛠 Pipeline & Methodology

The analysis follows a structured data analysis workflow[cite: 1]:

1. **Data Collection**:
   * Import raw historical weekly adjusted prices (`sp500_weekly_adjusted.csv`)[cite: 1].
2. **Data Cleaning & Preprocessing**:
   * Forward-fill missing values (`ffill()`)[cite: 1].
   * Convert timestamp values into standard `datetime` format[cite: 1].
   * Filter relevant columns (`Date`, `Adj Close`) and sort chronologically[cite: 1].
3. **Data Analysis & Modeling**:
   * Calculate percentage weekly returns: $\text{Return}_t = \left(\frac{\text{Price}_t - \text{Price}_{t-1}}{\text{Price}_{t-1}}\right) \times 100$[cite: 1].
   * Derive central tendency (Mean, Median) and volatility metrics (Standard Deviation)[cite: 1].
   * Extract actual $2.5\%$ and $97.5\%$ quantiles for non-parametric risk boundaries[cite: 1].
   * Compute standard Sharpe Ratio baseline[cite: 1].
4. **Data Storytelling**:
   * Output clear statistical metrics summarizing risk vs. return behavior[cite: 1].

---

## 🚀 Roadmap & Planned Enhancements

* **Annualized Metrics**: Compound Annual Growth Rate (CAGR) and Annualized Volatility[cite: 1].
* **Max Drawdown**: Historical peak-to-trough decline analysis[cite: 1].
* **Yearly Aggregations**: Year-by-year return breakdown and distribution comparison[cite: 1].

---

## 💻 Tech Stack & Requirements

* **Language**: Python 3.x[cite: 1]
* **Libraries**: `pandas`[cite: 1]
* **Environment**: Jupyter Notebook[cite: 1]

---

## 🏃 Quickstart

1. **Clone the repository**:
   ```bash
   git clone [https://github.com/tmanganiello-code/0004_SP500TR_analysis.git](https://github.com/tmanganiello-code/0004_SP500TR_analysis.git)
   cd 0004_SP500TR_analysis

---

## 💡 Technologies Used
- **Python 3.x**
- **Pandas** (Data manipulation and time-series resampling)
