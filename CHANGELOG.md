# Changelog

All notable changes to this list will be documented in this file. Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/); versioning follows [Semantic Versioning](https://semver.org/) — MAJOR for category restructures, MINOR for connector additions, PATCH for description/URL fixes.

## [Unreleased]

### Planned for v1.1.0
- Track Lovable's enterprise / paid-tier connector surface as it diverges from the public directory.
- Field reports for the most-used App Connectors (Supabase, Stripe, Resend) and most-used Chat Connectors (Figma, Sentry, Linear).
- Reciprocal sister-list backlinks once published.
- Per-recipe build templates linked from Stack Recipes (one starter project per recipe).
- Add a "Lovable as MCP" section covering Lovable's outbound MCP server (`https://mcp.lovable.dev`) — distinct from the inbound chat-connector surface; lets external agents drive Lovable. Research preview as of May 7, 2026.

---

## [1.0.3] — 2026-05-22

### Added
- **Maps and Location** (new category): Google Maps Platform — geocoding, routes, places, embedded maps, address validation, weather, and air quality APIs. Workspace admins can choose Managed by Lovable or BYO Google Cloud credentials. Confirmed live in Lovable's published changelog 2026-05-22.
- **Media and Streaming:** TikTok — read profile information, follower counts, like counts, video statistics, and published video metadata. Read-only connector; does not support publishing to TikTok.

### Changed
- **Semrush** graduated from Coming Soon → **Data and Analytics**. 🔜 marker dropped. Same `semrush.com` URL retained; description rewritten to match the GA capability surface (keyword research, domain analytics, backlinks, paid-search data, position tracking) per Lovable's 2026-05-22 changelog entry and the May 13 Lovable × Semrush partnership announcement.
- Coming Soon section removed from README and Contents TOC — currently no 🔜 entries in the in-product directory. 🔜 legend marker retained for future weeks.
- Header counts: App Connectors 50 → 52, version 1.0.2 → 1.0.3.

### Notes
- Chat Connectors surface: no changes this week. 16 entries unchanged.
- Lovable MCP server (research preview, May 7, 2026) still **not** added — outbound (Lovable as MCP server for external agents), not inbound (third-party context into Lovable's chat). Held for v1.1.0 in a dedicated section.
- "Chat with Lovable in Telegram" (Settings → Devices & apps) is Lovable-as-Telegram-bot, not Telegram as a new connector — Telegram already listed as an App Connector since v1.0.0. No change.
- Net category count unchanged at 27 (17 App + 10 Chat): −Coming Soon, +Maps and Location.

---

## [1.0.2] — 2026-05-15

### Added
- **Email and Messaging:** Mailgun — transactional email API with domain verification and delivery tracking. Confirmed live in workspace App Connectors directory; tied to Sinch–Lovable strategic partnership announced February 2026.
- **Content Management:** Notion (App) — runtime read/write to Notion pages and databases from a deployed app. Listed as `Notion (App)` to distinguish from the chat-side Notion entry which only reads context during build; URLs differ (`notion.so/product` vs `notion.so`) to satisfy awesome-lint double-link rule.
- **Coming Soon:** Semrush — SEO, keyword research, and competitive analysis platform.

### Changed
- **Data and Analytics:** Google Search Console moved out of Coming Soon — now generally available as a default-enabled App Connector. Re-listed under Data and Analytics; `🔜` marker dropped.
- Header counts: App Connectors 47 → 50, version 1.0.1 → 1.0.2.

### Notes
- Chat Connectors surface: no changes this week. Live in-product directory verified all 16 entries unchanged.
- Lovable MCP server (research preview, May 7, 2026) is **not** added here — it's outbound (Lovable as MCP server for external agents), not inbound (third-party tools providing context). Held for v1.1.0 in a dedicated section.

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

[Unreleased]: https://github.com/rdmgator12/awesome-lovable-connectors/compare/v1.0.3...HEAD
[1.0.3]: https://github.com/rdmgator12/awesome-lovable-connectors/compare/v1.0.2...v1.0.3
[1.0.2]: https://github.com/rdmgator12/awesome-lovable-connectors/compare/v1.0.1...v1.0.2
[1.0.1]: https://github.com/rdmgator12/awesome-lovable-connectors/compare/v1.0.0...v1.0.1
[1.0.0]: https://github.com/rdmgator12/awesome-lovable-connectors/releases/tag/v1.0.0
