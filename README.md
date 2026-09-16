# Marketing & Sales Marketplace for Claude Code

A Claude Code plugin marketplace containing skills, subagents, commands, and MCP server templates for marketing and sales work — from a single social post to full multi-channel campaign orchestration.

## Install

```
/plugin marketplace add RajaC1/Marketing-Sales
/plugin install marketing-sales-toolkit
/plugin install ecc-marketing-sales-extras
```

## What's inside

Two plugins.

### Plugin 1: `marketing-sales-toolkit` (original content)

### Skills (`plugins/marketing-sales-toolkit/skills/`)

| Skill | Difficulty | What it does |
|---|---|---|
| `social-post-writer` | Basic | Platform-native social posts (LinkedIn, X, Instagram, Facebook) |
| `email-subject-optimizer` | Basic | Generates and ranks email subject lines + preview text |
| `brand-voice-guide` | Basic | Builds or applies a brand voice/tone guide |
| `cold-outreach-sequence` | Intermediate | Multi-touch cold email/LinkedIn prospecting sequences |
| `landing-page-copy` | Intermediate | Full landing page copy: hero, benefits, proof, FAQ, CTA |
| `seo-content-brief` | Intermediate | Keyword-targeted SEO content briefs with outline and intent |
| `competitor-teardown` | Advanced | Structured competitor positioning/pricing/messaging analysis |
| `pricing-page-audit` | Advanced | Conversion-focused audit of a pricing page or model |
| `ab-test-analyzer` | Advanced | Statistical validity check and interpretation of A/B test results |
| `campaign-orchestrator` | Extreme | Full multi-channel campaign plan — positioning through measurement, delegating to the skills above |

### Agents (`plugins/marketing-sales-toolkit/agents/`)

| Agent | Difficulty | What it does |
|---|---|---|
| `sales-copywriter` | Intermediate | Writes all sales-facing copy (outreach, follow-ups, battlecards) |
| `seo-specialist` | Intermediate | SEO content and technical strategy |
| `competitive-analyst` | Advanced | Competitor research and battlecards, sourced only from real material |
| `marketing-strategist` | Extreme | End-to-end campaign planning and coordination across the whole plugin |

### Commands (`plugins/marketing-sales-toolkit/commands/`)

- `/campaign-kickoff` — gathers campaign inputs and runs the `campaign-orchestrator` skill.

### MCP server templates (`plugins/marketing-sales-toolkit/mcp/`)

Copy-paste `.mcp.json` templates (no credentials included) for HubSpot, Google Analytics, and SendGrid — see `mcp/README.md`.

### Plugin 2: `ecc-marketing-sales-extras` (vendored, MIT-licensed)

Additional skills/agents/command copied from the [ecc marketplace](https://github.com/affaan-m/ECC) (MIT license, Copyright (c) 2026 Affaan Mustafa). Full attribution and file list in `plugins/ecc-marketing-sales-extras/NOTICE.md`.

| Skill | What it does |
|---|---|
| `brand-discovery` | Discovers and documents brand identity fundamentals |
| `brand-voice` | Defines a brand's tone/voice for content generation |
| `competitive-platform-analysis` | Analyzes a competitor's product/platform |
| `competitive-report-structure` | Structures a competitive analysis report |
| `content-engine` | Platform-native content for X, LinkedIn, TikTok, YouTube, newsletters |
| `crosspost` | Adapts one piece of content across multiple platforms |
| `email-ops` | Email sending/operations workflows |
| `growth-log` | Tracks growth experiments and outcomes |
| `lead-intelligence` | Lead scoring/enrichment logic |
| `mailtrap-email-integration` | Mailtrap email testing/integration |
| `market-research` | Market sizing and research methodology |
| `marketing-campaign` | Full campaign brief → assets across channels |
| `seo` | Technical SEO audits and on-page optimization |
| `social-graph-ranker` | Ranks/analyzes social graph data |
| `social-publisher` | Publishes content to social platforms |
| `x-api` | X (Twitter) API usage patterns |
| `article-writing` | Long-form article/blog writing |
| `investor-materials` | Investor-facing decks and materials |
| `investor-outreach` | Investor outreach sequences |
| `customer-billing-ops` | Billing/subscription operational workflows |

Agents: `marketing-agent`, `ecc-seo-specialist` (renamed from upstream `seo-specialist` to avoid colliding with this repo's own agent of the same name). Command: `/marketing-campaign`.

## Related marketplaces (not vendored)

- **[Clay](https://github.com/clay-run/agent-plugins)** — Clay's official GTM/sales data-enrichment plugin (audiences, outbound sequencing, CRM-table workflows). Not copied into this repo because its source repo has no LICENSE file; install it directly instead: `/plugin marketplace add clay-run/agent-plugins`.

## Ground rules baked into every skill/agent

- Never fabricate metrics, testimonials, case studies, or competitor facts — ask for real data or use explicit placeholders.
- Every asset has one clear call to action.
- Bigger skills (`campaign-orchestrator`, `marketing-strategist`) delegate to the smaller, focused skills rather than duplicating their logic.

## License

`marketing-sales-toolkit` is original content, MIT — see `LICENSE`.
`ecc-marketing-sales-extras` is vendored MIT content from ecc — see `plugins/ecc-marketing-sales-extras/NOTICE.md` and `LICENSE-ecc-upstream.txt`.
