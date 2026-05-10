# Contributing

This list tracks the connectors visible across Lovable's two integration surfaces — **App Connectors** (workspace-scoped, available to apps you build) and **Chat Connectors** (MCP servers attached to your build session). Contributions welcome.

> This is an independent, community-maintained project. Not affiliated with, endorsed by, or sponsored by Lovable.

## What You Can Contribute

### New Connectors
When Lovable adds new integrations to either surface, submit a PR adding them to the appropriate section and category with a description and use case. **In the PR description, state which surface the connector belongs to — App or Chat.** App connectors and Chat connectors are tracked in different parts of the README.

### Surface Migrations
Lovable occasionally promotes a Chat MCP into a full App Connector (or vice versa). If a connector has moved between surfaces, submit a PR moving the entry and noting the change in the PR description.

### Improved Descriptions
If a description or use case is missing detail or could be more helpful, submit a PR with a better one. Use cases should describe what someone would actually build with the connector inside Lovable, not generic vendor marketing.

### Category Corrections
If a connector is in the wrong category, submit a PR moving it. Category boundaries are fuzzy — when in doubt, follow what the connector does *inside Lovable's surface*, not the vendor's own self-categorization.

### Field Reports
Tested a connector inside Lovable and have real-world notes? Add a brief field report below the connector entry:

```markdown
- [Connector Name](https://example.com) - Description. *Use case: ...*
  > **Field report:** One paragraph on what worked, what didn't, what surprised you. Be specific.
```

Field reports are most useful on connectors with non-obvious authentication flows, rate limits, or capability gaps inside Lovable's specific integration shape.

## Guidelines

- One PR per change unless closely related.
- Keep descriptions concise — one sentence for the description, one for the use case.
- Use cases should be specific and practical, not marketing copy. Anchor the use case in something a Lovable builder would actually do during a build.
- Don't add connectors that aren't in Lovable's official in-product directory. This list tracks Lovable's curated connector surface, not all MCP servers (see [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) for that).
- Link to the connector vendor's canonical homepage, not to a Lovable docs page or third-party marketplace listing.
- Maintain alphabetical order within categories.
- Apply legend markers conservatively: `⚡` only for connectors **Enabled** by default in a fresh Lovable workspace, `🔜` only for connectors marked **Soon** in the directory.

## Surface Tracking

Lovable exposes connectors across two distinct surfaces, and this list keeps them separate:

- **App Connectors** — workspace-level integrations available to apps you build. Configured once by workspace admins; accessible at runtime by every app in the workspace. Examples: Supabase, Stripe, Gmail, Slack, Twilio.
- **Chat Connectors (MCP)** — Model Context Protocol servers attached to the build session itself, not the shipped app. Personal — only visible to you while building. Examples: Figma (local MCP), Sentry, Linear, Notion, Atlassian.

A few vendors appear on both surfaces (Linear, Granola). When that happens, the App entry covers the runtime integration and the Chat entry covers the build-time context. Both are tracked separately in this list.

## Updates

This list is updated as Lovable's directory changes. If you notice connectors that have been added, removed, promoted between surfaces, or had their **Soon** flag dropped — and the change isn't reflected here — please open an issue or PR.
