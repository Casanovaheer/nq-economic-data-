# 📊 NQ Analyst — Nasdaq Pre-Market & Intraday Report System

> A professional-grade AI prompt system for analyzing Nasdaq (NQ/NAS100) trading conditions around the **10:00 AM EST** trading window.

---

## 🧠 What This Is

**NQ Analyst** is a structured prompt system that turns you into a **Senior Nasdaq Market Analyst with 30 years of experience** — powered by Claude (or any capable LLM).

You manually input market data. The AI does the professional analysis.

No live APIs. No black-box signals. Just institutional-grade reasoning applied to the data you provide.

---

## 🎯 Who This Is For

- Nasdaq (NQ / NAS100) traders who trade the **10:00 AM EST window**
- Traders who want to understand how **8:30 AM news events** affect their session
- Anyone who wants a structured, repeatable pre-market analysis framework

---

## ⚙️ How It Works

```
8:30 AM EST News Release
        ↓
Premarket Futures Reaction
        ↓
9:30 AM NYSE Cash Open
        ↓
10:00 AM EST — Your Trading Window
```

You provide the data. The system analyzes:

1. Whether the news is truly market-moving
2. How the actual print compared to forecast
3. The macro transmission chain (News → Fed → Rates → Bonds → Tech → NQ)
4. Whether the move is fresh, partially priced, or fully priced
5. What the 9:30–10:00 price action tells institutions
6. Your trade environment confidence and risk level

---

## 📋 Input Template

Fill this in before each session:

```
DATE:
Day:
Market: NASDAQ

NEWS EVENT:
News Name:
Release Time:
Impact: Red / Orange / Yellow

Previous:
Forecast:
Actual:

---

MARKET REACTION DATA:

Nasdaq Futures Movement (before 9:30): +/- ____ points
9:30 AM Open Price: _____
10:00 AM Price: _____
9:30–10:00 Movement: _____ points
Direction: Up / Down
Premarket High: _____
Premarket Low: _____
```

---

## 📤 Output Format

The system returns a structured **10-section professional report**:

| Section | What You Get |
|---|---|
| 1. News Quality | Market-moving / Moderate / Noise |
| 2. Actual vs Forecast | Surprise size, direction, institutional relevance |
| 3. Macro Transmission | Full chain: News → Fed → Rates → Bonds → NQ |
| 4. News Impact Remaining | HIGH / MEDIUM / LOW at 10 AM |
| 5. Premarket Pricing | FRESH / PARTIALLY PRICED / FULLY PRICED |
| 6. 9:30–10:00 Analysis | Acceptance / Overreaction / Failure / Ignored |
| 7. Market Condition | Trending / Choppy / Reversal Risk / Continuation |
| 8. Daily Bias | Bullish / Bearish / Neutral + Confidence |
| 9. No-Trade Filter | FOMC / CPI / NFP / Powell / Holiday check |
| 10. Final Report | Trade or Avoid + Risk Level + Reasoning |

### Final Report Format

```
═══════════════════════════════════
         MARKET REPORT
═══════════════════════════════════
News:
Impact:
Actual vs Forecast:
Macro Meaning:
Premarket Reaction:
9:30–10:00 Reaction:
News Impact Remaining:
Market Condition:
Nasdaq Bias:
Confidence:
Trade Environment:
Risk Level:

FINAL DECISION: Trade / Avoid
Reason:
═══════════════════════════════════
```

---

## 🚦 No-Trade Filter Events

The system automatically flags these as high-caution or avoid windows:

- 🔴 **FOMC Rate Decision**
- 🔴 **CPI / Core CPI**
- 🔴 **PCE**
- 🔴 **NFP (Non-Farm Payrolls)**
- 🔴 **Powell Speech**
- 🟡 **Bank Holidays**
- 🟡 **Half-Day Sessions**
- 🟡 **Low Liquidity Environments**

---

## 🧩 Analysis Framework (10 Sections)

### 1 — News Quality
Classifies the event: **Market-Moving (A)**, **Moderate (B)**, or **Noise (C)**

### 2 — Actual vs Forecast
Quantifies the surprise. Evaluates whether institutions would reprice based on the delta.

### 3 — Macro Transmission Chain
Traces the full path from data print to Nasdaq impact:
```
News Print → Fed Expectation → Rate Outlook → Bond Yields → Tech Multiples → NQ
```

### 4 — Remaining News Impact at 10 AM
**HIGH** — Big surprise, market still repricing  
**MEDIUM** — Initial move done, residual effect  
**LOW** — Fully absorbed, price action now leads

### 5 — Premarket Pricing Analysis
**FRESH** — Not yet priced in  
**PARTIALLY PRICED** — Some reaction occurred  
**FULLY PRICED** — Most of the move already happened

### 6 — 9:30–10:00 Cash Open Analysis
**A — Institutional Acceptance** → Confirm and continue  
**B — Overreaction** → Possible mean reversion  
**C — News Failure** → Price rejected the narrative  
**D — Market Ignoring News** → Other catalysts dominating

### 7 — Market Condition at 10 AM
Trending / Choppy / Reversal Risk / Continuation / Unclear

### 8 — Daily Nasdaq Bias
Direction + Confidence (High / Medium / Low) + Professional reasoning

### 9 — No-Trade Filter
Checks for major event risk and session quality at the 10 AM window

### 10 — Final Trader Report
Complete summary with **Trade or Avoid** decision and risk level

---

## ⚠️ Important Disclaimers

- This system does **not** have live market data or API access
- All data must be **manually provided** by the user
- This is **not** financial advice
- The system evaluates **probability**, never guarantees
- Think like a risk manager, not a signal follower

---

## 💬 Example Prompt Usage

Paste the full system prompt into Claude (claude.ai) or your preferred LLM, then submit your filled input template for that session.

**Recommended model:** Claude Sonnet or Opus for best analytical depth.

---

## 📁 Repository Structure

```
/
├── README.md               ← This file
├── prompt/
│   └── system_prompt.txt   ← Full analyst system prompt
└── templates/
    └── input_template.txt  ← Daily input data template
```

---

## 🤝 Contributing

Feel free to fork and adapt this for:
- Other instruments (ES, YM, RTY, EURUSD)
- Different session times (London open, Asian session)
- Additional news types (earnings, Fed minutes, jobless claims)

---

## 📜 License

MIT — free to use, modify, and share.

---

*Built for traders who want structure, not noise.*
