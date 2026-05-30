# Comparative Study: Institutional vs. Retail Trading Strategies

## Overview

This project conducts a systematic comparison between two distinct trading approaches:
- **Institutional Algorithmic Trading**: Quantitative mean reversion strategy with volatility-adjusted execution
- **Retail Trading Strategy**: Fair Value Gap (FVG) pattern recognition approach

Both strategies are empirically validated using historical data on the S&P 500 ($SPY$) with rigorous statistical testing to determine whether the signals hold genuine predictive power or are products of market noise and hindsight bias.

## Project Goals

1. **Bridge the gap** between institutional quantitative methods and retail price action analysis
2. **Validate strategy logic** through statistical regression analysis and permutation testing
3. **Assess economic utility** by backtesting both approaches over multi-year periods
4. **Compare performance** across different market conditions and trading regimes

## Project Structure

```
├── Institutional_Algorithmic_Trading_Strategy-RMCT-Assignment.ipynb
│   └── Mean Reversion Strategy: z-score signals, volatility adjustments, and regression validation
├── Retail_Trading_Strategy_FVG-RMCT-Assignment.ipynb
│   └── FVG Strategy: Pattern detection, statistical validation, and backtest analysis
└── README.md
```

## Quick Start

### Requirements
- Python 3.x
- `yfinance` - Historical market data
- `pandas`, `numpy` - Data manipulation
- `statsmodels` - Statistical analysis
- `matplotlib` - Visualization

### Running the Notebooks

Both notebooks are designed to run on Google Colab (open-in-colab buttons included) or locally with Jupyter.

**For local execution:**
```bash
pip install yfinance pandas numpy statsmodels matplotlib
jupyter notebook
```

## Key Features

### Institutional Strategy Notebook
- Mean reversion signal generation using statistical z-scores
- Volatility-based position sizing (ATR)
- OLS regression analysis for signal validation
- Monte Carlo permutation testing (100,000 simulations)
- 5-year backtest on daily SPY data

### Retail Strategy Notebook
- Algorithmic Fair Value Gap detection
- Bullish and bearish gap identification
- Statistical significance testing
- Monte Carlo permutation testing (100,000 simulations)
- 5-year backtest on daily SPY data

## Methodology

Both strategies employ the same rigorous validation framework:
1. **Regression Analysis** - Measure correlation between signals and forward returns
2. **Residual Testing** - Validate linear regression assumptions (linearity, homoscedasticity, normality)
3. **Permutation Testing** - Test statistical significance against a null distribution
4. **Backtest Analysis** - Evaluate real-world economic performance vs. benchmark

## Data Source

- **Ticker**: S&P 500 ($SPY$)
- **Interval**: Daily OHLCV data
- **Historical Period**: Maximum available (approximately 10,000 trading days)

## Notes

- Backtests are for educational and research purposes
- Past performance does not guarantee future results
- No trading recommendations are implied
- Each notebook is self-contained and can be run independently