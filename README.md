# Huarizo

**No-code trading bot for Alpaca.** Build your own strategy from signals, test it on history, let it run.

> **Status:** in development · paper trading only · not yet open to the public

## What it does

- **Build strategies without code.** Combine signals such as moving averages, RSI, MACD and Bollinger Bands into entry and exit rules, with stop-loss, take-profit and position sizing.
- **Backtest on history.** See how a strategy would have behaved on historical market data: returns, drawdown, every trade on the chart, compared with buy & hold.
- **Run it on your own account.** Connect your Alpaca account via OAuth and let Huarizo evaluate your rules and place the orders automatically. Paper trading first.

Example rule:

```
Entry rule – applies when all conditions hold
      RSI(14)  crosses above  30
  and Close    is above       SMA(200)
then  Buy 10% of equity · stop-loss 5%
```

## Status

- [x] Strategy engine and backtester
- [x] Web app with visual strategy editor, versioned strategies, backtest charts and user accounts
- [ ] Alpaca account connection (OAuth, paper accounts)
- [ ] Automated paper trading with risk limits and an emergency stop
- [ ] Live trading – only after Alpaca's review and approval, and after legal review

## Principles

- **Your rules, your decisions.** Users define their own strategies. Huarizo does not recommend strategies or give investment advice.
- **Your own broker account.** Orders are placed in the user's own Alpaca account. Huarizo never holds customer funds.
- **Paper before live.** Every strategy can be tested with paper money first. Live trading is a deliberate opt-in.
- **Built-in risk limits.** Maximum position size, daily loss limits and an emergency stop that closes everything.
- **Least privilege.** Only the permissions needed to trade and read market data are requested; access tokens are stored encrypted.
- **Transparent.** Every trade is logged with the rule that triggered it.

## Contact

Questions about Huarizo: huarizo.info@gmail.com

---

Huarizo is an independent project. It is not affiliated with, endorsed by or sponsored by Alpaca. "Alpaca" is a trademark of its respective owner and is used here only to describe compatibility.

Trading involves risk, including the loss of capital. Backtest results are simulations and do not guarantee future performance. Nothing here is investment advice.

© 2026 Huarizo. All rights reserved. The application source code is not public.
