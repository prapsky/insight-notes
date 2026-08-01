---
title: RAG (Retrieval-Augmented Generation)
type: concept
created: 2026-08-01
updated: 2026-08-01
tags: [knowledge-management, retrieval]
sources: [sources/001-llm-wiki-pattern]
status: active
---

# RAG

**Retrieval-Augmented Generation**: at query time, retrieve relevant chunks from a document collection, then generate an answer. Used by NotebookLM, ChatGPT file uploads, and most "chat with your docs" systems.

## Strengths

- Fast to stand up; no ongoing wiki maintenance
- Works on large corpora with embeddings / search

## Limits (from the LLM Wiki lens)

- **No accumulation** — each question rediscovers fragments
- Subtle multi-document synthesis is re-pieced every time
- Cross-references, contradictions, and evolving thesis are not first-class artifacts

## Relationship to this wiki

RAG is the foil for [[concepts/llm-wiki|LLM Wiki]]. See [[comparisons/rag-vs-llm-wiki]]. This vault may still use retrieval *over the wiki* (index first; optional search later) — that is retrieval over *compiled* knowledge, not raw-only RAG.
