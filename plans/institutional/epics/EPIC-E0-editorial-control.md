# EPIC E0 — Editorial control and production setup

## Implementation request

Establish the controlled production system for the organic-media program before
drafting or publishing any article or thread. The website remains canonical;
Medium, Substack, GitHub, and optional communities receive reviewed
adaptations only after the canonical source is approved.

## Inputs

- `plans/institutional/organic-media-plan.md`
- `plans/institutional/organic-media-aees.md`
- `governance/evidence-boundaries.md`
- `research/claims-register.md`
- `governance/publication-review-checklist.md`

## Scope and non-goals

In scope: inventory, claims review, canonical-to-external workflow, channel
readiness, and observation logging. Out of scope: publication, outreach,
paid promotion, contacting editors, or changing external profiles without
separate human authorization.

## Sprint E0-S1 — Source of truth and workflow

### E0-S1-T1 — Create the editorial inventory

- Action: map all twelve article topics, two threads per article, owner,
  target week, status, canonical path, and planned adaptations.
- Output: versioned inventory under `plans/institutional/`.
- Depends on: AEES backlog.
- Validate: unique IDs; no topic omitted; no external item lacks a canonical
  source.
- Done when: a reviewer can identify the next production item and its source.

### E0-S1-T2 — Create the claims-review worksheet

- Action: add fields for claim text, type (fact/proposal/hypothesis/future
  work), evidence or `[REFERENCE NEEDED]`, limitation, reviewer, and decision.
- Output: worksheet linked to `research/claims-register.md`.
- Validate: sample all annotations from Articles 1–12; flag unsupported
  metrics, implementation, adoption, security, and performance language.
- Done when: every draft can be reviewed without hidden claim decisions.

### E0-S1-T3 — Define canonical-to-external adaptation flow

- Action: document site-first drafting, review, canonical publication, then
  Medium/Substack adaptation and thread distribution.
- Output: workflow note and article/thread templates.
- Validate: external text cannot be marked ready before canonical approval.
- Done when: the sequence is explicit in the inventory and templates.

### E0-S1-T4 — Create the monthly observation log

- Action: define fields for URL, channel, publication date, status, query or
  preview observation, correction, and reviewer notes.
- Output: empty baseline observation log.
- Validate: no field implies causality or guaranteed search impact.
- Done when: the first month can be recorded without inventing metrics.

## Sprint E0-S2 — Channel readiness

### E0-S2-T1 — Align channel bios

- Action: prepare bounded bios for Medium, Substack, and GitHub using the
  canonical identity and prototype-stage status.
- Output: reviewed bio set; no open-source, enterprise, outcome, or maturity
  claim unless evidenced.
- Validate: compare each bio with `governance/institutional-identity.md`.

### E0-S2-T2 — Verify official channel URLs and ownership

- Action: record the official site, docs, GitHub, Medium, Substack, and Notion
  URLs and the human who verified each one.
- Output: channel verification record.
- Validate: URLs resolve or are explicitly marked pending; ownership is not
  inferred from a link alone.

### E0-S2-T3 — Confirm external publication authorization

- Action: add a human approval gate for each channel and publication batch.
- Output: authorization field in the inventory and review record.
- Validate: no task changes an external service or publishes content.

## Acceptance criteria

- Inventory covers twelve articles and twenty-four threads.
- Claims worksheet, adaptation flow, and observation log exist and are linked.
- Channel URLs and ownership status are recorded.
- No external publication or directed outreach occurs under this EPIC.

## Blockers and escalation

Escalate missing channel access, unclear ownership, absent evidence, or a
request to publish externally to the human project owner. Do not resolve these
by assumption.

## E0 control artifact index

- [Editorial inventory](../editorial-inventory.md) — 12 articles and 24
  canonical-linked threads, owners, weeks, statuses, adaptations, and
  authorization fields.
- [Claims-review worksheet](../claims-review-worksheet.md) — per-claim type,
  evidence, limitation, reviewer, and decision fields, with Article 1–12
  sampling checkpoints.
- [Canonical-to-external adaptation flow](../editorial-adaptation-flow.md) —
  site-first gates and external authorization sequence.
- [Monthly observation log](../observation-log.md) — empty baseline for
  URL/date/status/observation/correction records without causal claims.
- [Channel readiness and authorization](../channel-readiness.md) — bounded
  bios, URL/ownership verification, and channel-specific approval matrix.
