# Ergon Automation Labs — Public View

This repo is a live window into the build progress of [Bot Army](https://github.com/ergon-automation-labs), a personal operating system for attention management built on Elixir/BEAM, NATS, SaltStack, and a push/pull surface philosophy.

It exists because the work is worth showing, and because shipping in public is more honest than a polished portfolio page.

---

## What You're Looking At

**[PROJECT_PROGRESS.md](./PROJECT_PROGRESS.md)** is a running engineering log — updated per session, per release, and per milestone. It tracks:

- Active bot status, version, and completion percentage
- What shipped in each session (with test counts and NATS subjects)
- What's pending and why
- Infrastructure decisions and their reasoning
- Blockers, risks, and how they were resolved

It reads like an internal engineering document because it is one. That's intentional.

---

## The System at a Glance

Bot Army is a 45+ repo distributed system organized around one idea:

> *Attention is finite. Information shouldn't have to be.*

Information is routed to the right surface at the right moment:

| Surface | Mode | Examples |
|---|---|---|
| Apple Watch · AR Glasses | Push / interrupt | P0 alerts, urgent nudges |
| LiveView dashboard · Terminal TUI | Pull / consult | GTD, SRE status, job tracking |

Every bot communicates via NATS. Every service boundary is a JSON Schema contract. The deployment chain runs Salt → Jenkins → NATS → surface.

---

## Current Status (as of March 2026)

| Bot | Version | Status |
|---|---|---|
| bot_army_llm | 0.6.2 | ✅ Production |
| bot_army_gtd | 0.2.0 | ✅ Production |
| bot_army_advocacy | 0.1.2 | ✅ Production |
| bot_army_job_applications | 0.2.14 | ✅ Production |
| bot_army_chore | 0.1.4 | ✅ Production |
| bot_army_fitness | 0.1.4 | ✅ Production |
| bot_army_terrain | 0.1.2 | ✅ Production |
| bot_army_email_triage | 0.1.0 | ✅ Production |
| bot_army_sre | 0.1.0 | 🟡 Phase 3 |
| bot_army_context_broker | 0.1.0 | ✅ Released |
| bot_army_notification_router | 0.1.0 | ✅ Released |

---

## How This Gets Updated

Progress is exported here at the end of meaningful sessions — new releases, completed phases, resolved blockers. It's maintained with AI assistance (Claude) and reflects real work, not aspirational roadmaps.

The goal is automation: eventually a progress bot watches commits and NATS events and pushes updates here directly. For now, it's human-in-the-loop.

---

## More

- **Org home:** [github.com/ergon-automation-labs](https://github.com/ergon-automation-labs)
- **Builder:** [github.com/the-great-abby](https://github.com/the-great-abby)
- **LinkedIn:** [linkedin.com/in/abbymalson](https://www.linkedin.com/in/abbymalson/)

---

<sub>Ergon Automation Labs · Denver, CO</sub>
