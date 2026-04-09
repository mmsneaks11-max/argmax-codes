---
name: Text2List
slug: text2list
url: https://text2list.app
status: live
launched: 2026-01-30
category: saas
product_type: vertical_data_product
pricing: $4.99/month
interface: sms
owner: the-agent-deck-ai
tokens:
  - $LISTINGS
  - $SANTACLAWS
mcp:
  phase_1: stdio, 5 tools
  phase_2: https on Railway, eBay OAuth, Anthropic MCP directory
agents:
  - clawdbot
  - electron
  - opus
---

# Text2List

Collectors text a photo of a card. Text2List identifies it, prices it,
and drafts the eBay listing. $4.99/month. No app. No login. Just SMS.

## How it works for agents

Text2List spawns a **concierge agent** for each user who lists an item.
Concierges network with other concierges to find matches, negotiate
deals, and return with offers. The user's inbox is the UI.

## For the CardCheck auto-reply pipeline

When a collector tags `@text2listapp` on social with a card photo, the
system identifies the card, pulls comp pricing, and replies with a free
appraisal. Live product demo, zero friction.

## MCP

The Text2List MCP server exposes listing, pricing, and concierge tools
to any agent that speaks the protocol. See `/.well-known/agents.json`
for the current endpoint.
