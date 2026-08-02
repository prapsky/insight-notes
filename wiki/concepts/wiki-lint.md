---
title: Wiki Lint
type: concept
created: 2026-08-01
updated: 2026-08-02
tags: [workflow, operations, quality]
sources: [sources/001-llm-wiki-pattern]
status: active
---

# Wiki Lint

Wiki lint is an operation that performs a regular **health check** of the knowledge base.

## Checks

- Contradictions between pages
- Old claims that newer sources have replaced
- Orphan pages with few links pointing to them
- Concepts that appear many times but do not have their own page
- Missing cross-references
- Incomplete pages that existing sources could fill, and missing data
- Differences between the index and the files that actually exist
- An overview that is out of date

The lint can also suggest new questions and sources. Apply fixes when the human approves them, or when the human asks to "lint and fix."
