# Salary Simulator — USD to Local Currency

Interactive tool to simulate the impact of USD exchange rate fluctuations on a fixed USD salary converted to local currency (BRL, UYU, EUR, or any live rate via Frankfurter API).

**No build tools required.** Open `index.html` in a browser and it works.

## Quick Start

```bash
# Just open the file
open index.html
# or: xdg-open index.html
# or: double-click in your file manager
```

Or serve locally:
```bash
python3 -m http.server 8080
# → http://localhost:8080
```

## Features

- **BRL / UYU / EUR** — 13-month history (May 2025 – May 2026) with confirmed data + estimates
- **Any currency** — enter any ISO 4217 code (GBP, JPY, ARS, etc.) — fetches live rate from [Frankfurter API](https://www.frankfurter.app/) (ECB), no API key needed
- **Tax simulation** — BRL (CLT: INSS + IRPF 2026 rules with simplified deduction) and UYU (BPS + IRPF)
- **Risk analysis** — shows purchasing power loss if salary is locked at today's rate and USD returns to peak
- **Responsive** — works on desktop, tablet, mobile (320px+)
- **Dark theme** — built-in, no toggle needed

## Deploy to GitHub Pages (Free)

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Under "Branch", select `main` / root
4. Save → your site is live at `https://GitOpsGarage.github.io/salary-simulator/`

No build step. No config file. No cost.

## Data Sources

| Currency | Source |
|----------|--------|
| BRL | x-rates.com monthly averages (2025) + estimates (2026) |
| UYU | exchange-rates.org / poundsterlinglive |
| EUR | ECB via EUR/USD data + estimates |
| Any other | [Frankfurter API](https://www.frankfurter.app/) (live ECB rates) |

## License

MIT
