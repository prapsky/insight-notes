---
title: Ingest
type: concept
created: 2026-08-01
updated: 2026-08-01
tags: [workflow, operations]
sources: [sources/001-llm-wiki-pattern]
status: active
---

# Ingest

Wiki operation: take one (or a batch of) raw source(s) and **integrate** them into the wiki.

## Typical flow

1. Read source from `raw/` (never modify)
2. Discuss takeaways with human (unless batch/unsupervised)
3. Write `wiki/sources/NNN-slug.md`
4. Create/update entity & concept pages (often 5–15 touches)
5. Update [[../index|index]], optionally [[../overview|overview]]
6. Append [[../log|log]]

## Design preference

Default: **one source at a time**, human in the loop. Batch mode available when requested.
