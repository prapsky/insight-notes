# insight-notes

A personal **LLM Wiki** — a second brain where an AI agent maintains a persistent, interlinked markdown knowledge base, and you curate sources and ask questions.

Unlike RAG (chat-with-your-docs), knowledge here is **compiled once and kept current**. When you add a source, the agent integrates it across entity pages, concept summaries, and cross-references. Ask a question later and the synthesis is already there — not rediscovered from scratch.

Open this folder in **Obsidian** to browse and follow links. Use **Cursor** (or another agent that reads `.cursorrules`) as the wiki maintainer.

---

## Idea in one line

> You source and direct. The LLM does the bookkeeping. The wiki compounds.

## Architecture

| Layer | Path | Who owns it |
|-------|------|-------------|
| **Raw sources** | `raw/` | You — immutable. Agent reads, never edits. |
| **Wiki** | `wiki/` | Agent — creates, updates, cross-links. |
| **Schema** | `.cursorrules` | Both — co-evolve conventions over time. |

```
raw/
  articles/   papers/   notes/   journals/   media/   assets/

wiki/
  index.md          Content catalog (start here for navigation)
  log.md            Append-only activity timeline
  overview.md       Living high-level synthesis
  entities/         People, orgs, products, places, projects
  concepts/         Ideas, frameworks, themes
  sources/          One summary page per ingested source
  comparisons/      Explicit compare / contrast pages
  queries/          Filed answers worth keeping
```

---

## Everyday operations

Talk to the agent in plain language:

| Command | What happens |
|---------|----------------|
| **ingest** | Drop a file in `raw/` (or paste text). Agent summarizes, updates related pages, refreshes index + log. |
| **query** | Ask anything. Agent reads `wiki/index.md`, cites pages, and can **file** strong answers back into the wiki. |
| **lint** | Health-check: contradictions, orphans, stale claims, missing pages, gaps. |
| **schema** | Change conventions in `.cursorrules` as your domain evolves. |

Suggested loop: ingest sources one at a time → browse updates in Obsidian → ask questions → file useful answers → lint every so often.

---

## Getting started

1. Open this repo as an Obsidian vault (and/or open it in Cursor).
2. Skim `wiki/overview.md` and `wiki/index.md`.
3. Add a source under `raw/` (e.g. `raw/articles/my-piece.md`).
4. In the agent chat, say: **ingest** `raw/articles/my-piece.md`.
5. Follow the new links in the graph view.

The vault already includes a bootstrap ingest of the LLM Wiki pattern itself (`wiki/sources/001-llm-wiki-pattern.md`) so the system documents how it works.

---

## Conventions (short)

- Wiki pages use YAML frontmatter (`title`, `type`, `tags`, `sources`, `status`).
- Links are Obsidian wikilinks: `[[concepts/rag|RAG]]`.
- Source summaries are numbered: `wiki/sources/001-slug.md`, `002-…`.
- `wiki/log.md` entries look like: `## [YYYY-MM-DD] ingest | Title` (grep-friendly).
- Full rules live in **`.cursorrules`** — the agent follows that file every session.

---

## Optional tooling

- **Obsidian Web Clipper** — save articles into `raw/` as markdown.
- **Graph view** — see hubs, orphans, and how topics connect.
- **Dataview** — query frontmatter if you want dynamic tables.
- **Marp** — slide decks from markdown when you want presentations from wiki content.
- Local search (e.g. [qmd](https://github.com/tobi/qmd)) — optional once the wiki outgrows index-only navigation.

---

## Why this works

Maintaining a wiki by hand fails because cross-references and consistency don’t scale. An LLM can touch many pages in one pass and doesn’t skip the boring updates. Your job is judgment: what to read, what to emphasize, what questions matter.
