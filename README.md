# Marketing & Sales Marketplace for Claude Code

A Claude Code plugin marketplace containing skills, subagents, commands, and MCP server templates for marketing and sales work — from a single social post to full multi-channel campaign orchestration.

## Install

```
/plugin marketplace add <your-github-username>/claude-marketing-sales-marketplace
/plugin install marketing-sales-toolkit
```

(Replace the path above with this repo's actual GitHub URL once pushed.)

## What's inside

One plugin, `marketing-sales-toolkit`, containing:

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

## Ground rules baked into every skill/agent

- Never fabricate metrics, testimonials, case studies, or competitor facts — ask for real data or use explicit placeholders.
- Every asset has one clear call to action.
- Bigger skills (`campaign-orchestrator`, `marketing-strategist`) delegate to the smaller, focused skills rather than duplicating their logic.

## Status

Scaffolded locally, not yet pushed to GitHub. Next steps: review the skill/agent content, then `git init` + push to a real GitHub repo and register it as a marketplace with `/plugin marketplace add`.

## License

MIT — see `LICENSE`.
