# QuantProcess_Trading_Model
Complete trading model created by Justin Gianfelice. Output and indicators received are based on stock ticker input and choice of trading strategy. Complete_Model_Python is the original code created in Python, Complete_Model_Pine is the model optimized in Pine to be directly implemented into trading facilitators such as TradingView.

Strategy logic
- Multi-strategy signals (MA, Mean Reversion, RSI, BB, Momentum)
- Regime-aware allocation with volatility targeting
- Portfolio construction via optimization

Assumptions
- Clean adjusted close data
- Stable regimes and correlations
- Monthly rebalance suffices

Costs
- Fixed commissions and simple slippage
- No market impact modeling

Benchmarks
- SPY buy-and-hold
- Equal-weight portfolio

Risk controls
- Volatility targeting
- Max drawdown monitoring
- Diversification via allocation rules

What Surprised Me:
- Sensitivity to rebalance timing
- Sample-size loss from multi-timeframe alignment

Next Improvements:
- Robust data validation and schema checks
- Event-aware risk throttles
- Impact-aware costs and liquidity constraints
- Strict anti-leakage ML pipelines
