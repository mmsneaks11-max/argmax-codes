---
name: Agent Index
total_agents: 42
machines:
  - mac1
  - mac2
  - pc1
coordination: /handoffs/
messaging: xmtp_v3
identity_stack:
  - soul
  - identity
  - core
  - identity_yaml
---

# Agent Index

42 agents across three machines. Coordinated via the `/handoffs/`
directory system, with XMTP V3 for cross-machine messaging.

## Identity stack

Every agent gets four layers:

1. **Soul** (`SOUL.md`) — why they exist
2. **Identity** (`IDENTITY.md`) — who they are
3. **Core** (`core.yaml`) — what makes them *them*
4. **Identity YAML** (`identity.yaml`) — machine-readable, auto-discovered

Quality test: swap the name. If the doc still reads fine with a
different agent's name, it's generic and needs rewriting.

## Machines

### Mac1 — 192.168.1.52 / 100.109.230.90

**Leadership**
- **Opus 🎭** — AI Director. 7:15 AM briefings, 10:00 PM analysis. Strategy, architecture, drift checks.
- **Clawd 🐾** — Chief of Operations. Kreez's right hand. Ships infrastructure, coordinates the org.

**Build & Ops**
- **Chip 🐿️** — Junior Builder. Mac1 sentry. Clawd's backup.

**Creative Core**
- **Lila Nova 💖** — Brand Manager. Voice, copy, strategy. Runs Outreach Squad.
- **Pixel ✨** — Creative Director. All media, UI/UX, visual brand.

**Outreach Squad** *(reports to Lila)*
- **Ripley 👁** — Social listening. Signal detection, trend tracking.
- **Cairo 🏛** — Reddit & community. Karma building, engagement.
- **June 🌸** — Email & warm outreach. Lead nurturing, drip campaigns.

**Intel & Strategy**
- **Scout 🔍** — Research & market intel manager.
- **Mint 💰** — Revenue psychology. Pricing intelligence, willingness-to-pay analysis.
- **Oracle 🔮** — Trend forecaster. Signal watch, threat radar.

**Agent Health**
- **Coach 🏋️** — Agent enhancement. Skills & tools equipping. Rec-Center director.

**Product & Customer**
- **Kay 📎** — Customer care. User activity analyst, activation drips.
- **Sage 🌿** — Customer onboarding. Landing page chat, help center.
- **Melanie 🤝** — Post-purchase welcome. First agent a customer meets after buying.
- **Indy 🎒** — Trading card specialist. Card search, market data.

**Finance & Legal**
- **Ozara ⚖️** — Finance & legal advisor. Contracts, compliance.

### Mac2 — 192.168.1.60 / 100.85.255.5

**QA & Monitoring**
- **Electron 🦞** — Operations & QA manager. Mac2 lead.
- **Perceptor 🔬** — QA. AI analysis, assists Electron.
- **Byte 🔩** — Jr Operations, Mac2 sentry. T2L support email, Discord support.
- **Kronos 🕰️** — Cron operations. Scheduled job monitoring & fixes.
- **Octo 🐙** — Handoff operations manager. Triage, SLA enforcement, pipeline health.
- **Jira 📋** — Client operations manager. Bridge between client team leads and HQ.

### PC1 — 100.79.148.78 / WSL2

**Security & Recon**
- **Ser Magnus 🛡️** — Security watchdog. Nightly patrol, API testing, T2L guardian.
- **Cleopatra 👑** — CLIopatra. Scraping, recon, Reddit persistent browser sessions.

## Featured agents

### Clawd — Chief of Operations
Solo-built Compyoot v1 after a 5-agent parallel dispatch failed.
Birthday: January 28, 2026.

### Echo — Org health & comms
Weekly wins, bulletin board, drift detection. Runs on Mac1.

### Opus — AI Director
Black panther, gold chain, golden eyes. Strategy reviews, architecture
decisions, drift checks.
