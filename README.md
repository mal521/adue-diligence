# ADUe diligence

A beginner-friendly financial model for evaluating properties where an ADU (Accessory Dwelling Unit) can be built. Delivered as a single-page web app with a vaporwave/outrun aesthetic on an architectural dot-grid background.

## Features
- **Property & ADU Feasibility** - guided checklist with green/yellow/red scoring
- **Legal & Permitting** - state-specific guidance (CA, OR, WA, TX, CO) and timeline estimates
- **ADU Build Cost Estimator** - toggle beds/bath/sqft/construction type with cost breakdown
- **Rental Income Estimator** - comparable rent analysis with vacancy assumptions
- **Full 10-Year DCF Model** - two cash flow tables: income flow (GPR through levered CF) and wealth building (equity, appreciation, sale proceeds), with plain-English explanations
- **Summary Metrics** - cap rate, DSCR, cash-on-cash, IRR, NPV, MOIC
- **Glossary** - plain-English tooltips for every financial term
- **.xlsx Export** - multi-sheet spreadsheet (inputs, feasibility, cash flow, detailed cash flow, summary)

## Design
- Vaporwave/outrun aesthetic with muted neons (teal, dusty magenta, warm orange)
- Dual-layer architectural dot grid background
- CRT scanline overlay, floating gradient sun, glass-panel cards
- Scroll-reveal animations, hover glow effects, blinking terminal cursor
- Orbitron (headings) + Share Tech Mono (body) typography
- Hamburger menu with solid overlay for mobile
- Touch-friendly tooltips on mobile (tap to show/dismiss)
- Responsive down to 320px

## Usage
Open `index.html` in any modern browser. No build tools or server required.

## Deploy
```
npx netlify-cli deploy --dir . --prod
```

## Tech
- Vanilla HTML/CSS/JS (single file)
- SheetJS (CDN) for .xlsx export
- Google Fonts (Orbitron + Share Tech Mono)
