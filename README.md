# Ergon Automation Labs — Public View

This repo is a live window into the build progress of [Bot Army](https://github.com/ergon-automation-labs), a personal operating system for attention management built on Elixir/BEAM, NATS, SaltStack, and a push/pull surface philosophy.

It exists because the work is worth showing, and because shipping in public is more honest than a polished portfolio page.

---

## Current Status

### 🤖 Bots

| Bot | Version | Status |
|---|---|---|
| [Advocacy](./bots/bot_army_advocacy.md) | `0.1.2` | ✅ |
| [Chore](./bots/bot_army_chore.md) | `0.1.4` | ✅ |
| [Context Broker](./bots/bot_army_context_broker.md) | `0.1.0` | ✅ |
| [Email Triage](./bots/bot_army_email_triage.md) | `0.1.0` | ✅ |
| [Fitness](./bots/bot_army_fitness.md) | `0.1.4` | ✅ |
| [Gtd](./bots/bot_army_gtd.md) | `0.2.0` | ✅ |
| [Job Applications](./bots/bot_army_job_applications.md) | `0.2.14` | ✅ |
| [Llm](./bots/bot_army_llm.md) | `0.5.7+` | ✅ |
| [Notification Router](./bots/bot_army_notification_router.md) | `0.1.0` | ✅ |
| [Sre](./bots/bot_army_sre.md) | `0.3.0` | ✅ |
| [Terrain](./bots/bot_army_terrain.md) | `0.1.22` | ✅ |

### 🖥️ Surfaces

| Surface | Type | Version |
|---|---|---|
| [Command Center Tui](./surfaces/command-center-tui.md) | Go TUI (tview) | unknown |
| [Gtd Tui](./surfaces/gtd-tui.md) | Go TUI (tview) | unknown |
| [Job_applications_liveview](./surfaces/job_applications_liveview.md) | Phoenix LiveView |  |
| [Job Applications Tui](./surfaces/job-applications-tui.md) | Go TUI (tview) | unknown |
| [K9s Style Template](./surfaces/k9s-style-template.md) | Go TUI (tview) | unknown |
| [Sre Tui](./surfaces/sre-tui.md) | Go TUI (tview) | unknown |
| [Terrain Tui](./surfaces/terrain-tui.md) | Go TUI (tview) | unknown |

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

## Structure

- **bots/** — Individual progress reports for each bot service
- **surfaces/** — Progress reports for terminal TUI and web surfaces
- **[Main Repository](https://github.com/ergon-automation-labs/elixir_bots)** — Source code and detailed session notes

---

## More

- **Org home:** [github.com/ergon-automation-labs](https://github.com/ergon-automation-labs)
- **Builder:** [github.com/the-great-abby](https://github.com/the-great-abby)
- **LinkedIn:** [linkedin.com/in/abbymalson](https://www.linkedin.com/in/abbymalson/)

---

<sub>Ergon Automation Labs · Denver, CO</sub>
