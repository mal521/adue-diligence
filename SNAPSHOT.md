# ADUe diligence - Snapshot

**Date:** 2026-03-05
**Status:** Feature-complete, deployed, part of 3-site suite

## What's Built
Single-page ADU investment financial model with 6 interactive sections + glossary.
Original vaporwave design with Orbitron + Share Tech Mono fonts, dot grid, scanlines, skewed buttons, neon accents.

## Recent Changes (2026-03-05)
- Fixed capital gains tax (was collected but never applied to sale proceeds)
- Added `computeSaleMetrics` helper to DRY up triplicated sale/IRR/MOIC logic
- Clamped IRR Newton-Raphson solver to prevent divergence
- Added division-by-zero guards (calcMonthlyPayment, cap rate, cash-on-cash)
- Simplified tax savings calculation (removed no-op ternary)
- Removed dead JADU permit branch, unused params, redundant init calls
- Migrated all deployment references from Netlify to GitHub Pages

## Previous Changes
- Subtler dot grid (reduced opacity from 0.18 to 0.10, larger spacing 28px)
- Dark/light mode toggle (bottom-right button, persists via localStorage)
- Removed "Print / PDF" button (export .xlsx only)
- Added shared top nav bar linking to sister sites
- Backup of pre-redesign version saved as `index-original.html`

## Sister Sites
- **ADU:** https://mal521.github.io/adue-diligence (this site)
- **Single-Family:** https://mal521.github.io/single-family-dd
- **Multi-Family:** https://mal521.github.io/multifamily-dd

## Key Files
- `index.html` - entire app (single file)
- `index-original.html` - backup of original before any changes
- `README.md` - project description

## Deployment
- **URL:** https://mal521.github.io/adue-diligence
- **Method:** GitHub Pages (auto-deploys from main branch)
