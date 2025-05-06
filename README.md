# Quant-Projects
This repository contains prominent projects related to quantative trading, algorithmic trading, stock market analysis and much more.

Author- Shuchi Chitrakar

import numpy as np

# Simulated daily returns of a stock (e.g., from model or historical data)
daily_returns = np.array([0.001, 0.002, -0.001, 0.003, -0.002, 0.0005, 0.0025])

# Risk-free rate (e.g., daily return of T-bill, assume 0.0001 or 0.01%)
risk_free_rate = 0.0001

# Excess returns
excess_returns = daily_returns - risk_free_rate

# Sharpe Ratio = Mean(Excess Return) / Std(Excess Return)
sharpe_ratio = np.mean(excess_returns) / np.std(excess_returns)

print(f"Sharpe Ratio: {sharpe_ratio:.2f}")
