# Axodus Architecture Paper History

This directory groups historical paper lines and closed worklogs that should
not be treated as the default starting point for new work.

## Usage rule

Read the current paper files in `../` first. Use this directory only when you
need one of the following:

- version-to-version traceability
- prior author or reviewer decisions
- superseded planning records
- historical readiness state

Use `.archive/` only for deeper historical reconstruction after the current
files and this `history/` directory have been exhausted.

## Subdirectories

- `v0.3.2/` — preserved v0.3.2 baseline artifacts and the old internal
  peer-review package wrapper
- `v0.4/` — historical v0.4 and v0.4.1 reframing and review records
- `v0.5-worklog/` — closed v0.5 planning, patch-planning, and internal-review
  workflow artifacts

## Current vs history

Current baseline and control files remain in `../`:

- [`../paper.md`](../paper.md)
- [`../paper.tex`](../paper.tex)
- [`../references.bib`](../references.bib)
- [`../publication-readiness.md`](../publication-readiness.md)
- [`../author-decision-record-v0.5.md`](../author-decision-record-v0.5.md)
- [`../v0.5-closure-readiness-audit.md`](../v0.5-closure-readiness-audit.md)
- [`../v0.5-baseline-closure-record.md`](../v0.5-baseline-closure-record.md)
- [`../v0.5-internal-review-package.md`](../v0.5-internal-review-package.md)

Everything in `history/` is retained for traceability, not as the default
active manuscript surface.
