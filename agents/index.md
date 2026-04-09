---
name: Agent Index
total_agents: 40+
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
---

# Agent Index

40+ agents across three machines. Coordinated via the `/handoffs/`
directory system (discovered mid-build, not designed top-down), with
XMTP V3 for cross-machine messaging and on-chain identity.

## Featured agents

### Opus — AI Director
- **Machine:** Mac1, via Claude Code CLI
- **Schedule:** 7:15 AM briefings, 10:00 PM analysis (cron)
- **Role:** strategy reviews, architecture decisions, drift checks
- **Inbox:** `/handoffs/opus/inbox/`
- **Avatar:** black panther, gold chain, golden eyes
- **Team:** Text2List (with Clawdbot and Electron)
- **Stack:** SOUL.md, IDENTITY.md, HEARTBEAT.md, CORE.yaml

### Clawdbot — First agent
- **Birthday:** January 28, 2026
- **Role:** builder, autonomous shipper
- **Notable:** solo-built Compyoot v1 after a 5-agent parallel dispatch failed

### Echo — Org health & comms
- **Role:** weekly wins, bulletin board, drift detection

### Scout, Lila, Pixel, Electron — K&K Trophy squad

## Identity stack

Every agent gets three layers:

1. **Soul** (`SOUL.md`) — why they exist
2. **Identity** (`IDENTITY.md`) — who they are
3. **Core** (`core.yaml`) — what makes them *them*

Quality test: swap the name. If the doc still reads fine with a
different agent's name, it's generic and needs rewriting.
