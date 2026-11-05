# Buy/Sell Signals — TradingView Indicator

![Pine Script](https://img.shields.io/badge/Pine%20Script-v6-2962FF?logo=tradingview&logoColor=white) ![Status](https://img.shields.io/badge/Status-Prototype-64748B)

An experimental TradingView indicator that combines three signals before raising a buy or sell alert: **WaveTrend crosses**, **squeeze momentum**, and **Supertrend direction**.

## Signal logic

- A **buy** condition requires an oversold WaveTrend bullish cross, an upward Supertrend, and positive momentum.
- A **sell** condition requires an overbought WaveTrend bearish cross, a downward Supertrend, and negative momentum.
- The script defines TradingView `alertcondition` messages for both outcomes.

The implementation is in [`buy_sell_signals`](buy_sell_signals). Open it in the TradingView Pine Editor and add it to a chart to inspect the plots and alert conditions.

## Scope

This repository contains a **Pine Script indicator prototype**. Its earlier README described a possible Telegram bot workflow, but no Telegram integration or automated trading service is present in the code. Signals are experimental; the repository contains no backtest or performance claim.
