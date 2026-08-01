---
title: LLM Wiki Pattern
type: source
created: 2026-08-01
updated: 2026-08-01
tags: [meta, knowledge-management, foundational]
sources: []
status: active
---

# LLM Wiki Pattern

**Raw:** [[../../raw/notes/001-llm-wiki-pattern|raw/notes/001-llm-wiki-pattern.md]]  
**Type:** Idea / architecture note  
**Ingested:** 2026-08-01

## Summary

Argues that typical LLM+document workflows ([[concepts/rag|RAG]], NotebookLM, file uploads) rediscover knowledge from scratch on every question. The alternative: an LLM that **incrementally builds and maintains a persistent wiki** between the human and raw sources. Knowledge is compiled on ingest and kept current — not re-derived at query time.

## Core claims

1. A wiki sitting between raw sources and questions is a **compounding artifact** — cross-refs, contradictions, and synthesis accumulate.
2. Three layers: immutable **raw sources**, LLM-owned **wiki**, and a **[[concepts/schema|schema]]** that enforces discipline.
3. Three primary ops: [[concepts/ingest|ingest]], [[concepts/query-filing|query]] (with filing), [[concepts/wiki-lint|lint]].
4. `index.md` + `log.md` are enough navigation at moderate scale (~100 sources); search tools optional later.
5. Humans abandon wikis due to maintenance cost; LLMs make maintenance near-zero — solving the Memex problem of *who keeps trails current*.

## Notable ideas

- "Obsidian is the IDE; the LLM is the programmer; the wiki is the codebase."
- Good query answers should be **filed back** into the wiki so exploration compounds.
- Conceptual lineage: [[entities/vannevar-bush|Vannevar Bush]]'s [[concepts/memex|Memex]] (1945).

## Entities & concepts touched

- [[concepts/llm-wiki]], [[concepts/rag]], [[concepts/memex]], [[concepts/ingest]], [[concepts/query-filing]], [[concepts/wiki-lint]], [[concepts/schema]]
- [[entities/vannevar-bush]]
- [[comparisons/rag-vs-llm-wiki]]

## Open questions

- What personal domain should this second brain specialize in first?
- When does index-only navigation break down enough to need local search (e.g. qmd)?
