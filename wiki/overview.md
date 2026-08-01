---
title: Wiki Overview
type: overview
created: 2026-08-01
updated: 2026-08-01
tags: [meta, synthesis]
sources: [sources/001-llm-wiki-pattern]
status: active
---

# Overview

This is **insight-notes** — a personal LLM Wiki (second brain). Knowledge compounds in interlinked markdown under `wiki/`; immutable sources live in `raw/`.

## Current shape

Early bootstrap. One foundational source ingested: the [[sources/001-llm-wiki-pattern|LLM Wiki pattern]] itself. The wiki now knows *how it works* and the core concepts that define it.

## Major topics

| Area | Status | Hub pages |
|------|--------|-----------|
| Knowledge systems | Active | [[concepts/llm-wiki]], [[concepts/rag]], [[concepts/memex]] |
| Wiki operations | Active | [[concepts/ingest]], [[concepts/query-filing]], [[concepts/wiki-lint]] |
| People / history | Stub-rich | [[entities/vannevar-bush]] |

## Working thesis

> Retrieval alone does not accumulate understanding. A maintained intermediate wiki — compiled once per source, kept current — compounds; RAG rediscovers from scratch every time.

## Gaps / next

- No personal domain content yet (goals, research topic, book, etc.) — awaiting first *real* source from you
- Schema may need domain-specific entity types as the focus clarifies
- Search tooling (e.g. qmd) deferred until scale demands it

## How to grow this

Drop a source into `raw/`, say **ingest**, and the wiki expands. Ask questions; file the best answers. Periodically **lint**.
