---
title: RAG vs LLM Wiki
type: comparison
created: 2026-08-01
updated: 2026-08-01
tags: [comparison, knowledge-management]
sources: [sources/001-llm-wiki-pattern]
status: active
---

# RAG vs LLM Wiki

| Dimension | [[concepts/rag\|RAG]] | [[concepts/llm-wiki\|LLM Wiki]] |
|-----------|----------------------|--------------------------------|
| When knowledge is structured | Query time | Ingest / update time |
| Between questions | Nothing accumulates | Wiki compounds |
| Cross-references | Re-discovered ad hoc | Explicit, maintained links |
| Contradictions | Easy to miss | Flagged on pages |
| Maintenance cost | Low setup, no wiki upkeep | LLM does bookkeeping |
| Best for | Large static corpora, one-shot Q&A | Ongoing learning, evolving thesis |

## Shared ground

Both can use search. Difference is **what** you search: raw chunks vs compiled, interlinked pages.

## Source

[[sources/001-llm-wiki-pattern]]
