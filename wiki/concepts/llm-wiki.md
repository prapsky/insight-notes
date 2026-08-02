---
title: LLM Wiki
type: concept
created: 2026-08-01
updated: 2026-08-02
tags: [knowledge-management, core]
sources: [sources/001-llm-wiki-pattern]
status: active
---

# LLM Wiki

An **LLM Wiki** is a lasting collection of connected Markdown files. A large language model (LLM) builds and maintains these files between you and your raw sources. During [[concepts/ingest|ingest]], the LLM organizes knowledge from a source. It updates that knowledge when new material arrives. It does not rediscover everything each time you ask a question.

## Why it exists

[[concepts/rag|RAG]] starts from scratch for each answer. An LLM Wiki builds knowledge over time. Entity pages gain more detail. Topic summaries are updated. Contradictions are marked. Combined explanations reflect everything read so far.

## Three layers

1. **Raw** — original sources that must not be changed (`raw/`)
2. **Wiki** — pages created by the LLM (`wiki/`)
3. **[[concepts/schema|Schema]]** — rules that tell the LLM how to maintain the wiki (`.cursorrules`)

## Operations

| Op | Role |
|----|------|
| [[concepts/ingest\|Ingest]] | Add knowledge from a new source to many pages |
| [[concepts/query-filing\|Query]] | Answer from the wiki and save useful answers |
| [[concepts/wiki-lint\|Lint]] | Check the wiki for consistency problems and gaps |

## See also

- [[comparisons/rag-vs-llm-wiki]]
- [[concepts/memex]] — an earlier idea that inspired this approach
- [[sources/001-llm-wiki-pattern]]
