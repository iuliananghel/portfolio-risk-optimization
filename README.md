# Covariance Matrix Estimation for Portfolio Optimization

This project evaluates classical and advanced covariance estimators (SCM, Ledoit-Wolf Shrinkage, and Factor-based models) in a high-dimensional equity environment. 

## Overview
- **Objective:** Compare out-of-sample portfolio risk and stability using 100 Fama-French portfolios.
- **Key Techniques:** Shrinkage (Ledoit-Wolf), Factor Models, Global Minimum Variance (GMV) optimization.
- **Tech Stack:** Python (Pandas, Scipy, Sklearn, Statsmodels), LaTeX.

## Key Results
| Estimator     | Ann. Volatility (%) | Sharpe Ratio | Quarterly Turnover (%) |
|---------------|---------------------|--------------|------------------------|
| SCM           | 14.09               | 1.02         | 30.27                  |
| **Shrinkage** | **14.04** | **1.02** | **28.36** |
| Factor Model  | 14.13               | 1.01         | 30.58                  |

**Key Insight:** While long-only constraints act as a natural regularizer for risk, the **Shrinkage estimator** provides superior operational efficiency by significantly reducing turnover and transaction costs.

## Repository Structure
- `notebooks/`: Contains the full analysis and backtesting engine.
- `paper/`: Contains the formal academic paper describing the methodology and results.

## Installation
```bash
pip install -r requirements.txt
