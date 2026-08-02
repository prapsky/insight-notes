---
title: RAG (Retrieval-Augmented Generation)
type: concept
created: 2026-08-01
updated: 2026-08-02
tags: [knowledge-management, retrieval]
sources: [sources/001-llm-wiki-pattern]
status: active
---

# RAG

**Retrieval-Augmented Generation (RAG)** is a way to answer questions with documents. When you ask a question, the system searches a document collection for relevant sections. It then uses those sections to generate an answer. NotebookLM, ChatGPT file uploads, and most "chat with your docs" systems use this approach.

## Strengths

- Quick to set up, with no wiki to maintain over time
- Works with large document collections by using search or embeddings, which are numerical representations of meaning

## Limits (from the LLM Wiki lens)

- **No accumulation** — each question requires the system to find relevant pieces again
- Careful explanations that combine several documents must be rebuilt each time
- Cross-references, contradictions, and changing main ideas are not stored as maintained pages

## Relationship to this wiki

RAG provides a useful contrast with [[concepts/llm-wiki|LLM Wiki]]. See [[comparisons/rag-vs-llm-wiki]]. This vault may still search *the wiki itself*. It checks the index first and may add search later. In that case, it searches organized knowledge instead of only searching raw sources.
