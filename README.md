# 0004_SP500TR_analysis
# S&P 500 Historical Return & Volatility Analysis
🔗 **Live Demo / Web Report:** [S&P 500 Analysis Webpage](https://tmanganiello-code.github.io/0004_SP500TR_analysis/)
A simple Python-based exploratory data analysis of the S&P 500 index using weekly adjusted closing prices from 1993 to present.

## 📌 Project Overview
This project analyzes the historical performance, statistical distribution, and annual yields of the S&P 500 index. The objective is to calculate basic return metrics, quantify weekly volatility, estimate confidence intervals for average returns, and review year-over-year performance.

---

## 📊 Dataset & Cleaning
- **Source Data**: `sp500_weekly_adjusted.csv` (contains weekly Open, High, Low, Close, Adjusted Close, and Volume).
- **Data Preprocessing**:
  - Parsed dates and sorted entries in chronological order.
  - Imputed missing records using Forward Fill (`ffill`) to prevent lookahead bias.
  - Calculated percentage changes on Adjusted Close prices to account for dividends and stock splits.

---

## 📈 Key Statistical Findings

### Weekly Returns Performance
- **Mean Weekly Return**: ~`0.23%`
- **Median Weekly Return**: ~`0.35%`
- **Standard Deviation (Volatility)**: ~`2.36%`
- **Standard Error of the Mean**: ~`0.056%`
- **95% Confidence Interval for Mean Return**: `[0.12%, 0.34%]`

> **Interpretation**: Over the analyzed timeframe, the S&P 500 generated an average positive weekly return of ~0.23%. We can be 95% confident that the true population mean weekly return lies between 0.12% and 0.34%.

---

## 📅 Annual Performance Summary
Annual returns are computed by resampling adjusted prices to year-end periods (`YE`) and measuring year-over-year percentage variations.

- **Historical Range**: 1993 – Present
- **Highest Annual Gain**: `+38.05%` (1995)
- **Largest Annual Loss**: `-32.63%` (2008)

---

## 🛠️ Repository Structure

```text
├── sp500_analysis.ipynb       # Jupyter Notebook containing code and analyses
├── sp500_weekly_adjusted.csv  # Raw weekly historical dataset
└── README.md                  # Project documentation
```

---

## 🚀 How to Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/sp500-return-analysis.git
   cd sp500-return-analysis
   ```

2. **Install dependencies**:
   ```bash
   pip install pandas
   ```

3. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook sp500_analysis.ipynb
   ```

---

## 💡 Technologies Used
- **Python 3.x**
- **Pandas** (Data manipulation and time-series resampling)
