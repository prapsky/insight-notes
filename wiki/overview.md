---
title: Wiki Overview
type: overview
created: 2026-08-01
updated: 2026-08-01
tags: [meta, synthesis]
sources: [sources/001-llm-wiki-pattern, sources/002-endgame-245-purbaya-sadewa]
status: active
---

# Overview

This is **insight-notes** — a personal LLM Wiki (second brain). Knowledge compounds in interlinked markdown under `wiki/`; immutable sources live in `raw/`.

## Current shape

Two layers of content:

1. **Meta** — How the wiki itself works ([[sources/001-llm-wiki-pattern|LLM Wiki pattern]]).
2. **Indonesia macro / policy** — First domain ingest from [[sources/002-endgame-245-purbaya-sadewa|Endgame #245]] with [[entities/purbaya-yudi-sadewa|Purbaya Yudi Sadewa]]: money growth, expectation management, debottlenecking, FDI climate, STEM pipeline.

## Major topics

| Area | Status | Hub pages |
|------|--------|-----------|
| Knowledge systems | Active | [[concepts/llm-wiki]], [[concepts/rag]], [[concepts/memex]] |
| Wiki operations | Active | [[concepts/ingest]], [[concepts/query-filing]], [[concepts/wiki-lint]] |
| Indonesia growth & liquidity | Active (single-source) | [[concepts/money-supply-vs-interest-rates]], [[concepts/expectation-management]], [[concepts/fdi-climate]] |
| Investment & talent | Active (single-source) | [[concepts/investment-debottlenecking]], [[concepts/uncertainty-to-risk-translation]], [[concepts/stem-talent-pipeline]] |
| People / history | Mixed | [[entities/vannevar-bush]], [[entities/purbaya-yudi-sadewa]], era stubs (Prabowo / SBY / Jokowi) |

## Working theses

> Retrieval alone does not accumulate understanding. A maintained intermediate wiki — compiled once per source, kept current — compounds; RAG rediscovers from scratch every time.

> *(Attributed — Purbaya)* Indonesia’s near-term binding problems are domestic: insufficient money in the *system*, broken expectations, and field-level investment bottlenecks — not primarily “global uncertainty.” ~6.5% from dual engines; ~8% needs FDI once climate and talent catch up.

## Gaps / next

- Domain content is still **one interview deep** — corroborate money-growth, confidence, and FDI figures from official series
- Era stubs (SBY / Jokowi / Prabowo) need independent sources
- More Endgame episodes or opposing macro views would prevent single-voice capture
- Schema may need `policy` / `episode` conventions if media ingest becomes routine
- Search tooling (e.g. qmd) still deferred

## How to grow this

Drop a source into `raw/`, say **ingest**, and the wiki expands. Ask questions; file the best answers. Periodically **lint**.
