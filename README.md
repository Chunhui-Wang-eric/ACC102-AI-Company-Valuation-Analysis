# ACC102_Track2_AI Company_Valuation_Analysis
A Python-based financial data analysis project comparing risk and return of public AI-related companies.
# What Drives AI Company Valuation? A Data-Based Comparison

## 1. Problem & User

This project explores what may drive the valuation of AI-related companies by comparing the risk and return of selected public AI-related firms.

The project is inspired by recent business discussions about the rapid valuation growth of private AI companies such as Anthropic and OpenAI. Since these companies are private and do not provide full public stock market data, this project uses listed AI-related companies as comparable examples.

The target users are beginner investors, business students, and accounting or finance students who want to understand why AI-related companies can receive high market valuations.

The main research question is:

**Do AI-related companies with higher growth also show higher risk, and what does this suggest about AI company valuation?**

---

## 2. Data

The project uses historical daily stock price data from Yahoo Finance, collected through the Python package `yfinance`.

### Data source

- Source: Yahoo Finance
- Access method: `yfinance`
- Access date: Please insert the date you ran the notebook
- Data period: 2022-01-01 to 2025-01-01
- Data frequency: Daily
- Key variable used: Closing stock price

### Companies analysed

| Ticker | Company |
|---|---|
| NVDA | Nvidia |
| MSFT | Microsoft |
| GOOGL | Alphabet / Google |
| META | Meta Platforms |

The cleaned dataset is saved in:

data/clean_ai_stock_prices.csv

The final risk-return summary is saved in:

data/final_risk_return_summary.csv

---

## 3. Methods

This project uses Python to collect, clean, transform, analyse, and visualise stock market data.

### The main Python steps are:

1. Define company tickers and the analysis period.
2. Download daily stock price data using yfinance.
3. Select closing prices for the four companies.
4. Inspect the data structure, columns, and missing values.
5. Clean the data using .dropna().
6. Save the cleaned dataset as a CSV file.
7. Calculate daily returns using .pct_change().
8. Calculate descriptive statistics, including average daily return and daily volatility.
9. Convert daily return and volatility into annualised return and annualised risk.
10. Create visualisations using matplotlib.
11. Build a simple risk-return ranking table.
12. Export the final summary table.

### The analysis follows this workflow:
Problem → Data → Cleaning → Analysis → Visualisation → Findings

---

## 4. Key Findings

The analysis produces several findings:

1. AI-related companies do not have the same risk-return profile.
2. Nvidia shows strong growth during the selected period, but it also has relatively high volatility.
3. Microsoft appears more stable compared with some other AI-related companies.
4. Higher growth potential in the AI sector may be associated with higher risk.
5. This helps explain why AI company valuations can rise quickly: investors may reward future growth expectations, even when uncertainty remains high.

Overall, the project suggests that AI company valuation is not only related to current performance. It is also influenced by market expectations about future growth.

---

## 5. How to Run

### Step 1: Download this repository

Download or clone this GitHub repository to your computer.

### Step 2: Install required packages

Install the required Python packages using:
pip install -r requirements.txt

The required packages are:
pandas
matplotlib
yfinance

### Step 3: Open the notebook

Open the Jupyter Notebook file:
ACC102_Track2_AI Company_Valuation_Analysis.ipynb

### Step 4: Run the notebook

Run all cells from top to bottom.

The notebook will:

* download stock price data,
* inspect and clean the data,
* calculate daily returns,
* calculate annualised return and annualised risk,
* create charts,
* save output files into the data/ and figures/ folders.

---

## 6. Product Link / Demo

### GitHub Repository：


### Demo Video：

The demo video explains the project problem, dataset, Python workflow, key outputs, and main findings.

---

## 7. Limitations & Next Steps

### Limitations

This project has several limitations:

a. It uses public stock price data from listed companies, not direct valuation data from private companies such as Anthropic or OpenAI.
b. Stock price performance is not exactly the same as company valuation.
c. The analysis does not include financial statement data such as revenue, profit, cash flow, or R&D spending.
d. The selected time period may affect the results.
e. The simple ranking system is for educational comparison only and should not be used as investment advice.

### Next steps

Future improvements could include:

* adding financial statement data,
* comparing revenue growth and profit margins,
* including R&D spending,
* adding more AI-related companies,
* using news sentiment analysis,
* building a simple interactive dashboard.

---

# Repository Structure

```text
ACC102-AI-Valuation-Analysis/
├── README.md
├── ACC102_Track2_AI_Company_Valuation_Analysis.ipynb
├── requirements.txt
├── data/
│   ├── clean_ai_stock_prices.csv
│   └── final_risk_return_summary.csv
└── figures/
    ├── price_trend.png
    ├── annual_return_comparison.png
    ├── risk_return.png
    └── normalised_price_index.png
```

---

# Disclaimer

This project is for educational purposes only. It is not financial advice or investment advice.
