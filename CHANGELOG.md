# Changelog

All notable changes to this project will be documented in this file.

## [1.2.0] - 2026-05-15

### Added

- USD/BRL/UYU switchable input modes — toggle now controls input currency, not just display
- PJ Simples Nacional Anexo V tax panel for USD mode (6 RBT12 brackets, effective rate formula)
- Auto-conversion of input value when switching modes (uses current exchange rate)
- USD mode cards: today in BRL + today in UYU + best/worst BRL historical
- BRL/UYU modes: cards show USD equivalent with amplitude of risk
- Chart inverts for BRL/UYU modes (local currency → USD historical value)
- Risk box and monthly table adapt copy and math per active mode

## [1.1.0] - 2026-05-14

### Fixed

- FONASA tiered rate: 3% up to 2.5 BPC (~$U 17,160), 4.5% above — was incorrectly flat 3%

## [1.0.0] - 2026-05-14

### Added

- Initial release: salary simulator for USD → BRL/UYU
- CLT Brazil taxes — progressive INSS + IRPF 2026 with simplified deduction and gradual reducer (Lei 15.270/2025)
- Uruguay taxes — BPS jubilatorio 15%, FONASA, FRL 0.1%, IRPF with BPS credit
- 13-month exchange rate history (May 2025 – May 2026) with confirmed/estimated data
- Pure SVG chart (no chart library), responsive
- Risk analysis box with historical peak comparison
- GitHub Pages ready, no build step
