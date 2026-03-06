# 🇮🇳 India Startup Intelligence Dashboard

> A live, interactive financial intelligence dashboard tracking India's startup ecosystem from 2023 to 2026 — funding trends, unicorns, IPOs, acquisitions, and shutdowns. Powered by Claude AI.

**[→ View Live Dashboard](https://bhargavram0828.github.io/india-startup-dashboard)**

---

## What This Is

A single-file HTML dashboard built and maintained as a personal project to track the India startup ecosystem. It uses the Claude API to generate live drill-down intelligence on demand — no backend, no database, no server required on your end.

All static data (KPI cards, charts, deals, sector heatmap) loads instantly for everyone with **no sign-up and no API key needed.**

The AI-powered features (drill-down intelligence + query engine) require your own Claude API key — each visitor uses their own, so there's no shared cost.

---

## How to Use

### Viewing the dashboard
Just visit the live link above. Everything loads immediately — charts, KPI cards, sector heatmap, notable deals. No account needed.

### Activating AI features
The drill-down panels and AI query engine need a Claude API key:

1. Go to **[console.anthropic.com](https://console.anthropic.com)** → sign up (free)
2. Go to **API Keys** → click **+ Create Key** → copy it immediately
3. Add a payment method under **Billing** (required by Anthropic to activate keys)
4. Set a **spend limit** under Settings → Limits → recommend $5/month
5. Paste the key into the field at the top of the dashboard → click **Connect**

**Cost per session:** ~$0.002–0.005 per query. A full session costs less than ₹1.

Your key is saved in your browser — it auto-loads on your next visit and is never stored anywhere else.

---

## Features

| Section | What it shows |
|---|---|
| **KPI Cards** | Total funding, unicorns, deal count, avg deal size, IPOs — filter by 2023 / 2024 / 2025 / 2026 YTD |
| **Quarterly Funding Chart** | Bar chart Q1 2023 → Q1 2026 YTD |
| **Sector Share Donut** | Funding split by sector — 2023, 2024, 2025 |
| **Deal Stage Breakdown** | Seed → IPO funnel — 2023, 2024, 2025 |
| **Ecosystem Shift Panel** | Key metric changes 2023 → 2026 at a glance |
| **Sector Heat Map** | 22 sectors with company dropdowns, trending filter |
| **Notable Deals by Year** | 2023 / 2024 / 2025 / 2026 YTD — expand to 10 deals |
| **Drill-Down Intelligence** | Top Valued / IPOs / Acquired / Shutdowns — filter by sector + year · requires API key |
| **AI Query Engine** | Ask anything about the India ecosystem · requires API key |

---

## Tech Stack

```
HTML + CSS + Vanilla JavaScript    — zero dependencies, zero frameworks
Claude API (claude-haiku-4-5)      — AI drill-down and query engine
Cloudflare Workers                 — API proxy (handles browser security)
GitHub Pages                       — hosting
Google Fonts                       — Playfair Display + JetBrains Mono
```

No npm. No build step. No backend. One file.

---

## Data Sources

| Data | Source |
|---|---|
| Historical funding | Tracxn, Inc42, Bain India VC Report 2024 |
| Unicorn list | Hurun India Unicorn Index 2024 |
| IPO data | NSE / BSE official listings |
| Deal-level data | YourStory, TechCrunch India, Entrackr |
| 2025 estimates | Trend extrapolation from Q1–Q3 2025 actuals |
| 2026 YTD | AI estimates — directional only, not audited |

> All figures are for research and analysis purposes only. Not financial advice.

---

## Update Log

| Version | Date | What changed |
|---|---|---|
| v1.0 | Mar 2026 | Initial publish — full dashboard with AI drill-downs, Cloudflare proxy, GitHub Pages |

---

## Roadmap

- [ ] Live data via Google Sheets + Make.com + Apify scrapers
- [ ] City-level breakdown — Bengaluru vs Mumbai vs Delhi NCR
- [ ] Investor activity tracker — most active VCs by quarter  
- [ ] Mobile optimised layout
- [ ] Weekly data refresh workflow

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

## About

Built by [@bhargavram0828](https://github.com/bhargavram0828) · Powered by Claude AI · Data covers 2023–2026

*MIT License — fork it, use it, build on it.*
