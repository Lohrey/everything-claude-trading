---
name: trading-guardrails
description: "Core principles, risk limits, agent orchestration and compliance rules for all trading work. Use when designing, backtesting, sizing, hedging or reviewing any trading strategy, trade or portfolio, or when routing work between the trading agents."
metadata:
  category: governance
---

# Trading Guardrails

Load this before any strategy, trade, allocation or backtest work. Detailed rule sets live in `references/`.

## Core Principles

1. **Risk-First** — Never skip risk assessment. Every strategy, trade and allocation needs explicit risk quantification before it proceeds.
2. **Data-Driven** — Every decision backed by quantitative evidence. Intuition is a hypothesis; data is the proof.
3. **Backtest Before Deploy** — No live trading without validated backtests. Walk-forward and out-of-sample testing are mandatory.
4. **Overfitting-Aware** — Guard against curve-fitting and data snooping. Track complexity, regularize, validate on held-out data.
5. **Execution-Conscious** — Account for slippage, fees and market impact.
6. **Regulatory-Compliant** — MiFID II, Dodd-Frank and position limits respected.

## Quality Standards

- Alpha signal: t-stat ≥ 2.0 before further development.
- Backtest: walk-forward with ≥ 3 out-of-sample windows.
- Net Sharpe > 1.0 after transaction costs.
- Max drawdown > 20% in backtest needs explicit risk-manager approval.
- Market data must pass validation (gaps, outliers, corporate actions) before use.
- Every strategy defines stop-loss, position sizing and drawdown limits.

## Agent Orchestration

Route to the most specialized agent. Gates: `risk-manager` approves every strategy/trade, `regulatory-compliance` validates before deployment, `backtesting-engineer` validates every systematic strategy.

| Flow | Chain |
|------|-------|
| Strategy development | quant-researcher → algo-strategist → backtesting-engineer → risk-manager |
| Options trade | derivatives-analyst → options-strategist → risk-manager → execution-specialist |
| Crypto analysis | crypto-defi-analyst → risk-manager → execution-specialist |
| Portfolio rebalance | portfolio-manager → risk-manager → execution-specialist |

## Reference Rules

Read the matching file when the task touches its area:

- `references/risk-limits.md` — position, leverage, drawdown, correlation limits
- `references/data-integrity.md` — point-in-time data, survivorship bias, validation
- `references/model-governance.md` — model validation, documentation, monitoring
- `references/regulatory-compliance.md` — MiFID II, Dodd-Frank, best execution
- `references/ethical-trading.md` — market abuse, manipulation, conflicts

## Disclaimer

Educational and research tooling, not investment advice. Real-money decisions stay with the user.
