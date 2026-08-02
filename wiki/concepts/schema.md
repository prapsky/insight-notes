---
title: Schema
type: concept
created: 2026-08-01
updated: 2026-08-02
tags: [workflow, meta]
sources: [sources/001-llm-wiki-pattern]
status: active
---

# Schema

The schema is a configuration document. It turns a general-purpose LLM into a **disciplined wiki maintainer**. In this vault, the schema is **`.cursorrules`**.

It defines the folder structure and page rules. These rules cover frontmatter, wikilinks, and file names. It also defines workflows for [[concepts/ingest|ingest]], [[concepts/query-filing|query]], [[concepts/wiki-lint|lint]], and changes to the schema itself.

## Plain language (2026-08-02)

Wiki pages must use **simple, beginner-friendly English**. Short sentences. Explain jargon on first use. Avoid telegraphic bullets and arrow shorthand. This applies to every [[concepts/ingest|ingest]] and to filed query answers. Facts stay precise; only the wording stays plain.

The schema should develop together with the human as the subject becomes clearer. Do not expand it before there is a need.
