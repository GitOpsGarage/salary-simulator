# Salary Simulator — USD / BRL / UYU

Interactive tool to simulate salary in three currencies with tax breakdown and 13-month exchange rate history.

**No build tools required.** Open `index.html` directly or serve locally.

## Quick Start

```bash
python3 -m http.server 8080
# → http://localhost:8080
```

Or just open `index.html` in a browser.

## Modes

| Mode | Input | Tax calculation |
|------|-------|-----------------|
| **USD** | Salary in dollars | PJ Brazil — Simples Nacional Anexo V |
| **BRL** | Salary in reais | CLT Brazil — INSS + IRPF 2026 |
| **UYU** | Salary in pesos | BPS (jubilatorio + FONASA + FRL) + IRPF |

Switching modes auto-converts the input value using the current exchange rate.

## Features

- **13-month history** (May 2025 – May 2026) with confirmed rates + estimates
- **PJ taxes (USD mode)** — Simples Nacional Anexo V, effective rate by RBT12 bracket
- **CLT taxes (BRL mode)** — INSS progressive + IRPF 2026 with gradual reducer (Lei 15.270/2025)
- **UY taxes (UYU mode)** — BPS jubilatorio 15%, FONASA tiered (3%/4.5%), FRL 0.1%, IRPF with BPS credit
- **Risk analysis** — shows purchasing-power loss if exchange rate returns to historical peak
- **SVG chart** — confirmed vs estimated data points, no chart library
- **Responsive** — works on desktop, tablet, mobile (320px+)

## Data Sources

| Currency | Source |
|----------|--------|
| BRL | x-rates.com monthly averages (2025) + estimates (2026) |
| UYU | exchange-rates.org + estimates (2026) |

## Deploy

GitHub Pages: push to `main`, enable Pages on root. Live at `https://GitOpsGarage.github.io/salary-simulator/`.

No build step. No config. No cost.

## License

MIT
