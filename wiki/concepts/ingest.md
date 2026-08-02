---
title: Ingest
type: concept
created: 2026-08-01
updated: 2026-08-02
tags: [workflow, operations]
sources: [sources/001-llm-wiki-pattern]
status: active
---

# Ingest

Ingest is a wiki operation. It takes one raw source, or a batch of raw sources, and **adds their knowledge** to the wiki.

## Typical flow

1. Read the source from `raw/` and never change it
2. Discuss the main lessons with the human, unless the work is in batch or unsupervised mode
3. Write `wiki/sources/NNN-slug.md`
4. Create or update entity and concept pages, often touching 5–15 pages
5. Update the [[../index|index]] and, when needed, the [[../overview|overview]]
6. Add a new entry to the [[../log|log]]

## Design preference

The default is **one source at a time**, with the human involved. Batch mode is available when requested.
