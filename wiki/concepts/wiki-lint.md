---
title: Wiki Lint
type: concept
created: 2026-08-01
updated: 2026-08-01
tags: [workflow, operations, quality]
sources: [sources/001-llm-wiki-pattern]
status: active
---

# Wiki Lint

Wiki operation: periodic **health-check** of the knowledge base.

## Checks

- Contradictions between pages
- Stale claims superseded by newer sources
- Orphan pages (weak inbound links)
- Repeated concepts lacking their own page
- Missing cross-references
- Fillable stubs / data gaps
- Index drift vs actual files
- Overview out of date

Suggest new questions and sources. Apply fixes when the human approves (or on "lint and fix").
