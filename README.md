
This project applies robust GARCH modelling techniques to study and forecast the volatility of stock returns.  
It focuses on both model estimation and risk quantification through Value-at-Risk (VaR) simulations and backtesting.

## Overview

The main objectives of the project are:
- **Modeling volatility** using different GARCH specifications:
  - Standard GARCH model (non-robust, no leverage)
  - Robust GARCH model without leverage
  - Robust GARCH model with leverage
- **Visualizing volatility dynamics** with News Impact Curves (NICs) and filtered conditional volatilities.
- **Testing statistically** whether robust filtering and leverage effects are significant.
- **Forecasting risk** through Monte Carlo simulation of future returns.
- **Computing Value-at-Risk (VaR)** for 1-day, 5-day, and 20-day ahead horizons under different models.
- **Backtesting** the accuracy of VaR forecasts to validate the model performance.

## Data

The project uses daily return data for four stocks:
- Johnson & Johnson (JNJ)
- Merck (MRK)
- Pfizer (PFE)
- Coca-Cola (KO)

The data was pre-processed to center returns around zero and adjust for stability in estimation.

## Methods

- **Robust GARCH modeling** to capture heavy tails and asymmetric volatility behavior.
- **Maximum Likelihood Estimation (MLE)** for parameter estimation.
- **Wald tests** for detecting significance of the leverage effect and robustness need.
- **Monte Carlo simulation** to simulate future returns and compute the distribution of returns.
- **Value-at-Risk (VaR)** calculations at 1%, 5%, and 10% confidence levels.
- **Backtesting** using rolling-window techniques to evaluate VaR forecasts.

