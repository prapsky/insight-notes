---
title: LLM Wiki
type: concept
created: 2026-08-01
updated: 2026-08-01
tags: [knowledge-management, core]
sources: [sources/001-llm-wiki-pattern]
status: active
---

# LLM Wiki

A **persistent, interlinked collection of markdown files** that an LLM builds and maintains between you and your raw sources. Knowledge is compiled on [[concepts/ingest|ingest]] and revised as new material arrives — not rediscovered via retrieval on every question.

## Why it exists

[[concepts/rag|RAG]] answers from scratch each time. An LLM Wiki accumulates: entity pages deepen, topic summaries revise, contradictions get flagged, synthesis reflects everything read so far.

## Three layers

1. **Raw** — immutable sources (`raw/`)
2. **Wiki** — LLM-generated pages (`wiki/`)
3. **[[concepts/schema|Schema]]** — rules that make the LLM a maintainer (`.cursorrules`)

## Operations

| Op | Role |
|----|------|
| [[concepts/ingest\|Ingest]] | Integrate a new source across many pages |
| [[concepts/query-filing\|Query]] | Answer from wiki; file valuable answers |
| [[concepts/wiki-lint\|Lint]] | Health-check consistency and gaps |

## See also

- [[comparisons/rag-vs-llm-wiki]]
- [[concepts/memex]] — historical ancestor
- [[sources/001-llm-wiki-pattern]]
