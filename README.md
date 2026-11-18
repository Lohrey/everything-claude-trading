<p align="center">
  <h1 align="center">Everything Claude Trading</h1>
  <p align="center"><strong>The complete trading & quant finance system for Claude Code</strong></p>
  <p align="center">18 specialized agents | 83 domain skills | 20 commands | Every trading discipline covered</p>
</p>

<p align="center">
  <a href="https://github.com/brainbytes-dev/everything-claude-trading/stargazers"><img src="https://img.shields.io/github/stars/brainbytes-dev/everything-claude-trading?style=for-the-badge&logo=github&color=yellow" alt="Stars"></a>
  <a href="https://github.com/brainbytes-dev/everything-claude-trading/network/members"><img src="https://img.shields.io/github/forks/brainbytes-dev/everything-claude-trading?style=for-the-badge&logo=github&color=blue" alt="Forks"></a>
  <a href="https://github.com/brainbytes-dev/everything-claude-trading/graphs/contributors"><img src="https://img.shields.io/github/contributors/brainbytes-dev/everything-claude-trading?style=for-the-badge&logo=github&color=green" alt="Contributors"></a>
  <a href="https://github.com/brainbytes-dev/everything-claude-trading/blob/main/LICENSE"><img src="https://img.shields.io/github/license/brainbytes-dev/everything-claude-trading?style=for-the-badge&color=purple" alt="License"></a>
  <a href="https://buymeacoffee.com/brainbytes"><img src="https://img.shields.io/badge/Buy%20Me%20a%20Coffee-brainbytes-orange?style=for-the-badge&logo=buy-me-a-coffee" alt="Buy Me a Coffee"></a>
</p>

---

> **From strategy ideation to live execution** -- 83 skills, 18 agents, and 20 slash commands that turn Claude Code into your quant trading co-pilot. Backtest, optimize, risk-check, and deploy -- all from your terminal.

---

## Quick Start

**Install in Claude Code** (inside a `claude` session):

```text
/plugin marketplace add Lohrey/everything-claude-trading
/plugin install everything-claude-trading@everything-claude-trading
```

Or from the shell:

```bash
claude plugin marketplace add Lohrey/everything-claude-trading
claude plugin install everything-claude-trading@everything-claude-trading
```

Restart Claude Code afterwards. Check with `/plugin` or `claude plugin details everything-claude-trading`.

**Start using it:**

```text
/strategy pairs trading on SPY/QQQ with 2-sigma entry
/backtest momentum factor strategy, 2015-2025, daily rebalance
/risk-report 60/40 equity/bond portfolio
/options-analysis iron condor on AAPL, 30 DTE, 1-sigma wings
/crypto-analysis ETH on-chain metrics vs price action
```

**Optional market data:** `mcp-configs/mcp-servers.json` lists MCP servers (Polygon, Alpha Vantage, …). Copy the ones you need into your own Claude Code MCP config and set the API keys there.

---


## Agents (18)

Subagents Claude delegates to (or call them explicitly: "use the risk-manager agent to ...").

| Agent | Role | Model |
|-------|------|-------|
| `algo-strategist` | Algorithmic trading strategist for systematic strategy design, rule-based systems, and execution algorithm development. Use for strategy design or systematic trading approaches | Opus |
| `backtesting-engineer` | Backtesting and simulation specialist for strategy validation, walk-forward optimization, Monte Carlo simulation, and overfitting prevention. Use when validating any trading strategy | Sonnet |
| `commodities-analyst` | Commodities analyst for futures curve analysis, seasonality patterns, supply/demand fundamentals, and commodity trading strategies. Use for commodity market analysis | Sonnet |
| `crypto-defi-analyst` | Crypto and DeFi analyst for on-chain analytics, protocol analysis, tokenomics evaluation, and yield strategy assessment. Use for cryptocurrency or DeFi analysis | Sonnet |
| `derivatives-analyst` | Derivatives specialist for options pricing, volatility surface construction, exotic option analysis, and structured product evaluation. Use for any derivatives-related analysis | Opus |
| `execution-specialist` | Trade execution specialist for order management, execution algorithm selection, transaction cost analysis, and smart order routing. Use for execution planning or TCA | Sonnet |
| `financial-data-scientist` | Financial data science specialist for feature engineering, ML model development, alternative data analysis, and quantitative research infrastructure. Use for ML-based trading research or data pipeline design | Opus |
| `fixed-income-analyst` | Fixed income specialist for bond analysis, yield curve modeling, duration/convexity management, and credit spread analysis. Use for bond portfolio or fixed income strategy work | Opus |
| `fx-strategist` | FX strategy specialist for currency analysis, carry trade design, macro-driven FX strategies, and hedging. Use for foreign exchange strategy or currency risk management | Opus |
| `market-microstructure` | Market microstructure specialist for order flow analysis, liquidity assessment, market making, and price discovery research. Use for execution optimization or market structure analysis | Opus |
| `options-strategist` | Options strategy specialist for spread design, volatility trading, hedging strategies, and options portfolio management. Use for options trade structuring or vol trading | Opus |
| `portfolio-manager` | Portfolio construction specialist for asset allocation, optimization, rebalancing, and performance attribution. Use for portfolio design or optimization tasks | Opus |
| `quant-researcher` | Quantitative researcher for alpha signal discovery, factor model construction, and systematic strategy research | Opus |
| `regulatory-compliance` | Trading compliance specialist for MiFID II, Dodd-Frank, position limits, best execution, and regulatory reporting. Use for compliance questions or regulatory risk assessment | Sonnet |
| `risk-manager` | Market risk manager for VaR calculation, stress testing, exposure analysis, and risk limit monitoring | Opus |
| `stat-arb-specialist` | Statistical arbitrage specialist for pairs trading, mean reversion strategies, cointegration analysis, and market-neutral portfolio construction. Use for stat-arb strategy development | Opus |
| `technical-analyst` | Technical analysis specialist for chart patterns, indicators, price action analysis, and support/resistance identification. Use for technical market analysis | Sonnet |
| `volatility-trader` | Volatility trading specialist for vol surface analysis, variance swaps, dispersion trading, and VIX strategies. Use for volatility-focused analysis or trading | Opus |

---

## Skills (83)

Skills load automatically when Claude sees a matching task — you don't call them by hand.

<details>
<summary><strong>Quant Methods (10)</strong></summary>

| Skill | Description |
|-------|-------------|
| `alpha-research` | Alpha signal discovery, testing, and evaluation |
| `bayesian-methods` | Bayesian inference for trading — prior selection, posterior updating, Bayesian portfolio optimization. Use for probabilistic trading analysis |
| `deep-learning-trading` | Deep learning for trading — LSTM, transformers, sequence models for price prediction |
| `factor-models` | Factor model construction and analysis — Fama-French, Carhart, Barra, custom factors |
| `kalman-filters` | Kalman filter applications in finance — dynamic beta estimation, pairs trading, state-space models. Use for dynamic parameter estimation |
| `ml-for-finance` | Machine learning for trading — supervised models, feature importance, cross-validation for time series |
| `regime-detection` | Market regime detection using HMM, Markov switching, and structural break methods |
| `reinforcement-learning-trading` | Reinforcement learning for trading — Q-learning, policy gradient, reward shaping for portfolio management |
| `signal-processing` | Signal processing for financial data — wavelets, Fourier analysis, noise filtering |
| `time-series-analysis` | Time series analysis for financial data — ARIMA, GARCH, cointegration, stationarity |

</details>

<details>
<summary><strong>Strategies (10)</strong></summary>

| Skill | Description |
|-------|-------------|
| `carry-strategies` | Carry strategies across asset classes — FX carry, yield curve carry, commodity roll |
| `event-driven` | Event-driven trading — earnings, M&A arb, index rebalancing, spin-offs |
| `market-making` | Market making strategies — bid-ask management, inventory risk, Avellaneda-Stoikov framework. Use for market-making strategy design |
| `mean-reversion` | Mean reversion strategies — Bollinger, Z-score, Ornstein-Uhlenbeck, and statistical approaches |
| `momentum-strategies` | Momentum strategy design — time-series, cross-sectional, and dual momentum approaches |
| `multi-asset-strategies` | Multi-asset systematic strategies — risk premia, CTA, global macro systematic |
| `pairs-trading` | Pairs trading methodology — cointegration, distance, copula methods |
| `relative-value` | Relative value strategies — cross-asset, capital structure, convertible arb |
| `stat-arb` | Statistical arbitrage — PCA-based, factor-neutral, sector-neutral portfolio construction. Use for stat-arb strategy development |
| `trend-following` | Trend-following strategies — CTA-style, moving averages, breakout systems, Turtle Trading |

</details>

<details>
<summary><strong>Risk Management (10)</strong></summary>

| Skill | Description |
|-------|-------------|
| `correlation-risk` | Regime-dependent correlation, diversification failure, dynamic correlation models, and correlation trading strategies |
| `counterparty-risk` | Margin, collateral, CVA/DVA/FVA, central clearing, netting, wrong-way risk, and credit support framework |
| `drawdown-management` | Max drawdown, recovery analysis, conditional drawdown at risk, stop-loss design, de-leveraging rules, and drawdown-based position sizing |
| `expected-shortfall` | Expected Shortfall calculation, advantages over VaR, regulatory adoption under FRTB, extreme value theory, and tail dependence modeling |
| `greeks-management` | Delta, gamma, vega, theta hedging and higher-order Greeks. Portfolio-level risk management, dynamic hedging, and rebalancing strategies |
| `liquidity-risk` | Bid-ask spreads, market impact, Amihud illiquidity, liquidity-adjusted VaR, and the illiquidity premium |
| `position-sizing` | Kelly criterion, optimal-f, fixed fractional, volatility targeting, risk parity position sizing, and practical implementation |
| `stress-testing` | Historical, hypothetical, and reverse stress testing. Scenario design, regulatory frameworks, crisis replay, and integration with risk management |
| `tail-risk-hedging` | Put spreads, VIX calls, tail risk parity, cost-effective crash protection, and systematic tail hedging programs |
| `var-models` | Parametric, historical simulation, and Monte Carlo VaR. Confidence levels, holding periods, backtesting, regulatory requirements, and known limitations |

</details>

<details>
<summary><strong>Derivatives (10)</strong></summary>

| Skill | Description |
|-------|-------------|
| `binomial-trees` | CRR model, multi-step trees, American options, early exercise boundary, calibration, and convergence to BSM |
| `black-scholes` | BSM derivation intuition, formula, put-call parity, Greeks, limitations, and extensions for dividends, American options, and implied volatility |
| `credit-derivatives` | Credit derivatives — CDS, CDO, credit indices, default correlation |
| `exotic-options` | Barriers, Asians, lookbacks, digitals, cliquets, autocallables, and quanto options. Pricing, hedging, and risk management |
| `hedging-strategies` | Derivatives hedging — delta-neutral, gamma scalping, vega hedging |
| `interest-rate-derivatives` | Swaps, swaptions, caps/floors, curve construction, OIS discounting, and multi-curve framework |
| `monte-carlo-pricing` | Random number generation, GBM simulation, path-dependent options, variance reduction, Longstaff-Schwartz for Americans, and convergence analysis |
| `structured-products` | Structured products — autocallables, reverse convertibles, capital protected |
| `vol-surfaces` | Implied vol surface, smile/skew, SVI parameterization, SABR model, sticky strike vs sticky delta, surface dynamics, and arbitrage constraints |
| `vol-trading` | Volatility trading — straddles, variance swaps, dispersion, VIX |

</details>

<details>
<summary><strong>Portfolio Management (8)</strong></summary>

| Skill | Description |
|-------|-------------|
| `alternative-allocations` | Alternative investment allocation — PE, VC, hedge funds, real assets in portfolio context |
| `benchmark-tracking` | Index tracking and replication strategies — full replication, sampling, and optimization |
| `black-litterman` | Black-Litterman model for portfolio allocation — combining equilibrium returns with investor views |
| `factor-investing` | Factor investing and smart beta strategies — systematic exposure to return drivers |
| `markowitz-optimization` | Mean-variance optimization and efficient frontier construction for portfolio allocation |
| `portfolio-attribution` | Decomposing portfolio returns into allocation, selection, and factor contributions |
| `rebalancing-strategies` | Portfolio rebalancing methodologies — when, how, and how much to trade |
| `risk-parity` | Risk parity and equal risk contribution portfolios — balancing risk, not capital |

</details>

<details>
<summary><strong>Execution (8)</strong></summary>

| Skill | Description |
|-------|-------------|
| `execution-algos` | Execution algorithms — TWAP, VWAP, IS, POV, Iceberg for optimal trade execution |
| `latency-optimization` | Low-latency trading infrastructure — co-location, FPGA, kernel bypass, network optimization |
| `market-microstructure-theory` | Market microstructure theory — limit order books, price discovery, bid-ask spread economics |
| `order-flow-analysis` | Order flow analysis — volume profile, footprint charts, delta for short-term price prediction |
| `performance-metrics` | Sharpe, Sortino, Calmar, Information Ratio, and comprehensive performance measurement |
| `smart-order-routing` | Smart order routing — dark pools, lit markets, internalization, and best execution |
| `tick-data-processing` | Tick data processing — cleaning, aggregation, bar construction from raw market data |
| `transaction-cost-analysis` | Transaction cost analysis (TCA) — slippage, market impact, benchmarks for measuring execution quality |

</details>

<details>
<summary><strong>Market Data (6)</strong></summary>

| Skill | Description |
|-------|-------------|
| `alternative-data` | Alternative data for trading — satellite, credit card, web traffic, app usage |
| `data-quality` | Financial data quality — survivorship bias, look-ahead bias, point-in-time |
| `data-vendors` | Financial data vendors — Bloomberg, Refinitiv, Polygon, Alpha Vantage |
| `feature-engineering` | Feature engineering for financial ML — lag features, rolling stats, ranks |
| `sentiment-analysis` | Sentiment analysis for trading — news NLP, social media, earnings calls |
| `web-scraping-finance` | Web scraping for financial data — SEC filings, earnings, macro releases |

</details>

<details>
<summary><strong>Crypto & DeFi (8)</strong></summary>

| Skill | Description |
|-------|-------------|
| `cross-chain-arbitrage` | Cross-Chain and CEX-DEX Arbitrage |
| `crypto-derivatives` | Crypto Derivatives |
| `defi-protocols` | DeFi Protocol Analysis |
| `mev-strategies` | MEV Strategies |
| `on-chain-analytics` | On-Chain Analytics |
| `stablecoin-analysis` | Stablecoin Analysis |
| `tokenomics` | Tokenomics Analysis |
| `yield-farming` | Yield Farming Analysis |

</details>

<details>
<summary><strong>Macro (6)</strong></summary>

| Skill | Description |
|-------|-------------|
| `central-bank-analysis` | Central Bank Analysis |
| `commodities-fundamentals` | Commodities Fundamental Analysis |
| `economic-indicators` | Economic Indicators for Trading |
| `fx-fundamentals` | FX Fundamental Analysis |
| `geopolitical-risk` | Geopolitical Risk for Trading |
| `yield-curve-analysis` | Yield Curve Analysis |

</details>

<details>
<summary><strong>Backtesting (6)</strong></summary>

| Skill | Description |
|-------|-------------|
| `live-trading-monitoring` | Live trading monitoring — drift detection, performance tracking, kill switches |
| `monte-carlo-simulation` | Monte Carlo Simulation for Strategy Evaluation |
| `overfitting-prevention` | Overfitting Prevention |
| `research-notebooks` | Research Notebook Best Practices |
| `strategy-evaluation` | Strategy Evaluation Framework |
| `walk-forward-optimization` | Walk-Forward Optimization |

</details>

<details>
<summary><strong>Governance (1)</strong></summary>

| Skill | Description |
|-------|-------------|
| `trading-guardrails` | Core principles, risk limits, agent orchestration and compliance rules for all trading work |

</details>

---

## Commands (20)

Plugin commands can also be called fully qualified, e.g. `/everything-claude-trading:backtest`.

| Command | Description |
|---------|-------------|
| `/alpha-decay` | Analyze signal half-life, alpha decay curves, and strategy capacity |
| `/backtest` | Backtest a trading strategy with rigorous validation and overfitting checks |
| `/correlation-check` | Analyze portfolio correlations, detect regime breaks, and identify hidden exposures |
| `/crypto-analysis` | Analyze crypto assets, DeFi protocols, on-chain metrics, and yield opportunities |
| `/data-pipeline` | Design and validate financial data ingestion, cleaning, and transformation pipelines |
| `/execution-plan` | Plan trade execution with optimal scheduling, venue selection, and TCA targets |
| `/factor-analysis` | Decompose portfolio returns by factor exposures and identify unintended bets |
| `/hedging-plan` | Design hedging strategies for portfolio risk or single-name exposure |
| `/macro-outlook` | Assess macroeconomic outlook and cross-asset market impact |
| `/market-regime` | Detect and classify the current market regime for strategy selection |
| `/options-analysis` | Analyze options strategies including pricing, Greeks, vol surfaces, and trade structuring |
| `/pairs-scan` | Scan for pairs trading opportunities using cointegration and mean-reversion analysis |
| `/portfolio-optimize` | Optimize portfolio allocation using mean-variance, risk parity, or factor-based methods |
| `/position-size` | Calculate optimal position sizes using Kelly criterion, volatility targeting, or risk budgeting |
| `/risk-report` | Generate a comprehensive portfolio risk report with VaR, stress tests, and exposure analysis |
| `/signal-research` | Research and validate alpha signals with statistical rigor |
| `/strategy` | Design a systematic trading strategy from concept to implementation |
| `/stress-test` | Run historical and hypothetical stress test scenarios on a portfolio |
| `/trade-review` | Review trading performance with execution quality analysis and lessons learned |
| `/vol-analysis` | Analyze volatility surfaces, term structure, and skew for trading opportunities |

---

## Rules (5)

| # | Rule | Description |
|---|------|-------------|
| 1 | **Risk Before Return** | Always quantify risk before evaluating return potential |
| 2 | **Backtest Before Deploy** | No strategy goes live without rigorous historical testing |
| 3 | **Overfitting Awareness** | Apply deflated Sharpe, cross-validation, and out-of-sample checks |
| 4 | **Data Integrity First** | Validate all data inputs; never trust raw feeds blindly |
| 5 | **Execution Realism** | Include transaction costs, slippage, and market impact in all analysis |

---

## Architecture

```
everything-claude-trading/
├── .claude-plugin/
│   ├── plugin.json          # plugin manifest
│   └── marketplace.json     # marketplace manifest (source: ./)
├── agents/                  # 18 subagents (<name>.md)
├── skills/                  # 83 skills, flat: skills/<name>/SKILL.md
│   └── trading-guardrails/  # core principles + rules (references/)
├── commands/                # 20 slash commands (<name>.md)
├── hooks/hooks.json         # SessionStart banner + non-blocking post-edit checks
├── scripts/hooks/           # hook scripts (Node)
├── rules/common/            # rule files (also bundled in trading-guardrails)
├── contexts/                # research / backtesting / live-trading modes
├── examples/                # sample project CLAUDE.md files
└── mcp-configs/             # optional market-data MCP servers
```

---

## Core Principles

| Principle | What It Means |
|-----------|---------------|
| **Risk-First** | Every analysis starts with risk quantification. No blind return-chasing. |
| **Data-Driven** | Decisions grounded in data, not narratives. Statistical significance required. |
| **Backtest Before Deploy** | Rigorous historical validation before any live deployment. |
| **Overfitting-Aware** | Multiple testing corrections, out-of-sample validation, deflated Sharpe ratios. |
| **Execution-Conscious** | Transaction costs, slippage, and market impact are never ignored. |
| **Regulatory-Compliant** | Adherence to MiFID II, Reg NMS, Dodd-Frank, and relevant trading regulations. |

---

## Multi-Agent Workflows

Complex trading tasks orchestrate multiple agents working together:

| Workflow | Agents Involved | Description |
|----------|----------------|-------------|
| **Strategy Development** | Quant Strategist -> Backtesting Engineer -> Risk Manager -> Performance Analyst | End-to-end strategy creation, validation, and analysis |
| **Risk Assessment** | Risk Manager -> Portfolio Optimizer -> Compliance Monitor | Comprehensive portfolio risk review with compliance checks |
| **Live Deployment** | Systematic Trader -> Execution Specialist -> Compliance Monitor -> Performance Analyst | Strategy deployment with execution optimization |
| **Derivatives Pricing** | Derivatives Analyst -> Volatility Trader -> Risk Manager | Complex derivatives pricing with vol and risk analysis |
| **Crypto Research** | Crypto Trader -> Data Engineer -> Quant Strategist | Digital asset research with on-chain data integration |
| **Macro Analysis** | Macro Strategist -> Fixed Income Quant -> Portfolio Optimizer | Global macro view with rates analysis and positioning |

---

## Contexts

Mode files in `contexts/` — not auto-loaded. Paste or reference one in your project's `CLAUDE.md` to switch Claude's behavior.

| Context | Purpose |
|---------|---------|
| `research` | Exploratory research: hypotheses, statistical rigor |
| `backtesting` | Backtest mode: bias checks, walk-forward discipline |
| `live-trading` | Live mode: risk-first, pre-trade checklist, audit trail |

---

## Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on adding new strategy skills, asset-class agents, and indicator skills.

## License

MIT License -- see [LICENSE](LICENSE) for details.

## Acknowledgments

- The quantitative finance open-source community
- Contributors who keep pushing the boundaries of AI-assisted trading
- Every quant who shared a paper, a backtest, or a hard-won lesson

---

<p align="center">
  <strong>Built for traders who build with AI.</strong>
</p>
<p align="center">
  <a href="https://buymeacoffee.com/brainbytes"><img src="https://img.shields.io/badge/Buy%20Me%20a%20Coffee-brainbytes-orange?style=for-the-badge&logo=buy-me-a-coffee" alt="Buy Me a Coffee"></a>
</p>
<p align="center">
  <sub>Made with conviction by <a href="https://github.com/brainbytes-dev">Brain Bytes</a></sub>
</p>
