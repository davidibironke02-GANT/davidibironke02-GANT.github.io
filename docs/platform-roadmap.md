# GANT Exchange Roadmap

The roadmap tracks how we move from the existing static materials to a production-ready exchange with authenticated users.

## Milestone 1: Foundations
- Define the domain model (users, roles, lots, bids, trades, payments, documents) and shared vocabulary.
- Choose initial tech stack (front-end framework, API framework, data store) and lay out repo folders (e.g., `apps/web`, `services/api`, `packages/ui`).
- Add CI for linting/tests, basic security scanning, and a preview deploy for the static site.

## Milestone 2: Identity & Access
- Implement authentication (email + password first) with session management and password resets.
- Role-based access control with auditable events for high-risk actions (bid creation, trade approval, payouts).
- Organization/team membership for buyers, farmers, and warehouse partners.

## Milestone 3: Marketplace & Escrow
- Lot listing creation: commodity, volume, grade, location, timing, and pricing expectations.
- Bid workflow: submit, counter, accept; trigger escrow initiation on acceptance.
- Trade confirmation flows with document capture (contracts, inspection results) and status history.

## Milestone 4: Traceability & Compliance
- Lot traceability timeline with corridor checks and evidence attachments per checkpoint.
- Compliance checklist per trade (certifications, insurance, inspections) with expiry alerts.
- Exportable audit trail for regulators and counterparties.

## Milestone 5: Financing & Settlement
- Credit line requests with approval workflow and configurable limits per organization.
- Payment schedules, status tracking, and notifications tied to trade milestones.
- Settlement dashboard with reconciled payouts, downloadable statements, and dispute handling steps.

## Milestone 6: Observability & Operations
- Metrics and alerting for API latency, failed payments, and data pipeline health.
- Admin tooling for support to view/adjust trades, user access, and document state.
- Backups, disaster recovery runbooks, and a privacy/compliance review checklist.

## Contribution expectations
- Document acceptance criteria and data contracts before shipping features; include API schemas (OpenAPI/JSON Schema) and ERDs where applicable.
- Add automated tests and security gates with every new service.
- Keep public marketing pages intact while platform work ships in scoped folders.
