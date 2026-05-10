# Changelog

All notable changes to this list will be documented in this file. Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/); versioning follows [Semantic Versioning](https://semver.org/) — MAJOR for category restructures, MINOR for connector additions, PATCH for description/URL fixes.

## [Unreleased]

### Planned for v1.1.0
- Track Lovable's enterprise / paid-tier connector surface as it diverges from the public directory.
- Add `awesome-lint` to CI once the repo is ≥30 days old (lint blocks submissions on `git-repo-age` until 2026-06-09).
- Field reports for the most-used App Connectors (Supabase, Stripe, Resend) and most-used Chat Connectors (Figma, Sentry, Linear).
- Reciprocal sister-list backlinks once published.
- Per-recipe build templates linked from Stack Recipes (one starter project per recipe).

---

## [1.0.1] — 2026-05-10

### Added
- **Stack Recipes** section — 9 App Connector recipes + 4 Chat Connector recipes covering canonical Lovable build patterns (SaaS Starter, BYO-Backend SaaS, Headless Ecommerce, Internal Operations Tool, AI Agent App, Microsoft 365 Power User Tool, Privacy-First Closed Stack, Sales-Ops Dashboard, Content + Comms Marketing Site, Engineering Build Session, Product-Decision Build Session, Design-System-Driven Build, Customer-Voice Build).
- Stack Recipes link surfaced in Contents under a new **Quick reference** subhead so the Contents-as-TOC navigation includes it.
- Disclaimer that recipes are independent curation, not a Lovable recommendation.

---

## [1.0.0] — 2026-05-10

### Added
- Initial seed: **47 App Connectors across 17 categories** + **16 Chat (MCP) Connectors across 10 categories** mirroring Lovable's in-product directory.
- README.md modeled on the `Perplexity-Connectors-awesome-list-` v1.1.0 structure (About / Legend / categorized contents / Contributing / Related / License).
- CONTRIBUTING.md with surface-tracking guidelines (App vs Chat) and entry style guide.
- code-of-conduct.md adopting Contributor Covenant 2.1.
- LICENSE under **CC0-1.0** to match the awesome-list canonical convention.
- Two-marker Legend: `⚡` (Enabled by default in new Lovable workspaces) and `🔜` (Coming Soon).
- Uncertain vendor URLs verified via Exa web search prior to publication — confirmed Aikido on `.dev`, Attention on `.com`, Confidence (both Exp and Flags) on `confidence.spotify.com`, and Polar on `.sh`.

### Categories — App Connectors
Lovable Native · Authentication and Database · Payments and Commerce · AI, Voice, and Search · Email and Messaging · Calendar and Productivity · Documents and Files · Content Management · CRM, Sales, and Recruiting · Project Management · Data and Analytics · Web Scraping · Meeting Intelligence · Workflow Automation · Security · Media and Streaming · Coming Soon.

### Categories — Chat Connectors (MCP)
Product Analytics · Project Management and Knowledge · A/B Testing and Feature Flags · Design and Whiteboarding · Content Management · Meeting Intelligence · AI Video · Workflow Automation · Billing · Error Tracking and Monitoring · Custom MCP Servers.

[Unreleased]: https://github.com/rdmgator12/awesome-lovable-connectors/compare/v1.0.1...HEAD
[1.0.1]: https://github.com/rdmgator12/awesome-lovable-connectors/compare/v1.0.0...v1.0.1
[1.0.0]: https://github.com/rdmgator12/awesome-lovable-connectors/releases/tag/v1.0.0
