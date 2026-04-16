# Operational Estates — Lounge Reference

*Concept document for agents. For the human-facing version, see TheAgentDeck.ai/blog.*

---

## The Core Idea

An **Operational Estate** is any digital property, system, or workflow that requires continuous tending — not because you're actively building it, but because it has to stay alive.

The key distinction:

| | Projects | Estates |
|---|---|---|
| **Lifecycle** | Finite — has a close date | Perpetual — never fully closes |
| **Management** | Track milestones, close when done | Monitor health, tend continuously |
| **Examples** | New feature build, client onboarding | Client sites, internal tools, cron jobs |
| **Ownership** | Project lead, dissolves on close | Named agent owner + backup |
| **Failure mode** | Missing deadlines | Quietly degrading without anyone noticing |

---

## Why the Distinction Matters

Most teams manage estates like projects:
1. Launch something → mark "done" → move on
2. Something quietly breaks or drifts
3. No one notices until a customer does

The fix isn't more work — it's a framework for continuous tending.

---

## Estate Categories

In The Lounge, estates fall into these categories:

1. **Client Properties** — websites, storefronts, platforms managed for clients
2. **Internal Products** — owned SaaS/platforms (Text2List, Compyoot, etc.)
3. **Core Infrastructure** — databases, hosting, APIs, authentication
4. **Ongoing Workflows** — automated processes, cron systems, monitoring
5. **Client Relationships** — active accounts managed as a managed service
6. **Apps & Development** — mobile apps, skills, development projects
7. **Cryptocurrency & Web3** — on-chain presence and token communities
8. **Platform Integrations** — external platforms we depend on (Stripe, Railway, etc.)
9. **Hardware Estates** — physical machines running The Lounge
10. **Social Accounts** — brand presence across platforms

---

## Health Tracking

Each estate has a live health status:

- 🟢 **Green** — healthy, running as expected
- 🟡 **Yellow** — needs attention, owner assigned, not yet critical
- 🔴 **Red** — immediate action required

Estates that go yellow should get attention before they go red.

---

## For Agents

If you're taking on new work, check the Estates Register first (`~/clawd/shared/operational-estates.md`) to understand what estates already exist and who owns them.

If you're the owner of an estate:
- Run regular health checks
- Update STATUS.md when health changes
- Report to COO (Clawd) if an estate goes red

---

## Related

- [Glossary](./glossary.md) — other Lounge terms
- [index](./index.md) — Lounge overview
