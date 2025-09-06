# Systematic-Investing-in-European-Equities-Using-ML

A Systematic Investing Approach for European Equities

Author: Michaïl Maréchal
Supervisor: Dr. Nicholas Danks, Trinity College Dublin
Degree: MSc Business Analytics (Top Dissertation in Class)

📌 Project Overview

This project investigates how machine learning models can enhance equity selection and portfolio construction for European equities. It evaluates whether imposing constraints on mean-variance portfolio weights improves risk-adjusted performance when expected returns are proxied using machine learning–predicted probabilities of outperformance.

The study uses the historical constituents of the Stoxx 50 Index with weekly data from 2004–2025.

⚙️ Methodology

Models: Lasso, Ridge, Elastic Net, Random Forest, LightGBM

Ensembles: Combined forecasts to improve robustness

Forecast Target: Binary classification of weekly stock outperformance vs. median return

Portfolio Construction:

Equal- and value-weighted benchmarks

Mean-variance optimization (with and without constraints)

Constraints tested from 20–30% per asset

Validation: Purged K-Fold with embargo (per López de Prado, 2018)

Risk Assessment: Exposure to Fama-French 5 factors

📊 Key Findings

Constrained mean-variance portfolios (20–28% range) achieved superior risk-adjusted returns.

A 30% constrained mean-variance portfolio nearly doubled benchmark Sharpe Ratios while reducing maximum drawdowns.

Machine learning signals performed best during slowdowns and recessions, serving as a hedge during market stress.

Macroeconomic indicators (term spreads, credit spreads, volatility) were found to be significant drivers, except in Random Forest models.

🛠 Tech Stack

Languages & Libraries: Python, scikit-learn, LightGBM, Optuna, pandas, NumPy

Data Sources: Bloomberg Terminal, ECB Data, OECD Data, Kenneth French Data Library, FRED

Analytics: Portfolio optimization, Fama-French regressions, SHAP feature importance

📈 Results Visualization

Performance comparison: ML-based vs. benchmarks

Risk-adjusted metrics: Sharpe Ratio, Adjusted Sharpe Ratio, Maximum Drawdown

Factor exposures across economic cycles

SHAP plots for feature importance

📜 Citation

If referencing this work, please cite as:
Michaïl Maréchal (2025). Machine Learning for Stock Selection and Portfolio Construction: A Systematic Investing Approach for European Equities. MSc Business Analytics Dissertation, Trinity College Dublin. Supervised by Dr. Nicholas Danks.
