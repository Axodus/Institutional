# Axodus Institutional Index

This is the canonical navigation map for agents and humans working in this
repository.

- `README.md` explains the repository at a high level.
- `AGENTS.md` defines mandatory workflow and editorial constraints.
- `index.md` defines safe reading order, source-of-truth routing, and where to
  look first.

## Read First

1. [AGENTS.md](AGENTS.md)
2. [governance/evidence-boundaries.md](governance/evidence-boundaries.md)
3. [governance/public-disclosure-boundary.md](governance/public-disclosure-boundary.md)
4. [README.md](README.md)

## Task-Based Reading Paths

### If you will edit public text

1. [AGENTS.md](AGENTS.md)
2. [governance/evidence-boundaries.md](governance/evidence-boundaries.md)
3. [research/claims-register.md](research/claims-register.md)
4. The target directory README or index

### If you will work on the architecture paper

1. [papers/axodus-architecture-paper/README.md](papers/axodus-architecture-paper/README.md)
2. [papers/axodus-architecture-paper/publication-readiness.md](papers/axodus-architecture-paper/publication-readiness.md)
3. [papers/axodus-architecture-paper/paper.md](papers/axodus-architecture-paper/paper.md)
4. [papers/axodus-architecture-paper/paper.tex](papers/axodus-architecture-paper/paper.tex)

### If you will work on citations or references

1. [governance/citation-policy.md](governance/citation-policy.md)
2. [research/bibliography-verified.md](research/bibliography-verified.md)
3. [papers/axodus-architecture-paper/references.bib](papers/axodus-architecture-paper/references.bib)

### If you need controlled terminology

1. [research/terminology.md](research/terminology.md)
2. The current manuscript readiness or directory README

### If you need disclosure or IP boundaries

1. [governance/public-disclosure-boundary.md](governance/public-disclosure-boundary.md)
2. [governance/ip-boundaries.md](governance/ip-boundaries.md)

## Repository Map

- `governance/` — editorial controls, disclosure limits, citation policy, IP
  boundaries, maturity taxonomy, and review checklist
- `research/` — claims, terminology, gaps, related work, and bibliography
- `papers/` — manuscript baselines, readiness records, and historical tracks
- `whitepaper/`, `articles/`, `outreach/` — deferred-phase indexes only

## Source-of-Truth Rules

Use this precedence when reading:

1. current baseline files in the target directory
2. current readiness and control records
3. `history/` for traceability and prior decisions
4. `.archive/` only when a current file explicitly points there or when the
   task is historical reconstruction

Do not treat `history/` or `.archive/` as the default starting point when a
current baseline exists.

## Agent Search Rules

- Start with `index.md`, then local `README.md`, then `AGENTS.md`.
- Search current directories before `history/`.
- Search `.archive/` only when the current state does not answer the question
  or when the task explicitly asks for historical traceability.
- For the paper, prefer top-level current files in
  `papers/axodus-architecture-paper/` before any `history/` or `.archive/`
  material.

## Current Paper Status Snapshot

The current architecture-paper state is:

- `v0.5` = closed internal baseline
- controlled external review = blocked
- publication = blocked
- submission = blocked
- external circulation = blocked

See
[papers/axodus-architecture-paper/publication-readiness.md](papers/axodus-architecture-paper/publication-readiness.md)
for the authoritative status.

## Deferred Areas

The following remain deferred and should not be treated as active delivery
tracks:

- whitepaper drafting
- derived articles
- outreach and external contact
- publication package preparation
- broad bibliography expansion
