# AnalystLab-Week-6---Chidozie-Iheme
# AAPL Historical Stock Analysis — Advanced Python for Data Analysis

**Week 6 Project | AnalystLab Africa Internship, Batch B (June–August 2026)**

An end-to-end analysis of 5 years of Apple Inc. (AAPL) historical stock data, applying advanced Pandas techniques, time-series analysis, and feature engineering to uncover trends in price movement, volatility, and returns.

## 📌 Overview

This project takes raw daily OHLCV (Open, High, Low, Close, Volume) stock data for AAPL and transforms it into a structured analysis covering data cleaning, trend analysis, rolling metrics, and risk measures — the kind of workflow used in real-world financial and business analytics.

## 📊 Dataset

- **Source:** Yahoo Finance — Apple Inc. (AAPL) Historical Data
- **Range:** 5 years, daily frequency
- **Fields:** Date, Open, High, Low, Close, Adjusted Close, Volume
- **Retrieval method:** Pulled programmatically using the `yfinance` Python library (see `Section 1b` in the notebook)

## 🛠️ Tools & Libraries

| Tool | Purpose |
|---|---|
| Python | Core analysis language |
| Pandas | Data cleaning, transformation, aggregation |
| NumPy | Numerical computation |
| Matplotlib | Data visualization |
| yfinance | Programmatic data retrieval from Yahoo Finance |
| Jupyter / Google Colab | Notebook environment |

## 🔍 What This Project Covers

**1. Data Transformation with Pandas**
- Cleaning and type correction, missing-value handling, duplicate removal
- Filtering, sorting, grouping/aggregation (yearly summary stats)
- Calculated columns and restructuring via resampling (monthly OHLC)

**2. Time-Series Analysis**
- Date/time feature extraction (year, month, weekday)
- Daily percentage change in closing price
- Rolling averages — 7-day, 30-day, and 90-day
- Monthly performance aggregation

**3. Feature Engineering**
- `Price_Change` — day-over-day absolute price change
- `Daily_Return_%` — day-over-day percentage change
- `MA_7 / MA_30 / MA_90` — short-, medium-, and long-term moving averages
- `Monthly_Return_%` — month-end to month-end percentage return
- `Volatility_30D_Annualized` — 30-day rolling volatility, annualized
- `Cumulative_Return_%` — total return since the start of the dataset

## 📈 Visualizations

1. Stock Closing Price Trend (5-year line chart)
2. Trading Volume Trend
3. Moving Average Analysis (Close price with 7/30/90-day MAs overlaid)
4. Monthly Returns Analysis (color-coded: green = positive, red = negative)
5. 30-Day Rolling Annualized Volatility

## 💡 Key Insights

- AAPL delivered strong multi-year growth, but the path was far from linear — a sharp 2022 drawdown (tied to broad market rate-hike pressure) was followed by a strong 2023–2024 recovery, then a more volatile 2025–2026 stretch.
- The two clearest volatility spikes align with real market events: the **January 2022 rate-hike selloff** and the **April 2025 tariff shock**, both of which show up as high-volume, high-volatility periods in the data.
- Moving-average crossovers lag price turns rather than predicting them — useful context for framing trend-following approaches as reactive, not predictive.

*(Full findings and supporting numbers are in Section 8 of the notebook.)*

## 📂 Repository Structure

```
├── Week6_AAPL_Advanced_Python_Analysis.ipynb   # Main analysis notebook
├── AAPL.csv                                     # Historical dataset (5-year daily data)
├── AAPL_Insight_Summary.docx                    # 2-page written insight summary
└── README.md                                    # Project overview (this file)
```

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/<your-repo>.git
   ```
2. Open `Week6_AAPL_Advanced_Python_Analysis.ipynb` in Jupyter or upload it to [Google Colab](https://colab.research.google.com).
3. Run all cells (`Runtime → Run all` in Colab). The notebook either reads from the included `AAPL.csv` or pulls fresh data directly via `yfinance` (Section 1b).

## 🎓 About This Project

This is a Week 6 deliverable for the **AnalystLab Africa Internship, Batch B**, focused on building advanced Python and data analysis skills using real-world financial data.

**Author:** Chidozie
**Program:** AnalystLab Africa Internship — Batch B (June–August 2026)
**Connect:** [LinkedIn](https://linkedin.com) · [Portfolio](https://your-portfolio-link.com)
