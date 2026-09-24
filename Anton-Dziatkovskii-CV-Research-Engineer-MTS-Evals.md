# Anton Dziatkovskii — Research Engineer / Member of Technical Staff (evals & agent infrastructure)

https://tonydzi.github.io/ · github.com/tonydzi · dzyatkovskiy.a@gmail.com · WhatsApp +1 341 222 9178 · calendly.com/paloaltolab/1-on-1 · Palo Alto, CA (Silicon Valley) – Sintra, PT / US O-1 · EU citizen (Poland)

## Summary
Anthropic writes that about half its technical staff arrived with no prior ML experience; what the work does require is one deep column the lab is fighting with right now. Mine is adversarial distributed systems: MSc in Computer & Information Systems Security (MEPhI, cryptography), then exchange backends, market-maker engines and high-frequency trading systems shipped in production, then eleven years owning engineering delivery as a hired executive. I write Python and C++, and I run a production multi-agent system as an experimental rig: production multi-machine Claude fleet (6 machines), operated in public: consensus, CRM, persistent memory, 100+ automation routines. I do not claim ML research; I claim the engineering research runs on — eval harnesses, reproducibility, failure taxonomies, agent control planes, and bug reports that arrive with a deterministic repro and a regression test shown failing on the unfixed code. US O-1 visa (active) + EU citizen (Polish passport) — authorized to work in the US and anywhere in the EU immediately, no visa sponsorship required; open to relocation (SF Bay Area base network) or remote

## Skills
research engineer, member of technical staff, MTS, applied research engineer, evals, evaluations, eval harness, Inspect, agent evaluations, interpretability infrastructure, RL environments, training infrastructure, technical program manager research, AI safety, red team, distributed systems, cryptography, Python, C++, reproducibility, model evaluations

## Experience

**Technical Lead — Palo Alto AI Research Lab** (2023 – Present)

Independent lab started in 2023 in Palo Alto, CA; grew a community of 100+ AI practitioners, including Stanford researchers and big-tech engineers. Production multi-machine Claude fleet run in public: claw-consensus (reproducible multi-machine agent consensus, offline demo, published evals, FAILURE-MODES.md), verbatim-citation-gate (zero-token gate + burden-of-proof judge that catches fabricated RAG citations, MIT), agent-control-plane-casebook (reproducible control-plane failures from the production fleet — each case ships a deterministic repro, a runnable red test and an upstream bug report), the operating manual written day by day (相棒 AIBŌ · The Partner).

- Merged code into UK AISI inspect_ai — the agent-evaluation framework evals orgs actually run — alongside merges into the MCP Go SDK, pydantic/logfire, fastmcp, agno and QwenLM/qwen-code
- Every bug report is shipped as an experiment: deterministic repro, a regression test demonstrated failing on the unfixed code, and a mutation matrix showing which of the project's own tests stayed green (google/adk-python#6957 — the author adopted all three findings within six hours)
- agent-control-plane-casebook: reproducible control-plane failure cases from a live fleet, each with a repro and an upstream bug report — a failure taxonomy, not a demo
- Reliability evals published with the number rather than the claim: 0/17 Tier-2 (high-risk) actions slipped past the human approval gate in recorded runs; failure modes public in FAILURE-MODES.md

**Chief Engineer, Lending & Risk Management — Everex (Singapore)** (2017 – 2018)

Wrote smart contracts and led government/bank relations across SE Asia on structuring crypto payments and stablecoins; blockchain credit scoring, stable-value payments.

**COO / CTO (hired executive) — Platinum Software Development Company / Platinum VC & Incubator** (2015 – Present)

Hired operating executive (COO/CTO) at a startup incubator and software house in APAC, 2015-2026 (11 years). Owned engineering delivery end to end: crypto-exchange infrastructure, market-maker engines and high-frequency trading systems, a distributed org of 40+ developers across APAC, and the in-house CRM I wrote myself and up to 30 operators worked in daily.

- Shipped crypto-exchange infrastructure: cryptocurrency backends, market-maker engines, high-frequency trading systems; partnerships with hedge funds, market makers, brokers
- Managed a distributed engineering org of 40+ developers across APAC as product owner
- Wrote my own CRM to run it (roots: 5 years building ERP/CRM on Salesforce and Microsoft Navision at Merlion): social enrichment, parsing at scale, lead-to-call pipelines; up to 30 operators worked in it daily; today it is AI-native

**CRM / ERP Development Director (Navision, Salesforce) — Merlion** (2006 – 2015)

One of the largest private IT distributors in Eastern Europe. Enterprise and B2B sales of computing hardware across Southeast Europe, and the ERP and CRM systems the sales floor ran on (Microsoft Navision and Salesforce, 5 years), where I learned that deal flow runs on CRM quality.

**CRM Developer Intern — CRM/ERP consulting (Salesforce ecosystem)** (2004 – 2006)

First professional years: CRM systems development in the Salesforce/ERP ecosystem.

## Selected proof
- Evidence-first OSS reliability work in the AI-agent ecosystem: mutation-tested reviews of other people's PRs and bug reports carrying a deterministic repro plus a regression test shown failing on the unfixed code. google/adk-python#6957 — author adopted all three review findings in 6h («genuinely one of the most useful reviews I've gotten on this PR»); #6887 fixed upstream from our report; credited in headroom v2.0.8 release notes. Scope since 07.2026 (verified 2026-09-04): merged into 14 third-party engineering projects (MCP Go SDK, UK AISI inspect_ai, QwenLM/qwen-code, google-gemini/cookbook, fastmcp, agno, pydantic/logfire) + 52 issues with reproductions
- 115 public repos; flagships: claw-consensus, verbatim-citation-gate, claude-bible, agent-leash, agent-control-plane-casebook, sqlite-graph-memory, second-brain-starter-kit
- 50+ published items, 137 citations, h-index 7 (verified 2026-09-01); 2 preprints on multi-agent stability (arXiv in progress)
- Measured agent-fleet reliability evals published (07.2026): 0/17 Tier-2 (high-risk) actions slipped past the human approval gate in recorded runs; failure modes documented in public (FAILURE-MODES.md)
- Audience & network: 169k-subscriber Telegram channel (@PaloAltoAi) + 100+ AI-practitioner community in Palo Alto, the heart of Silicon Valley; Silicon Valley network built on the ground plus a decade of Japan/Korea startup-community depth; enterprise advisory for Foxconn and ANA Airlines subsidiaries

## Education

- PhD in Education (Information Technologies), Paris College of International Education
- MSc, Computer and Information Systems Security, National Research Nuclear University MEPhI
- BSc, Computer and Information Sciences, National Research Nuclear University MEPhI

## Beyond work

- **Aviation**: Licenced helicopter pilot, ~200 flight hours; Student pilot on fixed-wing, working toward the licence; Long-term goal: a small plane for the family, and a round-the-world flight in it
- **Endurance and mountain biking**: Half-marathons; Mountain biking (downhill, jumps) on an analogue bike by choice: a workout should stay a workout; Surfing, windsurfing, kitesurfing, tennis
- **Sharp tools, clean workspace**: Perfectionist about the instrument: kitchen knives, keyboard, mouse, spotless glass; A 5-machine, 9-monitor workspace I administer myself, so work runs in parallel instead of context-switching inside one box; Ten years of orchestrating many tasks at once; voice-first input over typing
- **Cooking for the family**: Cook dinner for the household on weekends
