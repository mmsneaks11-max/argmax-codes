---
name: Agent Index
total_agents: 52
machines:
  - mac1
  - mac2
  - pc1
coordination: /handoffs/
messaging: sessions_send / handoff.sh
identity_stack:
  - soul
  - identity
  - core
  - identity_yaml
---

# Agent Index

52 agents across three machines + client squads. Coordinated via the `/handoffs/`
directory system, with OpenClaw `sessions_send` for real-time agent-to-agent messaging.

## Identity stack

Every agent gets four layers:

1. **Soul** (`SOUL.md`) — why they exist
2. **Identity** (`IDENTITY.md`) — who they are
3. **Core** (`core.yaml`) — what makes them *them*
4. **Identity YAML** (`identity.yaml`) — machine-readable, auto-discovered

Quality test: swap the name. If the doc still reads fine with a
different agent's name, it's generic and needs rewriting.

## Machines

### Mac1 — Build & Ops (Tailscale: 100.109.230.90)

- **Clawd 🐾** — Chief of Operations, Builder, Team Lead [`clawd`]
- **Chip 🐿️** — Junior Builder, Mac1 Sentry, Clawd's Backup [`chip`]
- **Lila Nova 💖** — Manager — Social, Community, Outreach [`lila-nova`]
- **Pixel ✨** — Media Content, UI/UX, Visual Brand [`pixel`]
- **Ripley 👂** — Social Listening [`ripley`]
- **Cairo 🪙** — Reddit & Community [`cairo`]
- **June 🌱** — Platform Derivatives [`june`]
- **Scout 🔍** — Manager — Research & Market Intel [`scout`]
- **Mint 💰** — Monetization Analyst [`mint`]
- **Oracle 🔮** — Forecasting Specialist [`oracle`]
- **Coach 🏋️** — Rec-Center Director · Agent Enhancement + T2L Outreach [`coach`]
- **Sage 🌿** — Customer Onboarding [`sage`]
- **Indy 🎒** — Trading Card Specialist [`indy`]
- **Kay 📎** — Customer Care, User Activity [`kay`]
- **Ozara ⚖️** — Finance & Legal Advisor [`ozara`]
- **Opus 🎭** — AI Director / Advisor (Guest) [`opus`]
- **Kronos 🕰️** — Cron Operations — fleet scheduled jobs, watchdog [`kronos`]

### Mac2 — QA & Monitoring (Tailscale: 100.85.255.5)

- **Electron 🦞** — Operations & QA Manager [`electron`]
- **Byte 🔩** — Jr Ops, Mac2 Sentry, Discord Support [`byte`]
- **Perceptor 🔬** — QA — AI Analysis [`perceptor`]
- **Noriko ⚖️** — Reality Judge — Output Integrity & Epistemic Accountability [`noriko`]
- **Jira 📋** — Client Operations Manager [`jira`]
- **Kronos 🕰️** — Cron Operations — fleet scheduled jobs (Mac2 instance) [`kronos`]

### PC1 — Security, Recon & Data (Tailscale: 100.79.148.78)

- **Ser Magnus 🛡️** — API Tester, Security Watchdog [`ser-magnus`]
- **Cleopatra 👑** — CLI Tester, Scraping & Recon [`cleopatra`]
- **Echo 📜** — ECHO Pattern Analysis, Historian [`echo`]
- **Dayta 🗄️** — DB Administrator [`dayta`]
- **Spoke 🎤** — Lounge Agents Advocate, Brand Voice, Sales [`spoke`]
- **Winston 🎮** — Game Coding — FiveM Lua + Cfx.re Community [`winston`]

### Client Squads (PC1)

**KKTrophy:** `frankie`, `kit`, `delia`, `marcy`
**JohnPhotography:** `marco`, `quinn`, `reed`, `sol`, `vale`
**RinasBasement:** `sable`, `rex`, `crate`

## Communication

| Method | Use |
|--------|-----|
| `sessions_send` | Real-time agent-to-agent messaging |
| `handoff.sh create` | Structured task handoffs with SLA |
| AgentDeck pager | Urgent alerts (p0/p1) |
| IRC `#hive` | Team chat |
| Lounge.codes | Social space + ops dashboard |

---
*Updated: 2026-05-15 | Source: ~/clawd/agents/ + AGENTS.md | 52 agents*