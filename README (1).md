# 🇮🇳 India Startup Intelligence Dashboard

> A live, interactive financial intelligence dashboard tracking India's startup ecosystem from 2023 to 2026 — funding trends, unicorns, IPOs, acquisitions, and shutdowns. Powered by Claude AI.

**[→ View Live Dashboard](https://bhargavram0828.github.io/india-startup-dashboard)**

---

## What This Is

A single-file HTML dashboard I built and maintain as a personal project to track the India startup ecosystem in real time. It uses the Claude API to generate live drill-down intelligence on demand — no backend, no database, no server.

Everything runs in the browser. You bring your own Claude API key.

---

## Features

| Section | What it shows |
|---|---|
| **KPI Cards** | Total funding, unicorns, deal count, avg deal size, IPOs — filterable by year (2023/2024/2025/2026) |
| **Quarterly Funding Chart** | Bar chart from Q1 2023 to Q1 2026 YTD |
| **Sector Share Donut** | Funding split by sector — 2023, 2024, 2025 |
| **Deal Stage Breakdown** | Seed → IPO funnel by year |
| **Ecosystem Shift Panel** | Key metric changes 2023 → 2025 at a glance |
| **Sector Heat Map** | 8 sectors with company dropdowns, filter by trending/top 5 |
| **Notable Deals by Year** | 2023 / 2024 / 2025 / 2026 YTD — 5 shown, expand to 10 |
| **Drill-Down Intelligence** | 4 panels (Unicorns / IPOs / Acquired / Shutdowns) — filter by sector AND year, powered by Claude API |
| **AI Query Engine** | Ask anything about the India ecosystem — returns compact bullet insights |

---

## How to Use

### Option A — Just open the file
Download `index.html` → open in any browser. That's it.

### Option B — Use the live GitHub Pages link
Visit the link at the top of this README.

### Connecting the AI features
The drill-down panels and query engine use the Claude API. To activate:

1. Go to [console.anthropic.com](https://console.anthropic.com) → API Keys → Create Key
2. Paste the key (`sk-ant-api03-...`) into the key field at the top of the dashboard
3. Click **Connect**
4. Your key is saved in your browser — it auto-loads on next visit

**Cost:** ~$0.002–0.005 per query. A typical session costs less than ₹1.

---

## Tech Stack

```
HTML + CSS + Vanilla JavaScript    — zero dependencies, zero frameworks
Claude API (claude-sonnet-4)       — AI drill-down and query engine
Google Fonts                       — Playfair Display + JetBrains Mono
```

No npm. No build step. No backend. One file.

---

## Data Sources & Methodology

| Data type | Source |
|---|---|
| Historical funding figures | Tracxn, Inc42, Bain India VC Report 2024 |
| Unicorn list | Hurun India Unicorn Index 2024 |
| IPO data | NSE/BSE official listings |
| Deal-level data | Public reporting (YourStory, TechCrunch India, Entrackr) |
| 2025 estimates | Trend extrapolation from Q1–Q3 2025 |
| 2026 YTD | AI estimates — directional only, not audited |

> All figures are for research and analysis purposes. Not financial advice.

---

## Update Log

| Version | Date | What changed |
|---|---|---|
| v1.0 | Mar 2026 | Initial publish — full dashboard with AI drill-downs |

---

## Roadmap

- [ ] Connect live data via Google Sheets + Make.com + Apify
- [ ] Add city-level heat map (Bengaluru / Mumbai / Delhi NCR breakdown)
- [ ] Add investor activity tracker (most active VCs by quarter)
- [ ] Add weekly email digest mode
- [ ] Mobile-optimised layout

---

## Running Locally

```bash
# No setup needed — just open the file
open index.html

# Or serve locally
python3 -m http.server 8000
# then visit http://localhost:8000
```

---

## License

MIT — fork it, use it, build on it. Credit appreciated but not required.

---

*Built with Claude · Data covers 2023–2026 · India startup ecosystem*
