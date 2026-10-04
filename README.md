# Security Analysis & Portfolio Management

A two stage quantitative portfolio management project that begins with mean-variance portfolio optimization in Excel and extends the framework into a dynamic Python based portfolio strategy.

## Project Overview

This project applies portfolio theory, risk analysis, and quantitative optimization to construct and evaluate multi-asset portfolios.

### Stage 1 — Excel Portfolio Optimization

The initial SAPM analysis was developed in Excel using historical market data. The analysis included:

- Historical daily returns
- Mean returns and covariance matrix
- Portfolio volatility
- Sharpe ratio
- Portfolio construction
- Excel Solver-based Sharpe ratio maximization
- Portfolio backtesting

The original portfolio consisted of Indus Towers, HAL, ICICI Bank, and Gold.

### Stage 2 — Python Dynamic Portfolio Extension

The Excel framework was extended into Python to create a more dynamic portfolio management strategy.

The Python implementation uses:

- NumPy and Pandas for quantitative analysis
- SciPy SLSQP for constrained portfolio optimization
- Rolling 126-day training windows
- 21-day rebalancing periods
- Transaction-cost modelling
- Dynamic portfolio rebalancing
- Static vs. dynamic strategy comparison
- Drawdown and performance analysis

The Python extension uses a broader six-asset universe and therefore is not a direct 1:1 conversion of the Excel portfolio.

## Methodology

The core optimization framework is based on mean-variance portfolio theory.

Portfolio volatility is calculated using the covariance matrix:

σₚ = √(wᵀΣw)

The portfolio Sharpe ratio is then used as the optimization objective:

Sharpe = (Rₚ − Rf) / σₚ

The Python implementation maximizes the Sharpe ratio subject to portfolio weight constraints using SciPy's SLSQP optimizer.

## Excel vs. Python

| Component | Excel | Python |
|---|---|---|
| Historical returns | ✓ | ✓ |
| Covariance matrix | ✓ | ✓ |
| Portfolio volatility | ✓ | ✓ |
| Sharpe ratio | ✓ | ✓ |
| Portfolio optimization | Excel Solver | SciPy SLSQP |
| Static optimization | ✓ | ✓ |
| Rolling optimization | — | ✓ |
| Walk-forward testing | — | ✓ |
| Periodic rebalancing | Limited | ✓ |
| Transaction costs | — | ✓ |
| Drawdown analysis | Limited | ✓ |
| Dynamic vs. static comparison | — | ✓ |

## Key Results

### Excel

- Equal-weight portfolio Sharpe ratio: **1.28**
- Optimized portfolio Sharpe ratio: **2.52**

### Python

The Python extension evaluates a dynamic rebalancing strategy against a static portfolio using rolling training and testing windows, while incorporating transaction costs and portfolio drawdown.



## Tools & Technologies

**Excel | Python | Pandas | NumPy | SciPy | Matplotlib | Quantitative Finance | Portfolio Optimization | Risk Analysis**
