# GANT Exchange

This repository hosts the public marketing site for the GANT Exchange and the working space for the upcoming transaction platform. Until the authenticated product is available, the static pages in this repo power external communications and flow walkthroughs.

## Repo layout
- **Public site (legacy):** top-level HTML files and images that describe the exchange, financing, and traceability offerings.
- **Docs:** planning notes and roadmaps for the authenticated GANT Exchange experience.

## Running the site locally
The current site is static. You can open any HTML file directly in a browser or serve the repo root:

```bash
python -m http.server 8000
# visit http://localhost:8000
```

## Platform goals (next phase)
We are evolving this repo into the GANT Exchange platform that supports authenticated buyers, farmers, and warehouse partners. Core capabilities:
- **Identity & roles:** sign-up, login, and role-based permissions for buyers, farmers, and warehouse operators.
- **Marketplace flows:** lot listings, bids, trade approval, and escrow confirmation.
- **Traceability & compliance:** corridor checks, inspection documents, and certification tracking per trade.
- **Financing & settlement:** credit line requests, scheduled payouts, and reconciliation dashboards.

## How to contribute now
- Keep the static pages working—avoid breaking public routes while adding platform code in dedicated folders (e.g., `apps/web`, `services/api`).
- Add specs and acceptance criteria for new features under `docs/` before building them.
- Favor modular components and well-defined API contracts to keep teams decoupled.
- Document environment variables and setup steps alongside any new service you add.

## Roadmap
See `docs/platform-roadmap.md` for milestone-level planning of the authenticated exchange.
