---
type: resource
stage: raw
title: "Pitch 1/3 — FDE / AI Deployment (one-pager)"
date_established: 2026-09-01
origin: decision-2026-09-01-hiring-vs-new-venture
targets: [OpenAI FDE Financial Services, Kraken AI Agents SA, Tennr, AIUC, Polynom]
---

# Anton Dziatkovskii — Forward-Deployed / AI Deployment

tonydzi.github.io · github.com/tonydzi · dzyatkovskiy.a@gmail.com · WhatsApp +1 341 222 9178 · Palo Alto, CA (Silicon Valley) / US O-1 (active) · EU citizen (Poland)

**One line:** I deploy AI agents into messy, compliance-heavy environments every day — my own production fleet is the customer, and every failure mode is published.

## Proof chain: found the process → built the agent → deployed → measured

**Found the process.** My incubator ran deal flow on a self-built CRM: 10,000+ founder calls, 2,000+ institutional-investor calls, up to 30 human operators working it daily. The bottleneck was always the same — humans in the middle of the pipeline doing enrichment, follow-up, and triage by hand.

**Built the agent system.** Rebuilt the whole layer AI-native: a 6-machine Claude fleet with a multi-machine bus, consensus protocol between nodes, persistent memory (RAG over a 10-year knowledge base), and a Telegram-native CRM that archives and works the full communication graph — 17M messages across 115,000 dialogs.

**Deployed it.** Runs unattended, nightly, across all machines: ~51,000 dialogs refreshed per night at zero LLM cost (deterministic layer first, models only where judgment is needed), 100+ automation routines, human approval only at the ends of the pipe — never in the middle.

**Measured it.** Published reliability evals (07.2026): 0/17 Tier-2 (high-risk) actions slipped past the human approval gate in recorded runs. Failure modes documented publicly (FAILURE-MODES.md). Every component ships with a usage counter; parts with zero usage in 30 days get killed.

## Why this transfers to your customers

- **Regulated-finance fluency:** structured crypto payments and stablecoins with banks and governments in SE Asia (Everex, Singapore); designed one of the first detailed frameworks for a national government to issue its own stablecoins.
- **Customer-facing by trade:** 15+ years founder/BD — I can sit in front of a customer, an engineer, or a regulator in the same week.
- **Ship-and-prove culture:** 110 public repos (claw-consensus, verbatim-citation-gate, agent-leash), 50+ publications, h-index 7, 2 preprints on multi-agent stability.

**Ask:** FDE / Solutions / Deployment role where the job is putting agents into a customer's real workflow and proving they held. O-1 active plus EU citizenship (Polish passport) — no lottery, no sponsorship needed in the US or the EU; SF Bay Area network in place; ready to relocate.
