# <img width="40" height="40" alt="Screenshot 2025-07-12 at 02 12 51" src="https://github.com/user-attachments/assets/34a56406-36da-48e9-ade1-24733d13a9fd" /> Norns AI 

---

## ✨ Overview

**Norns AI** is a powerful, modular financial research and analytics platform — tailored for modern investors, analysts, and fintech builders.

Built for **clarity, insight, and agency**, it fuses structured market data with real-world news, advanced risk tools, and conversational AI agents in a clean, open-source workspace.  

Whether you're scanning for opportunities, managing portfolio risk, or decoding market chaos — Norns AI helps you act smarter, faster.

---

## 🔍 Core Features

### 📈 1. Real-Time Financial Dashboard
- Multi-asset data: equities, crypto, macro, FX, options, fixed income
- Economic indicators: BLS, FRED, IMF, central bank data, liquidity metrics
- Interactive visualizations and AI explanations of economic data
- Earnings call parsing + sentiment (FinBERT + LLM)

---

### 🧠 2. Agent-Powered Market Intelligence

#### **Holmes Agent** – *“Why is this moving?”*
> Detects and explains price spikes using correlated events, earnings surprises, macro shifts, and sector momentum.

#### **Polo Agent** – *Opportunity scout*
> Finds high-alpha setups based on custom screeners, filters, valuation anomalies, and unusual flows.

#### **Betty Agent** – *Sentiment overlay*
> Surfaces retail positioning from Reddit, Twitter, and short interest trends. Great for detecting froth, fear, or squeezes.

All agents are extensible via config + prompt schema.

---

### 💼 3. Portfolio Tools

- Upload CSV of holdings or connect via brokerage API
- Track P&L, allocation, and sector exposure in real time
- VaR calculator (95%, 99%) using **Monte Carlo simulations**
- Stress testing: see what happens under 2008/COVID-style scenarios
- Risk distribution curve visualizer (D3.js)
- Notion sync: push trades or performance metrics as widgets

---

### 🏦 4. Meta Investment Bank (Meta IBD)
#### Inspired by the operational flow of a real investment bank, Meta IBD is a multi-agent system that simulates roles like:

- 🧠 Financial Analyst (valuation, DCFs, KPI scoring)
- 📈 Quant (factor screens, risk model analysis)
- 📋 Strategy Lead (competitive analysis, positioning)
- 🧾 Macro Analyst (policy impact, inflation/debt tracking)

This feature uses a MetaGPT-style orchestration layer, turning user input (e.g. "Should I buy AAPL after CPI data?") into structured financial insight across disciplines — generating:
- Investment memos
- Data tables
- KPI diagnostics
- Cross-sector impact analysis
All AI activity is locally controlled and customizable per user SOP.

---

### 📬 5. AI Digest & Newsletter Engine

- Integrates with top finance newsletters (Amplify, Finimize, Daily Upside)
- LLM-generated TL;DR of daily editions
- **Weekly AI wrap** across macro, equities, crypto
- Digest is stored for review and shared via dashboard

---

### 📉 6. Risk Modeling & Simulation
#### Upload or connect portfolio data

- Live tracking of allocation, sector exposure, unrealized gain/loss
- VaR Calculator: Monte Carlo simulations at 95% or 99% confidence
- Stress Tests: See what happens under 2008, COVID, or custom drawdowns
- Risk Curves: Visualize distribution of outcomes over time
- Historical correlation matrix (coming soon)

---

### 🔐 7. Modular & Secure by Design

- Deployable locally or to private cloud (no vendor lock-in)
- Modular extension system: add agents, widgets, or custom APIs
- FastAPI backend with clean REST routes
- All data requests, AI prompts, and dashboards are user-controlled
  
---

### 🌐 8. OSINT Signals Engine

- Surfaces intelligence from public datasets, regulatory updates, social platforms, and crowd behavior  
- Powers Betty Agent (retail sentiment), Holmes Agent (event detection), and Polo Agent (opportunity spotting)  
- Expandable architecture: plug in RSS, X (Twitter), Reddit, YouTube, or filings feeds  

---

## 🧰 Tech Stack

| Layer        | Tools                                      |
|--------------|--------------------------------------------|
| Frontend     | React, Tailwind, Next.js, Recharts, D3.js  |
| Backend      | Python, FastAPI, Redis, Pandas, NumPy       |
| AI Models    | Qwen, GPT-4, FinBERT, OpenAI (optional)     |
| Data Feeds   | Yahoo Finance, FRED, IMF, SEC, CoinGecko    |
| Portfolio    | CSV ingest, SQLite, OAuth (optional)        |
| Newsletter   | Custom fetchers, Notion API, scraping utils |
| Hosting      | Local / Vercel / Railway / Render           |

---

## 🚀 Getting Started

bash
# Clone the repo
git clone https://github.com/yourusername/norns-ai.git
cd norns-ai

# Backend setup
cd backend
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
uvicorn main:app --reload

# Frontend setup
cd ../frontend
npm install
npm run dev

🧠 Philosophy
Named after the Norns of Norse mythology — the weavers of fate — this platform helps you understand and shape the forces that move global markets.

Built as a long-term open-source research companion, Norns AI is ideal for:
- Indie quants
- FinTech developers
- Retail investors
- Investment researchers
- AI agents engineers

🛠 Coming Soon
Agent chat overlay for direct financial Q&A

PDF export of dashboards

Portfolio simulation via scenario builder

Macro newsletter integration

TradingView-style charting with AI annotations
