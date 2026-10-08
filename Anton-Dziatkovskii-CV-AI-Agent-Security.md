# Anton Dziatkovskii — Red Team / AI Agent Security Engineering (applied)

https://tonydzi.github.io/ · github.com/tonydzi · dzyatkovskiy.a@gmail.com · WhatsApp +1 341 222 9178 · calendly.com/paloaltolab/1-on-1 · Palo Alto, CA (Silicon Valley) – Sintra, PT / US O-1 · EU citizen (Poland)

## Summary
Security engineer for agent systems: I run a production agent fleet and I attack it. A reproducible MCP tool-poisoning testbed where one poisoned string reaches four agents through four input surfaces and asks for five forbidden actions, every one stopped by a single independent authorization boundary, with a mutation suite that breaks the gate six ways and must go red; a written threat model mapped to OWASP LLM Top 10 (2025) and MITRE ATLAS by exact identifier, published with the rows I do not cover; and the gate's own refusal and over-refusal rates reported as two separate numbers. Also shipped: agent-leash, verbatim-citation-gate (catches fabricated RAG citations) and agent-control-plane-casebook. MSc in Computer & Information Systems Security (MEPhI, cryptography); Python and C++; smart-contract audit background and anti-fraud instincts from a decade in adversarial crypto markets. The fleet in question: production multi-machine agent fleet, 8 registered nodes and 1,275 scheduled routines across the 5 that report (measured 2026-10-08, recomputed weekly), operated in public: consensus, CRM, persistent memory. US O-1 visa (active) + EU citizen (Polish passport) — authorized to work in the US and anywhere in the EU immediately, no visa sponsorship required; open to relocation (SF Bay Area base network) or remote

## Skills
Python, C++, red team, AI security, agent safety, prompt injection, guardrails, threat modeling, OWASP LLM Top 10, MITRE ATLAS, MCP security, least privilege, human-in-the-loop, evals, cryptography, audit, trust and safety

## Experience

**Operating Lead — Palo Alto AI Research Lab** (2023 – Present)

Independent lab started in 2023 in Palo Alto, CA; grew a community of 100+ AI practitioners, including Stanford researchers and big-tech engineers. Production multi-machine Claude fleet run in public: claw-consensus (reproducible multi-machine agent consensus, offline demo, published evals, FAILURE-MODES.md), verbatim-citation-gate (zero-token gate + burden-of-proof judge that catches fabricated RAG citations, MIT), agent-control-plane-casebook (reproducible control-plane failures from the production fleet — each case ships a deterministic repro, a runnable red test and an upstream bug report), the operating manual written day by day (相棒 AIBŌ · The Partner).

**Chief Engineer, Lending & Risk Management — Everex (Singapore)** (2017 – 2018)

Wrote smart contracts and led government/bank relations across SE Asia on structuring crypto payments and stablecoins; blockchain credit scoring, stable-value payments.

**COO / CTO (hired executive) — Platinum Software Development Company / Platinum VC & Incubator** (2015 – Present)

Hired operating executive (COO/CTO) who ran a startup incubator + software house in APAC since 2015 (11 years), alongside Japanese partner Tetsuji Nagata (Grand Corp; 12 years at Bloomberg before that). The job a partner at 500 Startups or Plug and Play does — deal flow, cohorts, founder coaching, advisor matching, fundraising — done hands-on at a boutique incubator, with rare depth in Silicon Valley and even the Japanese and Korean startup communities. Portfolio ~70% crypto / 30% other, AI startups included.

- Shipped crypto-exchange infrastructure: cryptocurrency backends, market-maker engines, high-frequency trading systems; partnerships with hedge funds, market makers, brokers
- Designed one of the first detailed frameworks for a national government to issue its own stablecoins (regulatory + token-economic design)
- Managed a distributed engineering org of 40+ developers across APAC as product owner

**Sales Director, compute hardware (Southeast Europe) / CRM-ERP Development Director (Microsoft Navision, Salesforce) — Merlion** (2006 – 2015)

One of the largest private IT distributors in Eastern Europe. Enterprise and B2B sales of computing hardware across Southeast Europe, and the ERP and CRM systems the sales floor ran on (Microsoft Navision and Salesforce, 5 years), where I learned that deal flow runs on CRM quality.

**CRM Developer Intern — CRM/ERP consulting (Salesforce ecosystem)** (2004 – 2006)

First professional years: CRM systems development in the Salesforce/ERP ecosystem.

## Selected proof
- Red team on my own fleet, published: github.com/tonydzi/agent-fleet-red-team - a written threat model (8 assets, 6 trust boundaries, 10 untrusted input surfaces, 9 residual risks carrying numbers) and a mapping of the running system onto OWASP Top 10 for LLM Applications (2025) and MITRE ATLAS by exact identifier, published together with its holes: 15 ATLAS techniques reproduced on my own stand, 10 more named as applicable and untested, 12 ATLAS mitigations implemented and 8 explicitly not
- Guardrail measured as two separate numbers rather than one accuracy figure (2026-10-08): 100% refusal across 49 must-ask actions, 50% over-refusal across 42 benign ones, and 71.4% rule coverage - 14 of the 49 reach a human only because the default is fail-closed, each one named. Six-way mutation suite, shown failing on broken code before it was shown passing. On real traffic the same gate fired 2879 times in 90 days with 0 asks expiring unanswered
- Indirect prompt injection reproduced end to end (github.com/tonydzi/leash-poc): one poisoned string, four input surfaces, four agents, 24 requests. Naive fleet exfiltrated 168 bytes, deleted 5 files, rotated 4 production keys and spawned 4 admin sub-agents; the same fleet behind one independent authorization boundary scored zero on all five and still completed the user's work. 27 hash-chained decisions, chain verified after SIGKILL mid-run
- Merged into microsoft/semantic-kernel (#14371): closed the check-time/use-time gap in the OpenAPI plugin's anti-SSRF validator: its built-in HTTP client now connects to the exact address that was vetted. Evidence-first OSS reliability work in the AI-agent ecosystem: mutation-tested reviews of other people's PRs and bug reports carrying a deterministic repro plus a regression test shown failing on the unfixed code. google/adk-python#6957 — author adopted all three review findings in 6h («genuinely one of the most useful reviews I've gotten on this PR»); #6887 fixed upstream from our report; credited in headroom v2.0.8 release notes. Scope since 07.2026 (verified 2026-10-08): 40 PRs merged into 25 third-party engineering projects (Microsoft Semantic Kernel, MCP Go SDK, UK AISI inspect_ai, QwenLM/qwen-code, google-gemini/cookbook, fastmcp, agno, pydantic/logfire) + 65 issues filed upstream
- 148 public repos (2026-10-08); flagships: agent-fleet-red-team, leash-poc, agent-approval-gate, claw-consensus, verbatim-citation-gate, claude-bible, agent-control-plane-casebook
- 50+ published items, 137 citations, h-index 7 (verified 2026-09-01); 2 preprints on multi-agent stability (arXiv in progress)
- Measured agent-fleet reliability evals published (07.2026): 0/17 Tier-2 (high-risk) actions slipped past the human approval gate in recorded runs; failure modes documented in public (FAILURE-MODES.md)
- Audience & network: 169k-subscriber Telegram channel (@PaloAltoAi) + 100+ AI-practitioner community in Palo Alto, the heart of Silicon Valley; Silicon Valley network built on the ground plus a decade of Japan/Korea startup-community depth; enterprise advisory for Foxconn and ANA Airlines subsidiaries

## Education

- PhD in Education (Information Technologies), Paris College of International Education
- MSc, Computer and Information Systems Security, National Research Nuclear University MEPhI
- BSc, Computer and Information Sciences, National Research Nuclear University MEPhI

## Interests

- **Endurance sport**: Triathlon: mid-pack drifting to the back, and honest about it; Half-marathons; Surfing, windsurfing, kitesurfing, tennis; Mountain biking (downhill, jumps) on an analogue bike by choice: a workout should stay a workout
- **Aviation and building bunkers**: Licenced helicopter pilot, ~200 flight hours; student pilot on fixed-wing; I build bunkers: several already standing in New Zealand and Australia - the fixed-wing licence is how I reach them when things go sideways; Long-term goal: a small plane for the family, and a round-the-world flight in it
