---
title: Query Filing
type: concept
created: 2026-08-01
updated: 2026-08-01
tags: [workflow, operations]
sources: [sources/001-llm-wiki-pattern]
status: active
---

# Query Filing

Wiki operation: answer a question from the wiki, then **save valuable synthesis** as a page under `wiki/queries/` or `wiki/comparisons/` so exploration compounds like ingested sources.

## Flow

1. Read [[../index|index]] → drill into pages
2. Synthesize answer with citations
3. File reusable answers; update index + log

## Principle

Chat is ephemeral. Filed queries are knowledge. Prefer filing when the answer is a comparison, thesis, or connection you'd want again.
