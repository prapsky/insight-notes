---
title: LLM Wiki Pattern
type: source
created: 2026-08-01
updated: 2026-08-02
tags: [meta, knowledge-management, foundational]
sources: []
status: active
---

# LLM Wiki Pattern

**Raw:** [[../../raw/notes/001-llm-wiki-pattern|raw/notes/001-llm-wiki-pattern.md]]  
**Type:** Idea / architecture note  
**Ingested:** 2026-08-01

## Summary

Typical LLM and document tools ([[concepts/rag|RAG]], NotebookLM, and file uploads) search the source material again for every question. This note proposes a different approach. An LLM **gradually builds and maintains a permanent wiki** between the human and the raw sources. It organizes knowledge when a source is added and keeps that knowledge current. It does not rebuild the same understanding for every query.

## Core claims

1. A wiki between the raw sources and the questions becomes more useful over time. Cross-references, contradictions, and combined insights continue to accumulate.
2. The system has three layers: **raw sources** that never change, a **wiki** maintained by the LLM, and a **[[concepts/schema|schema]]** (a set of organizing rules) that keeps the work consistent.
3. It has three main operations: [[concepts/ingest|ingest]] (add a source), [[concepts/query-filing|query]] (answer and save useful results), and [[concepts/wiki-lint|lint]] (check the wiki's health).
4. At a moderate size of about 100 sources, `index.md` and `log.md` provide enough navigation. Search tools can be added later if needed.
5. People often abandon wikis because maintenance takes too much work. LLMs can make that work almost free. This addresses the Memex problem: *who keeps the knowledge trails current?*

## Notable ideas

- "Obsidian is the IDE; the LLM is the programmer; the wiki is the codebase."
- Useful query answers should be **saved back** into the wiki. This makes later exploration build on earlier work.
- The idea follows [[entities/vannevar-bush|Vannevar Bush]]'s [[concepts/memex|Memex]] from 1945.

## Entities & concepts touched

- [[concepts/llm-wiki]], [[concepts/rag]], [[concepts/memex]], [[concepts/ingest]], [[concepts/query-filing]], [[concepts/wiki-lint]], [[concepts/schema]]
- [[entities/vannevar-bush]]
- [[comparisons/rag-vs-llm-wiki]]

## Open questions

- What personal domain should this second brain specialize in first?
- When does index-only navigation break down enough to need local search (e.g. qmd)?
