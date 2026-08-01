---
title: Wiki Overview
type: overview
created: 2026-08-01
updated: 2026-08-01
tags: [meta, synthesis]
sources: [sources/001-llm-wiki-pattern, sources/002-endgame-245-purbaya-sadewa, sources/003-endgame-248-tom-lembong, sources/004-endgame-193-michael-levitt, sources/005-endgame-272-martyn-terpilowski]
status: active
---

# Overview

This is **insight-notes** — a personal LLM Wiki (second brain). Knowledge compounds in interlinked markdown under `wiki/`; immutable sources live in `raw/`.

## Current shape

Five layers of content:

1. **Meta** — How the wiki itself works ([[sources/001-llm-wiki-pattern|LLM Wiki pattern]]).
2. **Indonesia macro / liquidity** — [[sources/002-endgame-245-purbaya-sadewa|Endgame #245]] with [[entities/purbaya-yudi-sadewa|Purbaya]]: money growth, expectation management, satgas debottlenecking, path to 8%.
3. **Indonesia governance / soft infra** — [[sources/003-endgame-248-tom-lembong|Endgame #248]] with [[entities/tom-lembong|Tom Lembong]]: teachers, decentralization paradox, ownership society, risk culture, idea-contest centrism.
4. **Science / intelligence** — [[sources/004-endgame-193-michael-levitt|Endgame #193]] with [[entities/michael-levitt|Michael Levitt]]: biological intelligence, diversity-as-strategy, interdisciplinary silos, serendipity/failure (COVID kept light).
5. **Technocracy / business meritocracy** — [[sources/005-endgame-272-martyn-terpilowski|Endgame #272]] with [[entities/martyn-terpilowski|Martyn Terpilowski]]: meritocracy vs patronage, FDI/talent sponge, deep-tech long-termism ([[entities/bhumi-varta-technology|Bhumi Varta]] as counterexample).

Shared bridges:

- Between (2) and (3): [[concepts/fdi-climate|FDI climate]] = rule of law + [[concepts/uncertainty-to-risk-translation|uncertainty → priced risk]].
- Between (3) and (4): productive failure — [[concepts/risk-as-innovation-fuel|risk as innovation fuel]] ↔ [[concepts/scientific-serendipity-and-failure|scientific serendipity & failure]].
- Between (2)/(3) and (5): FDI sponge + [[concepts/meritocracy-vs-patronage|meritocracy]] + [[concepts/brain-gain-and-circulation|brain gain]]; Gita’s M/GDP–elite narrative bridge on [[concepts/money-supply-vs-interest-rates|money supply]]; honest vs recycled failure on risk-as-fuel.

## Major topics

| Area | Status | Hub pages |
|------|--------|-----------|
| Knowledge systems | Active | [[concepts/llm-wiki]], [[concepts/rag]], [[concepts/memex]] |
| Wiki operations | Active | [[concepts/ingest]], [[concepts/query-filing]], [[concepts/wiki-lint]] |
| Science / intelligence | Active (Levitt-led) | [[concepts/biological-intelligence]], [[concepts/diversity-as-evolutionary-strategy]], [[concepts/interdisciplinary-silos]], [[concepts/scientific-serendipity-and-failure]] |
| Indonesia growth & liquidity | Active (Purbaya-led) | [[concepts/money-supply-vs-interest-rates]], [[concepts/expectation-management]], [[concepts/fdi-climate]] |
| Investment & talent | Active (cross-source) | [[concepts/investment-debottlenecking]], [[concepts/uncertainty-to-risk-translation]], [[concepts/stem-talent-pipeline]], [[concepts/brain-gain-and-circulation]] |
| Governance & culture | Active (Tom + Martyn) | [[concepts/soft-infrastructure-teachers]], [[concepts/decentralization-paradox]], [[concepts/ownership-society]], [[concepts/risk-as-innovation-fuel]], [[concepts/idea-contest-and-centrism]], [[concepts/meritocracy-vs-patronage]] |
| Deep tech / startups | Active (Martyn-led) | [[concepts/deep-tech-long-termism]], [[entities/bhumi-varta-technology]] |
| People / history | Mixed | [[entities/vannevar-bush]], [[entities/michael-levitt]], [[entities/purbaya-yudi-sadewa]], [[entities/tom-lembong]], [[entities/martyn-terpilowski]], era stubs (Prabowo / SBY / Jokowi) |

## Working theses

> Retrieval alone does not accumulate understanding. A maintained intermediate wiki — compiled once per source, kept current — compounds; RAG rediscovers from scratch every time.

> *(Attributed — Purbaya)* Indonesia’s near-term binding problems are domestic: insufficient money in the *system*, broken expectations, and field-level investment bottlenecks — not primarily “global uncertainty.” ~6.5% from dual engines; ~8% needs FDI once climate and talent catch up.

> *(Attributed — Tom)* Soft infrastructure (especially teachers), incentive redesign against licensing rents ([[concepts/ownership-society|ownership society]]), and a culture that prices *and* permits risk-taking are co-equal with hard capital. Substance media and open idea contest shift mental models before politics and strategy follow.

> *(Attributed — Levitt)* Learn from biological intelligence: diversity is survival technology because we don’t know the future; disciplines are teaching artifacts; productive scientific failure (wrong 90–99%) and AI-as-tutor unlock young disruptors.

> *(Attributed — Martyn)* Technocracy in business = meritocracy + openness. Wrong people in wrong jobs and circular VC beat “skill gap” as the binding constraint; be an FDI/talent sponge; build exportable deep tech over decade horizons — money without management/DD is not a panacea.

## Gaps / next

- Endgame voices still interview-depth; corroborate money-growth, M/GDP, STEM conversion shares, education-budget composition, FDI, and permit-density figures from official series
- Natural comparison pages: Purbaya vs Tom vs Martyn on path-to-growth (liquidity/satgas vs teachers/incentives vs meritocracy/sponge/deep tech)
- Bio-X / random seed-grant design vs Indonesian STEM pipeline — unexplored comparison
- Era stubs (SBY / Jokowi / Prabowo) need independent sources
- Levitt COVID claims filed contested-only; elevate only with dedicated epidemiology sources
- Bhumi Varta product claims still interview-only (stub)
- Schema may need `policy` / `episode` conventions if media ingest becomes routine
- Search tooling (e.g. qmd) still deferred

## How to grow this

Drop a source into `raw/`, say **ingest**, and the wiki expands. Ask questions; file the best answers. Periodically **lint**.
