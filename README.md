# Awesome Lovable Connectors [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)
[![Last Commit](https://img.shields.io/github/last-commit/rdmgator12/awesome-lovable-connectors)](https://github.com/rdmgator12/awesome-lovable-connectors/commits/main)
[![Track Awesome List](https://www.trackawesomelist.com/badge.svg)](https://www.trackawesomelist.com/rdmgator12/awesome-lovable-connectors/)

> A curated directory of every connector available across [Lovable's](https://lovable.dev) two integration surfaces — **App Connectors** (services your built apps can read from and act on) and **Chat Connectors** (MCP servers that add context while you build).

**Last updated:** June 26, 2026 · **App Connectors:** 57 · **Chat Connectors:** 16 · **Categories:** 27 · **Version:** 1.2.0

Lovable exposes integrations through two distinct surfaces. **App Connectors** are workspace-scoped integrations that your generated app can call at runtime — configured once by workspace admins, available to any app built in the workspace, powering backend, payments, email, file storage, CRM, analytics, and more. **Chat Connectors** are MCP (Model Context Protocol) servers attached to *your* build session, not the app you ship — they give Lovable's chat surface live context from product analytics, design files, error trackers, project management, and feature-flag platforms while you iterate.

This list tracks both surfaces as visible in the Lovable in-product directory on the **Last updated** date. Lovable also supports custom MCP servers — the chat surface includes a "New MCP server" entry for connecting your own. For more information, see the [Lovable documentation](https://docs.lovable.dev).

**Legend:** ⚡ Enabled by default in new Lovable workspaces · 🔜 Marked **Soon** in the Lovable directory. Connectors with neither marker are available in the standard surface and link to the third-party vendor's homepage.

> This is an independent, community-maintained list. Not affiliated with, endorsed by, or sponsored by Lovable. "Lovable" and related marks are the property of their respective owner. Each connector is the property of its respective owner.

---

## Contents

- [Stack Recipes](#stack-recipes)
- [App Connectors](#app-connectors)
- [Lovable Native](#lovable-native)
- [Authentication and Database](#authentication-and-database)
- [Payments and Commerce](#payments-and-commerce)
- [AI, Voice, and Search](#ai-voice-and-search)
- [Email and Messaging](#email-and-messaging)
- [Calendar and Productivity](#calendar-and-productivity)
- [Documents and Files](#documents-and-files)
- [Content Management](#content-management)
- [CRM, Sales, and Recruiting](#crm-sales-and-recruiting)
- [Project Management](#project-management)
- [Data and Analytics](#data-and-analytics)
- [Web Scraping](#web-scraping)
- [Maps and Location](#maps-and-location)
- [Meeting Intelligence](#meeting-intelligence)
- [Workflow Automation](#workflow-automation)
- [Security](#security)
- [Media and Streaming](#media-and-streaming)
- [Chat Connectors](#chat-connectors)
- [Product Analytics](#product-analytics)
- [Project Management and Knowledge](#project-management-and-knowledge)
- [A/B Testing and Feature Flags](#ab-testing-and-feature-flags)
- [Design and Whiteboarding](#design-and-whiteboarding)
- [Content Management (Chat)](#content-management-chat)
- [Meeting Intelligence (Chat)](#meeting-intelligence-chat)
- [AI Video](#ai-video)
- [Workflow Automation (Chat)](#workflow-automation-chat)
- [Billing (Chat)](#billing-chat)
- [Error Tracking and Monitoring](#error-tracking-and-monitoring)
- [Custom MCP Servers](#custom-mcp-servers)

## Stack Recipes

Curated combinations that solve common Lovable build patterns. Each recipe is a battle-tested pairing. Mix and match — every connector listed below works with every other listed connector.

**SaaS Starter** · `⚡ Cloud` + `⚡ Stripe` + `Resend` + `Slack`. Auth + billing + transactional email + team notifications. The default starting point for any subscription app.

**BYO Backend SaaS** · `⚡ Supabase` + `⚡ Stripe` + `Resend` + `Inngest`. When you need RLS, real-time, or your own PostgreSQL. Inngest handles long-running webhooks + scheduled jobs.

**Headless Ecommerce** · `⚡ Shopify` + `Storyblok` + `Resend`. Shopify owns commerce, Storyblok owns content, Resend handles order mail. Lovable owns the storefront.

**Internal Operations Tool** · `⚡ Supabase` + `Linear` + `Slack` + `Inngest`. Read-write internal dashboards that talk to engineering systems.

**AI Agent App** · `⚡ AI` (or `⚡ Cloud` + Anthropic/OpenAI key) + `Perplexity` + `ElevenLabs` + `⚡ Supabase`. LLM reasoning + grounded web search + voice output + persistent memory.

**Microsoft 365 Power User Tool** · `Microsoft Outlook` + `Microsoft Excel` + `Microsoft OneDrive` + `Microsoft Teams`. When everything has to live in the M365 tenant.

**Privacy-First Closed Stack** · `⚡ Cloud` + `⚡ AI`. No third-party connector configuration. Useful for first-version internal tools.

**Sales-Ops Dashboard** · `HubSpot` + `Attention` + `Slack` + `⚡ Supabase`. CRM data + call-coaching transcripts + alerts + custom rollups.

**Content + Comms Marketing Site** · `Contentful` + `Resend` + `Google Calendar`. Editor-friendly CMS, transactional email, and scheduled events.

**Engineering Build Session** (Chat) · `Linear` + `Sentry` + `Figma`. Read your actual ticket, see the actual error, see the actual design, write the actual code.

**Product-Decision Build Session** (Chat) · `PostHog` + `Notion` + `Linear`. Ground UI choices in real funnel data, pull the PRD live from Notion, scope against the ticket.

**Design-System-Driven Build** (Chat) · `Figma` + `Sanity`. Components materialize from real Figma layers, populated with real Sanity content schemas.

**Customer-Voice Build** (Chat) · `Granola` + `Linear` + `Notion`. What the customer said in the call, what the team committed to in Linear, what the spec already says in Notion.

## App Connectors

Workspace-level integrations that the apps you build with Lovable can call at runtime. Configured once by workspace admins.

## Lovable Native

- ⚡ [Cloud](https://lovable.dev/cloud) - Built-in backend, ready to use. *Use case: Standing up a database, auth, and serverless functions inside a Lovable app without provisioning external infrastructure first.*
- ⚡ [AI](https://lovable.dev/ai) - Unlock powerful AI features inside your generated app. *Use case: Adding chat completions, embeddings, or generative features to a Lovable build without wiring up your own model provider keys.*

## Authentication and Database

- ⚡ [Supabase](https://supabase.com) - Connect your own Supabase project for PostgreSQL, auth, storage, and edge functions. *Use case: Bring-your-own-backend builds that need persistent data, row-level security, real-time subscriptions, or file storage in a Lovable app.*
- [AWS S3](https://aws.amazon.com/s3/) - Read and write data files in AWS S3 buckets. *Use case: Object storage for user uploads, generated artifacts, or static assets when the app needs S3-grade durability and IAM-scoped access.*

## Payments and Commerce

- ⚡ [Stripe](https://stripe.com) - Set up payments for one-time charges, subscriptions, and marketplaces. *Use case: Adding checkout, subscription billing, customer portals, or usage-based pricing to a Lovable-built SaaS app.*
- ⚡ [Shopify](https://www.shopify.com) - Build an eCommerce store with Lovable's frontend over Shopify's commerce backend. *Use case: Spinning up a custom storefront, headless checkout, or merchant tooling that reads products, orders, and inventory from a Shopify shop.*

## AI, Voice, and Search

- [Algolia](https://www.algolia.com) - AI-powered search and discovery platform with hybrid keyword/vector search and ranking. *Use case: Adding fast, typo-tolerant instant search and AI-ranked results to a Lovable-built catalog, docs site, or marketplace, or powering RAG-style conversational answers from indexed content.*
- ⚡ [ElevenLabs](https://elevenlabs.io) - AI voice generation, text-to-speech, and speech-to-text. *Use case: Adding lifelike voiceover, dubbing, or real-time voice agents to a Lovable app — narration, IVR replacements, accessibility readers.*
- [Gemini Enterprise](https://cloud.google.com/gemini) - Search, query, and summarize data across your Google data sources. *Use case: Grounding answers in Google Workspace + connected data sources for enterprise search and Q&A inside a Lovable app.*
- [Perplexity](https://www.perplexity.ai) - AI-powered search and answer engine. *Use case: Adding live, citation-grounded web search to an app — research assistants, briefing tools, fact-checking surfaces.*
- [Replicate](https://replicate.com) - Cloud API for running, fine-tuning, and deploying open-source and custom AI models. *Use case: Calling image, audio, or language models from a Lovable app (image generation, transcription, fine-tuned inference) without managing your own GPU infrastructure.*

## Email and Messaging

- [Brevo](https://www.brevo.com) - Email, SMS, CRM, and marketing automation API. *Use case: Sending transactional and marketing email, SMS campaigns, or running CRM-style workflows from a Lovable app without standing up multiple vendors.*
- [Gmail](https://mail.google.com) - Read, send, and manage emails. *Use case: Sending notifications from a personal Gmail account, drafting replies from app context, or building inbox-aware tooling on top of a user's Google account.*
- [Mailgun](https://www.mailgun.com) - Transactional email API with domain verification and delivery tracking. *Use case: Sending verifications, receipts, and notifications from a verified domain with bounce/complaint tracking — the production path when Lovable's built-in email isn't enough.*
- [Microsoft Outlook](https://outlook.com) - Read, send, and manage emails on Microsoft 365. *Use case: Email automation in Microsoft-shop environments, drafting replies, or scanning a user's mailbox for context inside a Lovable app.*
- [Resend](https://resend.com) - Email API for developers. *Use case: Transactional email (verification, password reset, receipts) with React Email templates and developer-grade deliverability.*
- [Slack](https://slack.com) - Send messages and interact with Slack workspaces. *Use case: Posting notifications from a Lovable app to a team channel, building Slack-first tools, or triggering app actions from Slack messages.*
- [Telegram](https://telegram.org) - Messaging platform with Bot API for automated interactions. *Use case: Bot-driven notifications, customer support workflows, or two-way messaging from a Lovable app to Telegram users.*
- [Microsoft Teams](https://www.microsoft.com/en-us/microsoft-teams/group-chat-software) - Send messages and manage channels. *Use case: Posting from a Lovable app to a Teams channel, building enterprise notification flows, or wiring app events into Teams collaboration.*
- [Twilio](https://www.twilio.com) - Cloud communications platform for SMS, voice, and messaging. *Use case: Sending SMS verifications, programmable voice flows, or WhatsApp messages from a Lovable app.*

## Calendar and Productivity

- [Google Calendar](https://calendar.google.com) - Create and manage Google Calendar events. *Use case: Scheduling features inside a Lovable app — booking flows, automated event creation, calendar-aware automations.*
- [Microsoft OneNote](https://www.onenote.com) - Read and write notes inside OneNote notebooks. *Use case: Capturing app-generated notes into a user's OneNote, summarizing meetings into a notebook, or syncing structured app data to OneNote pages.*
- [Granola](https://www.granola.ai) - AI meeting notes and transcripts. *Use case: Pulling meeting transcripts into a Lovable app for summarization, searchable archives, or note-driven action item extraction.*

## Documents and Files

- [Google Docs](https://docs.google.com) - Create and edit Google Docs documents. *Use case: Generating reports, contracts, or briefings from app data directly into a user's Google Drive — share-link automation, templated document generation.*
- [Google Drive](https://drive.google.com) - Upload and download files to and from Google Drive. *Use case: File ingest and export, attaching app-generated artifacts to a Drive folder, or reading user-uploaded documents from Drive into a Lovable app.*
- [Google Sheets](https://sheets.google.com) - Read and update spreadsheet data. *Use case: Lightweight data layer for low-volume apps, exposing app data to non-technical users via a sheet, or ingesting form responses for processing.*
- [Google Slides](https://slides.google.com) - Create and manage Google Slides presentations. *Use case: Auto-generating decks from app data, templated reports, or briefing presentations triggered by app events.*
- [Microsoft Excel](https://www.microsoft.com/en-us/microsoft-365/excel) - Read and write spreadsheets. *Use case: Microsoft 365 spreadsheet automation — exporting app data to Excel, ingesting Excel-shaped data sources, or driving dashboards from Lovable apps.*
- [Microsoft OneDrive](https://onedrive.live.com) - Upload and read files in OneDrive. *Use case: File storage for Microsoft-shop deployments, document ingestion from a user's OneDrive, or syncing app outputs to OneDrive folders.*
- [Microsoft PowerPoint](https://www.microsoft.com/en-us/microsoft-365/powerpoint) - Read and write presentations. *Use case: Auto-generated decks from app data in PowerPoint format, templated business presentations, or pulling slide content for processing.*
- [Microsoft SharePoint](https://www.microsoft.com/en-us/microsoft-365/sharepoint/collaboration) - Microsoft 365 content management and document storage platform with secure file sharing. *Use case: Reading, syncing, or surfacing SharePoint documents and lists inside a Lovable internal portal, or letting users upload and retrieve files against an organization's existing SharePoint libraries.*
- [Microsoft Word](https://www.microsoft.com/en-us/microsoft-365/word) - Read and write Word documents. *Use case: Document generation in `.docx` format — contracts, reports, briefings — and ingestion of user-supplied Word files into a Lovable app.*

## Content Management

- [Contentful](https://www.contentful.com) - Headless CMS for content delivery. *Use case: Powering content-driven Lovable apps (marketing sites, product catalogs, knowledge bases) with editor-friendly Contentful as the source of truth.*
- [Notion (App)](https://www.notion.so/product) - Read and write Notion pages and databases from your app. *Use case: Knowledge-base-driven apps, internal wikis, or runtime content sourced from a team's Notion workspace — distinct from the chat-side Notion connector that only reads context during build.*
- [Storyblok](https://www.storyblok.com) - Headless CMS and visual page builder. *Use case: Visual-editor-friendly content management for content-heavy Lovable apps where non-developers will edit copy and layout.*
- [WordPress.com](https://wordpress.com) - Access your WordPress.com sites, posts, and media. *Use case: Surfacing WordPress.com posts inside a Lovable app, syndicating app-generated content to a WordPress blog, or building authoring tools over an existing WordPress.com site.*

## CRM, Sales, and Recruiting

- [Ashby](https://www.ashbyhq.com) - Recruiting and applicant tracking system. *Use case: Custom recruiter dashboards, candidate pipeline views, or interviewer-feedback tools built on top of a company's Ashby ATS.*
- [Attention](https://www.attention.com) - Sales conversation intelligence and coaching API. *Use case: Pulling sales-call transcripts and coaching scorecards into a custom revenue dashboard, or surfacing conversation insights inside a sales-ops Lovable app.*
- [HubSpot](https://www.hubspot.com) - CRM platform for sales, marketing, and customer service. *Use case: Reading and writing CRM records — contacts, deals, tasks — from a Lovable app to extend HubSpot with custom workflows or internal tooling.*
- [Salesforce](https://www.salesforce.com) - CRM platform for sales, service, and marketing. *Use case: Reading and writing Salesforce records — accounts, opportunities, cases — from a Lovable app to build custom CRM dashboards, internal sales tooling, or customer portals over an organization's Salesforce data.*

## Project Management

- [Asana](https://asana.com) - Work management platform for tasks, projects, and teams. *Use case: Surfacing project state inside an internal tool, creating tasks from app events, or building bespoke views over Asana data.*
- [Linear](https://linear.app) - Project management and issue tracking for software teams. *Use case: Engineering dashboards, custom triage views, or wiring app events into Linear issues from a Lovable app.*

## Data and Analytics

- [Airtable](https://airtable.com) - Spreadsheet-database hybrid and automation platform. *Use case: Using Airtable as a friendly backend for low-to-medium-scale apps where non-developers will edit underlying records.*
- [Google Search Console](https://search.google.com/search-console) - Read search analytics and manage sites in Google Search Console. *Use case: SEO analytics dashboards, content-performance views, or surfacing indexing state inside a marketing-ops Lovable app.*
- [BigQuery](https://cloud.google.com/bigquery) - Query and analyze data in BigQuery. *Use case: Powering analytics dashboards or AI features over warehouse-scale data without standing up a separate query layer.*
- [Databricks](https://www.databricks.com) - Unified analytics and AI platform. *Use case: Surfacing notebook-driven models, lakehouse query results, or ML pipeline output inside a Lovable app for non-technical users.*
- [Semrush](https://www.semrush.com) - Keyword research, domain analytics, backlinks, paid-search data, and position tracking. *Use case: SEO dashboards, keyword-research tools, competitor tracking, backlink monitoring, or client-facing search-performance reports inside a Lovable app.*
- [Snowflake](https://www.snowflake.com) - Cloud data platform for analytics and AI. *Use case: Building customer-facing analytics, internal BI tools, or data-product surfaces over a Snowflake account from a Lovable app.*

## Web Scraping

- [Firecrawl](https://www.firecrawl.dev) - AI-powered scraper, search, and retrieval tool. *Use case: Crawling sites, extracting structured data from web pages, or building search-augmented Lovable apps that need fresh page content.*

## Maps and Location

- [Google Maps Platform](https://mapsplatform.google.com) - Geocoding, routes, places, embedded maps, address validation, weather, and air quality APIs. *Use case: Adding map-driven features to a Lovable app — store locators, route planning, address autocomplete, location-aware automations, or geospatial dashboards. Managed by Lovable or BYO Google Cloud credentials.*

## Meeting Intelligence

- [Fireflies](https://fireflies.ai) - Meeting transcription and conversation intelligence. *Use case: Pulling meeting transcripts into a Lovable app for summarization, action-item extraction, or building a searchable meeting archive.*

## Workflow Automation

- [Inngest](https://www.inngest.com) - Event-driven durable functions, background jobs, and workflows. *Use case: Long-running background work — webhooks, scheduled jobs, multi-step workflows — that the Lovable app frontend triggers but shouldn't block on.*

## Security

- [Aikido](https://www.aikido.dev) - AI-powered security scanning and pentesting. *Use case: Embedding security findings (SAST, DAST, container scans, AI pentests) in an internal security dashboard built with Lovable, or routing Aikido alerts into custom triage flows.*
- [Wiz](https://www.wiz.io) - Cloud security platform and posture management. *Use case: Surfacing cloud-security posture findings, attack-path graphs, or compliance state inside a Lovable-built executive or platform-engineering dashboard.*

## Media and Streaming

- [LinkedIn](https://www.linkedin.com) - Read profile data and publish posts through LinkedIn's API. *Use case: Building a social-publishing tool that posts updates to LinkedIn from a Lovable app, or surfacing a user's profile and post metrics in a personal-brand or recruiting dashboard.*
- [TikTok](https://www.tiktok.com) - Read profile information, follower counts, like counts, video statistics, and published video metadata. *Use case: Creator-analytics dashboards, social-listening tools, or campaign-reporting surfaces that ingest TikTok account data into a Lovable app — read-only, no publishing.*
- [Twitch](https://www.twitch.tv) - Live streaming platform for gaming and creative content. *Use case: Building creator-tools, channel-overlay apps, or stream-state dashboards on top of a streamer's Twitch account.*

## Chat Connectors

MCP servers attached to your Lovable build session. Add live context while you build — only available to you, not to the apps you ship.

## Product Analytics

- [Amplitude](https://amplitude.com) - Access your Amplitude product analytics and feedback. *Use case: Asking the chat surface to ground UI decisions in real funnel data, retention curves, or feature-adoption metrics from your Amplitude project.*
- [Hex](https://hex.tech) - Access your Hex data notebooks and projects. *Use case: Pulling notebook-derived metrics or query results into a Lovable build session to inform what you're shipping.*
- [PostHog](https://posthog.com) - Access your PostHog analytics, feature flags, and experiments. *Use case: Letting the chat surface reference event volume, funnel drop-offs, or active experiments while you iterate on the product.*

## Project Management and Knowledge

- [Atlassian](https://www.atlassian.com) - Access your Jira issues and Confluence pages. *Use case: Grounding what you build in real Jira ticket scope or Confluence specs without copy-pasting requirements into chat.*
- [Linear (Chat)](https://developers.linear.app) - Access your Linear issues and project data. *Use case: Asking the chat surface to read the actual ticket you're working from, including comments and acceptance criteria, while you build.*
- [Notion](https://www.notion.so) - Access your Notion pages and databases. *Use case: Pulling design briefs, PRDs, or roadmap pages from Notion into a build session — the spec stays in Notion, the implementation reads it live.*

## A/B Testing and Feature Flags

- [Confidence Exp](https://confidence.spotify.com/experiments) - Analyze your Confidence A/B tests and rollouts. *Use case: Letting Lovable read live experiment results from Spotify's open Confidence platform when building variants or rollout-aware UI.*
- [Confidence Flags](https://confidence.spotify.com/flags) - Create, modify, and manage your Confidence feature flags. *Use case: Wiring new code paths to Confidence feature flags during the build itself — no separate console-tabbing to set up flag rules.*

## Design and Whiteboarding

- [Figma](https://www.figma.com) - Use Figma's local MCP server from Figma Desktop on your machine. *Use case: Generating components from a Figma file's actual layers, tokens, and styles instead of describing the design in prose.*
- [Miro](https://miro.com) - Access your Miro boards and diagrams. *Use case: Reading product flows or system diagrams off a Miro board into the build context — architecture-aware code generation grounded in the team's whiteboard.*

## Content Management (Chat)

- [Sanity](https://www.sanity.io) - Access your Sanity content management. *Use case: Reading actual content schemas and entries from a Sanity project so generated UI matches the real data shape, not a guessed one.*

## Meeting Intelligence (Chat)

- [Granola (Chat)](https://docs.granola.ai) - Access your meeting notes and transcripts. *Use case: Pulling decisions, follow-ups, or quotes from a recent customer call directly into the build session — what got asked for in the meeting becomes input to what you ship.*

## AI Video

- [HeyGen](https://www.heygen.com) - Create AI videos, avatars, and translate content. *Use case: Generating product demo videos, localized voiceovers, or avatar-driven walkthroughs as part of the build session — marketing assets that ship with the app.*

## Workflow Automation (Chat)

- [n8n](https://n8n.io) - Access and power your apps with your n8n workflows. *Use case: Letting the chat surface read or trigger n8n workflows during the build — the workflow engine stays in n8n, Lovable wires app actions to it.*

## Billing (Chat)

- [Polar](https://polar.sh) - Set up subscription billing. *Use case: Wiring digital-product or subscription billing into a Lovable app via Polar's open-source merchant-of-record platform — pricing, checkout, and access management without rolling your own billing.*

## Error Tracking and Monitoring

- [Sentry](https://sentry.io) - Access your Sentry issues, errors, and project insights. *Use case: Reading live production errors into the build session so the next iteration fixes what's actually breaking, not what you remember last seeing.*

## Custom MCP Servers

Lovable's chat surface includes a **New MCP server** entry — connect any custom MCP-compliant server to add your own context source to the build session. See the [Model Context Protocol specification](https://modelcontextprotocol.io) for building or hosting your own.

## Contributing

Contributions are welcome — see [CONTRIBUTING.md](CONTRIBUTING.md) for the submission flow, surface conventions (App vs Chat), and the entry style guide. By contributing you agree to the [Code of Conduct](code-of-conduct.md).
