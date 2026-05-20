# 🏦 Treasury ALM Quantitative Dashboard

**Portfolio Project for U.S. Bank — Quantitative Model Analyst (Treasury)**

A 6-tab interactive Streamlit dashboard demonstrating balance sheet forecasting, NII sensitivity analysis, interest rate risk measurement, deposit behavior modeling, model validation, and macroeconomic scenario generation.

## 🎯 Skills Matrix — JD Requirement Mapping

| JD Requirement | Where Demonstrated | Dashboard Tab |
|---|---|---|
| Developing advanced statistical models for balance sheet forecasting | ARIMAX(2,1,1) with macro exogenous variables | Tab 1: Balance Sheet Forecast |
| Interest rate risk analysis | EVE + NII sensitivity under 6 Basel IRRBB scenarios | Tab 3: IRR Dashboard |
| Macroeconomic forecasting model frameworks | VAR(2) multi-variable scenario engine | Tab 6: Macro Scenarios |
| Regression techniques, parametric/non-parametric algorithms | Panel regression for NMD deposit decay modeling | Tab 4: Deposit Behavior |
| Time series techniques | ARIMA, ARIMAX, seasonal decomposition, VAR | Tab 1 + Tab 6 |
| Model validation tests/methodologies | Walk-forward backtesting, residual diagnostics, RMSE/MAE | Tab 5: Model Validation |
| Estimating, testing, documenting, implementing, maintaining | Full model lifecycle with methodology documentation | All tabs + docs/ |
| Communicating modeling approaches and results | Interactive visualizations, method boxes, stakeholder-ready layout | All tabs |
| Knowledge of regulatory rules | Basel IRRBB implementation, SR 11-7 model governance | Tab 3 + docs/ |

## 🚀 Live Demo

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://usbank-treasury-alm-quant-dashboard.streamlit.app)

## 📦 Quick Start

```bash
git clone https://github.com/YOUR_USERNAME/usbank-treasury-alm-quant-dashboard.git
cd usbank-treasury-alm-quant-dashboard
pip install -r requirements.txt
streamlit run app.py
```

## 🛠 Tech Stack

- **Python** — Primary language
- **Streamlit** — Dashboard framework
- **Plotly** — Interactive visualizations
- **Pandas / NumPy** — Data manipulation and synthetic data generation
- **Statistical Methods** — ARIMAX, VAR, OLS regression, walk-forward validation

## 📊 Dashboard Tabs

### 1. Balance Sheet Forecast
ARIMAX model forecasting loan balances, deposit balances, securities, and borrowings with GDP, unemployment, Fed funds rate as exogenous variables.

### 2. NII Sensitivity
Interactive rate shock slider (−300 to +300 bps) showing baseline vs. stressed NII projections with annual impact calculation.

### 3. IRR Dashboard
Basel IRRBB six prescribed scenarios with EVE and NII sensitivity, limit monitoring, and status indicators.

### 4. Deposit Behavior
Non-maturity deposit decay rate regression showing the non-linear relationship between rate spread and deposit runoff.

### 5. Model Validation
24-month walk-forward out-of-sample validation with 95% confidence intervals, RMSE/MAE metrics, and residual analysis.

### 6. Macro Scenarios
VAR(2) macroeconomic scenario engine showing GDP, unemployment, and Fed funds rate paths under baseline vs. severely adverse scenarios.

## 👤 Author

**Nitin Madagi**
- MS Financial Mathematics (Financial Risk Management Track) — University at Buffalo, SUNY
- [LinkedIn](https://www.linkedin.com/in/nitinmadagi)

---

*Built to demonstrate quantitative modeling capabilities for the U.S. Bank Corporate Treasury ALM Quantitative Finance group.*
