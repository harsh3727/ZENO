# ZENO — Zero-waste Expense & Net-growth Optimizer

A personal finance web application that transforms cashback and locked vouchers into real invested wealth. ZENO replaces passive reward accumulation with active financial empowerment — smart voucher allocation, budget discipline, and automatic micro-investment in one platform.

---

## Project Overview

ZENO addresses a common financial blind spot: people earn cashback and vouchers but never convert them into lasting wealth. The app provides:

- **Eco-Wallet** — Unified balance across parent brand ecosystems (e.g. Reliance: JioMart, Reliance Trends, Reliance Digital, Jio-BP). Cashback earned at any brand in the group is fungible across the whole group.
- **Locked Voucher Advisor** — For standalone brand vouchers (Myntra, Swiggy, etc.), ZENO maps the voucher to matching expense categories, calculates real cash freed, and guides you to invest it immediately.
- **Expense Builder** — Structured monthly budget with per-category cashback tracking and budget vs. actual analysis.
- **Investment Portfolio** — Sweep surplus and cashback into instruments (Digital Gold, Flexi Cap MF, Bluechip Fund, Liquid MF, NPS, PPF) with XIRR tracking.
- **Goals & Milestones** — Age-based financial milestones (Emergency Fund, Home Down Payment, Retirement Corpus) with progress tracking.
- **ZENO AI Agent** — Conversational financial advisor powered by Groq (Llama 3.3 70B), with full user financial context injected into every prompt.
- **Ledger** — Complete transaction history: earned, spent, invested, and swept.
- **Wealth Score** — Composite empowerment score based on cashback reinvestment rate, goal completion, and expense discipline.

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | Vanilla HTML5, CSS3, JavaScript (ES6+) — single-file SPA |
| Charts | Chart.js 4.4.1 (via CDN) |
| Fonts | Google Fonts — Playfair Display, Outfit, JetBrains Mono |
| AI / LLM | Groq API — `llama-3.3-70b-versatile` |
| Auth & Storage | Browser `localStorage` (no backend) |
| Hosting | Any static file server or GitHub Pages |

---

## Setup Instructions

### Prerequisites
- A modern browser (Chrome, Firefox, Edge, Safari)
- the app works offline with smart fallback responses

### Run Locally
Access - https://harsh3727.github.io/ZENO/
(
FOR DEVELOPER
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/zeno-finance.git
cd zeno-finance

# 2. Open in browser — no build step required
open index.html
# OR serve with any static server:
npx serve .
# OR
python -m http.server 8080


Then open `http://localhost:8080` in your browser.
)


## APIs & External Services

| Service | Purpose | Required? |
|---|---|---|
| [Groq API](https://console.groq.com/docs/openai) | Powers the ZENO AI Agent chatbot via `llama-3.3-70b-versatile` | Optional |
| Google Fonts | Loads Playfair Display, Outfit, JetBrains Mono | Requires internet |
| Chart.js CDN (cdnjs) | Renders bar, doughnut, and pie charts | Requires internet |

### Groq API Details
- **Endpoint:** `https://api.groq.com/openai/v1/chat/completions`
- **Model used:** `llama-3.3-70b-versatile`
- **Auth:** Bearer token (your Groq API key)
- **Key storage:** Browser `localStorage` only — never sent to any backend

---

## Project Structure
