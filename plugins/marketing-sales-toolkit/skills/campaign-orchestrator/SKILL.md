---
name: campaign-orchestrator
description: Plan and coordinate a full multi-channel marketing/sales campaign end to end — positioning, funnel, channel mix, content calendar, sales enablement, and success metrics. Use for a full product launch, quarterly campaign, or GTM push spanning multiple channels and teams. Difficulty: Extreme.
---

# Multi-Channel Campaign Orchestrator

This is the top-of-stack skill — it composes the other skills in this plugin rather than replacing them. Use it to plan a full campaign, then hand individual assets off to the narrower skills (`landing-page-copy`, `cold-outreach-sequence`, `social-post-writer`, `seo-content-brief`, `email-subject-optimizer`) or to the `marketing-strategist` / `sales-copywriter` / `seo-specialist` / `competitive-analyst` agents for execution.

## Inputs to gather
- Campaign goal and target metric (pipeline generated, signups, revenue, awareness)
- Launch date / timeline and budget constraints, if any
- Target segment(s) and any existing positioning/messaging to build on
- Available channels (paid, organic social, email/CRM list, sales outbound, partnerships, PR)
- Team/resource constraints (who executes what)

## Process
1. **Positioning pass**: confirm or draft the core message and proof points for this campaign — do not proceed to channel content until this is agreed, since every asset downstream depends on it.
2. **Funnel map**: for each stage (awareness → consideration → conversion → retention), name the channel(s) and the one asset needed at that stage.
3. **Channel plan**: for each selected channel, specify cadence, owner, and which narrower skill/agent produces the asset (e.g., "Week 1 LinkedIn posts → `social-post-writer`", "Outbound sequence → `cold-outreach-sequence`").
4. **Content calendar**: a week-by-week table of what ships, on which channel, and its dependency (e.g., landing page must ship before ads can point to it).
5. **Sales enablement**: if sales is involved, produce a one-page battlecard and talking points (reuse `competitor-teardown` output if available).
6. **Measurement plan**: define the metrics per funnel stage and how they'll be tracked — flag when the user needs an MCP/analytics connection (see `mcp/` configs in this plugin) rather than assuming data access you don't have.
7. **Risk/dependency check**: call out anything that blocks the timeline (legal review, design assets, integration not yet built) before declaring the plan ready.

## Rules
- Never invent budget numbers, team names, or tool access — ask if not given.
- This skill produces a *plan*; it should explicitly delegate copywriting to the narrower skills rather than writing all assets inline, so each asset stays focused and reviewable on its own.
- Surface conflicts (e.g., two channels competing for the same week's design bandwidth) instead of silently smoothing over them.
