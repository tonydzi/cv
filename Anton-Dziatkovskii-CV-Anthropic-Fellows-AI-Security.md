# Anton Dziatkovskii — Research Engineer, AI security & evaluation infrastructure

https://tonydzi.github.io/ · github.com/tonydzi · github.com/tonydzi/github-evidence · dzyatkovskiy.a@gmail.com · +1 341 222 9178 · Palo Alto, CA / US O-1 (active) · EU citizen (Poland) · Google Scholar: scholar.google.com/citations?user=b8gKHiMAAAAJ

## Summary
Security-trained systems engineer (MSc, Computer & Information Systems Security, MEPhI — cryptography), then exchange backends, market-maker engines and high-frequency trading systems in production, then smart contracts for stablecoin payments (Everex, 2017–18), then eleven years owning engineering delivery as a hired COO/CTO. I write Python and C++.

**My security instincts come from a domain where a defect is priced in money the same day it ships.** I wrote smart contracts, audited other people's, and ran the incubator where cryptographers shipped theirs — adversarial review was the job, not a phase of it. That is the transfer I bring to evaluating what a model does when it is trying to break something.

Since 2023 I run a production multi-machine Claude agent fleet in public and use it as an experimental rig: approval gates, control-plane failure cases, eval harnesses. I do not claim ML research; I claim the engineering research runs on — reproducible evals, failure taxonomies, adversarial probes, and bug reports that arrive with a deterministic repro and a regression test shown failing on the unfixed code. Built with Claude as implementation collaborator; I own problem framing, architecture, evaluation and final QA.

## Evidence-first open-source work (Jul–Sep 2026, verified 2026-09-20 via public GitHub API)
- 127 pull requests opened in other people's repositories, 43 merged; 58 issues filed with reproductions; 44 reviews on other people's PRs; credited in 21 third-party release notes — index: github.com/tonydzi/github-evidence
- UK AISI **inspect_ai** #4769 (merged 2026-09-01, +351/−18): model-graded scorers with a panel of graders now combine grades with a strict-majority reducer instead of mode; the "unscored stays in the denominator" semantic was chosen deliberately so a broken grader cannot cast the deciding vote
- google/adk-python #6957 (review, 2026-09-01): OAuth2 client_secret and tokens leaking over three endpoints — a mutation matrix showed which of the project's own tests stayed green; the author adopted all three findings within six hours ("genuinely one of the most useful reviews I've gotten on this PR")
- QwenLM/qwen-code #9414, punkpeye/fastmcp #325, agno #9498, zilliztech/memsearch #695, modelcontextprotocol/go-sdk #1142/#1148/#1159/#1196, Lyellr88/marm-memory #181/#183/#185/#192 (CI now builds the image on PRs; a healthcheck that could never report unhealthy), mixelpixx/Konnect #199/#442/#505 — each shipped with a repro or a red test
- google-gemini/cookbook #1296: worked example that checks citation faithfulness in RAG

## Own repositories (github.com/tonydzi)
- **verbatim-citation-gate** — zero-token deterministic gate plus burden-of-proof judge that catches fabricated RAG citations (MIT); listed in Awesome-LLMOps, awesome-rag-production and ant-research/awesome-mllm-guardrails
- **agent-control-plane-casebook** — reproducible control-plane failures from the live fleet; each case ships a deterministic repro, a runnable red test and an upstream bug report
- **claw-consensus** — reproducible multi-machine agent consensus with an offline demo, docs/EVALS.md and docs/FAILURE-MODES.md; fleet-reliability eval published 07.2026 (tonydzi.github.io/the-journey/evals-fleet-reliability.html): 0/17 Tier-2 (high-risk) actions slipped past the human approval gate in recorded runs
- **agent-leash** (LEASH-8 control model, listed in Awesome-LLMSecOps) · **sqlite-graph-memory** (retrieval eval on wikilink gold; #12 fixed an nDCG that could exceed 1.0)

## Experience
**Palo Alto AI Research Lab — Technical Lead** (2023 – Present) · Palo Alto, CA
Independent lab; 100+ AI practitioners in the community, including Stanford researchers and big-tech engineers. Six-machine Claude fleet operated in public (consensus, persistent memory, CRM, 100+ automation routines) with human approval gates on anything irreversible; 13 daily autonomous lanes (code review, live-install documentation QA, issue-first bug reports, thread watch).

**Everex (Singapore) — Chief Engineer, Lending & Risk Management** (2017 – 2018)
Wrote smart contracts for stable-value payments and blockchain credit scoring; led government and bank relations across SE Asia on structuring crypto payments and stablecoins. Contract code is the one place where a missed edge case is withdrawn by a stranger the same week, so review discipline there is not a process — it is the product.

**Smart-contract security across the Platinum portfolio** (2017 – 2024)
Audited contracts written by the teams the incubator took in — token distribution, vesting and locking, exchange settlement — and set the review bar those teams shipped against. Portfolio was roughly 70% crypto infrastructure, so the sample was adversarial by construction: public code, public money, attackers reading the same source.

**Platinum Software Development / Platinum VC & Incubator — COO / CTO (hired executive)** (2015 – Present) · APAC
Owned engineering delivery end to end: crypto-exchange infrastructure (backends, market-maker engines, HFT systems), a distributed organisation of 40+ developers, and an in-house CRM I wrote myself that up to 30 operators used daily. In 2018 worked with banks and central-bank stakeholders in Myanmar, Cambodia, Thailand and Australia on frameworks for their first stablecoins.

**Merlion — CRM/ERP Development Director (Microsoft Navision, Salesforce); enterprise hardware sales, SE Europe** (2006 – 2015)
Built the ERP and CRM systems the sales floor ran on (5 years); sold compute hardware (GPUs, CPUs, memory) B2B.

## Education
- MSc, Computer and Information Systems Security — National Research Nuclear University MEPhI
- BSc, Computer and Information Sciences — National Research Nuclear University MEPhI
- PhD in Education (Information Technologies), 2021 — Paris College of International Education; 50+ published items, 137 citations, h-index 7 (verified 2026-09-01); two preprints on multi-agent stability (not yet released)

## Logistics
Palo Alto, CA base; can work from the Berkeley workspace. US O-1 active and EU (Polish) citizen — no visa sponsorship needed. Available January 2027, full-time.

## Interests

- **Endurance sport**: triathlon; half-marathons; surfing; mountain biking (downhill, jumps) on an analogue bike by choice: a workout should stay a workout
- **Aviation and building bunkers**: licenced helicopter pilot, ~200 flight hours; student pilot on fixed-wing; I build bunkers: several already standing in New Zealand and Australia - the fixed-wing licence is how I reach them when things go sideways
