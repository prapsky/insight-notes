# insight-notes

A personal **LLM Wiki** (second brain): immutable sources in `raw/`, an agent-maintained knowledge graph in `wiki/`.

Unlike RAG (chat-with-your-docs), knowledge here is **compiled once and kept current**. Ingest a transcript or essay and the agent updates entities, concepts, cross-links, the index, and the log. Later questions hit synthesis that already exists — not a fresh retrieval pass.

Open this folder in **Obsidian** to browse and follow links. Use **Cursor** (or any agent that reads `.cursorrules`) as the wiki maintainer.

> You source and direct. The LLM does the bookkeeping. The wiki compounds.

---

## What’s in this vault

The wiki is active around:

| Theme | Examples |
|-------|----------|
| Indonesia growth, liquidity, fiscal | Money supply vs rates, FDI climate, middle-class squeeze, tax compliance |
| Governance & soft infrastructure | Teachers, decentralization / mayor economy, ownership society, meritocracy vs patronage |
| AI infra & sovereignty | Electrification threshold, physical vs cryptographic sovereignty, commoditization / lock-in, platform leadership |
| China political economy & US–China | Mayor economy, process/crisis innovation, value creation vs capture |
| Consciousness / media / storytelling | Attention-as-wealth, Techno-Marxism, meaning-full storytelling, innovation theater |
| Knowledge systems (meta) | LLM wiki pattern vs RAG |

**Primary raw material today:** Endgame podcast transcripts under `raw/media/endgame/`, Indrawan Nugroho essays under `raw/media/indrawan-nugroho/`, plus the bootstrap note `raw/notes/001-llm-wiki-pattern.md`. Folders `articles/`, `papers/`, `journals/`, and `assets/` exist but are mostly empty placeholders.

**Approximate inventory** (see `wiki/index.md` for the live catalog):

- 12 source summaries (`wiki/sources/001` … `012`)
- ~19 entity pages, ~46 concept pages
- 1 comparison (`rag-vs-llm-wiki`); `wiki/queries/` ready but unused

Start reading: [`wiki/overview.md`](wiki/overview.md) (synthesis) → [`wiki/index.md`](wiki/index.md) (catalog) → [`wiki/log.md`](wiki/log.md) (what changed when).

---

## Architecture

| Layer | Path | Who owns it |
|-------|------|-------------|
| **Raw sources** | `raw/` | You — immutable. Agent reads, never edits. |
| **Wiki** | `wiki/` | Agent — creates, updates, cross-links. |
| **Schema** | `.cursorrules` | Both — co-evolve conventions over time. |

```
raw/
  articles/   papers/   notes/   journals/   assets/
  media/
    endgame/              # Podcast episode transcripts
    indrawan-nugroho/     # Essay / video transcripts

wiki/
  index.md          Content catalog (start here for queries)
  log.md            Append-only activity timeline
  overview.md       Living high-level synthesis
  entities/         People, orgs, products, places, projects
  concepts/         Ideas, frameworks, themes
  sources/          One summary page per ingested source (NNN-slug.md)
  comparisons/      Explicit compare / contrast pages
  queries/          Filed answers worth keeping
```

---

## Everyday operations

Talk to the agent in plain language:

| Command | What happens |
|---------|----------------|
| **ingest** | Drop a file in `raw/` (or paste text). Agent summarizes, updates related pages, refreshes index + log. |
| **query** | Ask anything. Agent reads `wiki/index.md`, cites pages, and can **file** strong answers into `wiki/queries/` or `wiki/comparisons/`. |
| **lint** | Health-check: contradictions, orphans, stale claims, missing pages, gaps. |
| **explore** | Open-ended brainstorming grounded in the wiki; optional filing. |
| **schema** | Change conventions in `.cursorrules` as the domain evolves. |

Suggested loop: ingest sources one at a time → browse updates in Obsidian → ask questions → file useful answers → lint every so often.

---

## Getting started

1. Open this repo as an Obsidian vault (and/or open it in Cursor).
2. Skim `wiki/overview.md` and `wiki/index.md`.
3. Add a source under `raw/` (e.g. another Endgame transcript in `raw/media/endgame/`).
4. In the agent chat, say: **ingest** `raw/media/endgame/….md`.
5. Follow new links in the graph view.

Bootstrap source: `wiki/sources/001-llm-wiki-pattern.md` documents how the system itself works. Full agent rules: **`.cursorrules`**.

---

## Conventions (short)

- Wiki pages use YAML frontmatter (`title`, `type`, `tags`, `sources`, `status`).
- Links are Obsidian wikilinks: `[[concepts/rag|RAG]]`, `[[entities/indrawan-nugroho|Indrawan]]`.
- Source summaries are numbered: `wiki/sources/001-slug.md`, `002-…`.
- `wiki/log.md` entries look like: `## [YYYY-MM-DD] ingest | Title` (grep-friendly).
- Never edit `raw/`; never invent sources; cite `[[sources/NNN-…]]` for claims.

---

## Optional tooling

- **Obsidian Web Clipper** — save articles into `raw/articles/` as markdown.
- **Graph view** — see hubs, orphans, and how topics connect.
- **Dataview** — query frontmatter if you want dynamic tables.
- **Marp** — slide decks from markdown when you want presentations from wiki content.
- Local search (e.g. [qmd](https://github.com/tobi/qmd)) — optional once the wiki outgrows index-only navigation.
