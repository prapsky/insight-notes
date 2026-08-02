---
title: RAG vs LLM Wiki
type: comparison
created: 2026-08-01
updated: 2026-08-02
tags: [comparison, knowledge-management]
sources: [sources/001-llm-wiki-pattern]
status: active
---

# RAG vs LLM Wiki

| Dimension | [[concepts/rag\|RAG]] | [[concepts/llm-wiki\|LLM Wiki]] |
|-----------|----------------------|--------------------------------|
| When knowledge is organized | When a question is asked | When sources are added or updated |
| Between questions | Knowledge does not build up | The wiki builds knowledge over time |
| Cross-references | Found again as needed | Clearly written and maintained as links |
| Contradictions | Easy to miss | Flagged on pages |
| Maintenance cost | Easy setup and no wiki maintenance | The LLM handles the maintenance work |
| Best for | Large collections that rarely change and one-time questions | Ongoing learning and main ideas that change over time |

## Shared ground

Both approaches can use search. The difference is **what** they search. RAG searches sections of raw sources. An LLM Wiki searches organized pages that link to each other.

## Source

[[sources/001-llm-wiki-pattern]]
