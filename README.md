# ⚠️ Personal Research Experiment Financial Disclaimer & Liability Waiver

**This is not a Tool or Service.** This is a private, experimental sandbox, not intended for outside or public use, replication, or distribution. It is not a financial tool, software service, or product designed for public use.

**Not Financial Advice.** The author is not a licensed financial advisor, accountant, or broker. Nothing in this repository constitutes professional financial, investment, or legal advice.

**No Warranties.** This repository is provided "as-is" for display purposes only. The author makes no representations or warranties of any kind regarding the accuracy, completeness, or reliability of the data, code, or experimental models.

**Absolute Limitation of Liability.** Under no circumstances shall the author be liable for any claims, damages, or financial losses (direct or indirect) if you violate these terms and attempt to use, replicate, or rely on any part of this experiment.

---


<img width="1912" height="841" alt="desk" src="https://github.com/user-attachments/assets/a3fd668b-feaa-4874-b27a-dc4f9df150ad" />


---

# Pretty Desk First Draft

Keys save locally on your PC


Deploy from branch
-main
-root
-save

---

# 🌸 CaliQDesk — Pretty Desk (First Draft)

A single-page, window-based "desk operating system" for personal market research — canonical data, filing evidence, risk sizing, paper execution, and audit lineage, all in one scrollable workspace of draggable/resizable panels.

**🔗 Live desk:** [misoprettystacks.github.io/1stDRAFTPrettyDesk](https://misoprettystacks.github.io/1stDRAFTPrettyDesk/)

**🔑 Keys save locally on your PC** — nothing you enter is sent anywhere but the browser's own local storage and the data source you're querying directly.

## Operating rule

> Verified facts and model assumptions are kept separate. Forecasts are projections, not guarantees.

**Data contract:** a claim cannot become a verified fact merely because a model produces a number.

## What's on the desk

- **Mission Control** — live source status, registry entries, audit events, open approvals at a glance
- **Source Settings** — configure Finnhub and FRED API keys; test configured sources; see status for CoinGecko (direct), SEC EDGAR (direct link), Finnhub, and FRED
- **Paper Lab** — run real-data paper tests (asset, lookback window, fast/slow moving average) against CoinGecko historical price data; no simulated feed is substituted silently
- **Supervising Pretty Gate** — an approval protocol a strategy packet must clear before it's marked spawnable: evidence attached, validation/paper test passed, position sizing and tail checks passed, compliance and market-structure constraints passed, data lineage and source quality confirmed
- **Live Markets** — crypto, equities, and commodities feeds
- **Direct Sources / Filing** — add a direct source URL or paste source text and analyze it into a signal packet
- **Capital / Risk Engine** — enter total capital, risk per trade, entry, and stop to calculate exact position size, then send it on to the approval gate
- **Strategy Registry** — export the registry as JSON, or clear it
- **Canonical Data Model** — the shared schema every panel writes to (see below)
- **Audit & Memory** — clear the audit log or save a state snapshot
- **Research Ingestion** — drop in TXT, CSV, JSON, MD, HTML, PDF, or DOCX files to ingest and index
- **Analytics / P&L / Allocation / Drawdown** — portfolio value, P&L, capital in trades, drawdown, equity curve, allocation mix
- **Valuation / 180-Day / Fractional Mix** — longer-horizon valuation view
- **Agent Terminal / Source Health** — Brier score, win rate, Sharpe ratio
- **Compiled Security Universe** — tracked securities with a click-through dossier: price, public/model value, 24h and 180-day/IPO moves, projected earnings, known investors/funds, filings, and direct-source evidence
- **World Monitor** — full-width embed of an external global intelligence dashboard (pipelines, sanctions, weather, economic, waterways, outages, natural events, trade routes); opens directly if the destination blocks iframe embedding

## Canonical data model

| Object | Fields |
|---|---|
| **Thesis** | label, rationale, catalyst, horizon, invalidation |
| **Forecast** | base_case, bull_case, bear_case, confidence |
| **Strategy** | entry_rule, exit_rule, risk_rule, venue, status |
| **ApprovalPacket** | evidence, validation, risk, compliance, decision |
| **Position** | size, entry, stop, pnl, tax, status |
| **Source** | url, filing, timestamp, provenance, confidence |

## Getting started

1. Open the [live desk](https://misoprettystacks.github.io/1stDRAFTPrettyDesk/)
2. Add API keys under **Source Settings** if you want Finnhub or FRED data (CoinGecko and SEC EDGAR work without a key)
3. Run a paper test in the **Paper Lab**, size a position in the **Capital / Risk Engine**, and push it through the **Supervising Pretty Gate**
4. Save a state snapshot from **Audit & Memory** before you close the tab — this is local-only, so nothing persists on a server

## Tech notes

- Static, client-side site (`index.html`) deployed via GitHub Pages
- No backend — API keys and state live in your browser's local storage only
- Data sources: CoinGecko, SEC EDGAR, Finnhub, FRED (the latter two require your own free API key)

## Status

🚧 **First draft / active research experiment.** Panels, data sources, and the approval workflow are still evolving.

Made with 💖 by:
[@MisoPrettyStacks](https://github.com/MisoPrettyStacks)

@IGotGlitterOnMe on X
