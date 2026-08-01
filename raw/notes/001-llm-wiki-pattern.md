# LLM Wiki — A Pattern for Personal Knowledge Bases Using LLMs

> Archived idea file. Immutable source. Ingested as wiki source 001.

## The core idea

Most people's experience with LLMs and documents looks like RAG: you upload a collection of files, the LLM retrieves relevant chunks at query time, and generates an answer. This works, but the LLM is rediscovering knowledge from scratch on every question. There's no accumulation.

The idea here is different. Instead of just retrieving from raw documents at query time, the LLM **incrementally builds and maintains a persistent wiki** — a structured, interlinked collection of markdown files that sits between you and the raw sources. When you add a new source, the LLM reads it, extracts the key information, and integrates it into the existing wiki. The knowledge is compiled once and then *kept current*, not re-derived on every query.

**The wiki is a persistent, compounding artifact.**

## Architecture (three layers)

1. **Raw sources** — immutable curated documents. LLM reads, never modifies.
2. **The wiki** — LLM-generated markdown. Summaries, entities, concepts, synthesis.
3. **The schema** — conventions and workflows (e.g. `.cursorrules`) that make the LLM a disciplined maintainer.

## Operations

- **Ingest** — process a new source into the wiki (summary + entity/concept updates + index + log).
- **Query** — answer from the wiki; file valuable answers back as pages.
- **Lint** — health-check for contradictions, orphans, stale claims, missing pages.

## Indexing and logging

- **index.md** — content catalog by category; read first on queries.
- **log.md** — append-only chronological record with parseable prefixes.

## Why this works

Humans abandon wikis because maintenance burden grows faster than value. LLMs don't get bored and can touch 15 files in one pass. Related in spirit to Vannevar Bush's Memex (1945) — private, curated, associative trails. The LLM solves who does the maintenance.

## Contexts

Personal, research, reading a book, business/team, competitive analysis, due diligence, trip planning, course notes, hobby deep-dives.
