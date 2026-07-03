# Bibliography Hardening Plan

Planning date: 2026-07-03  
Scope: candidate-literature hardening plan before any verified bibliography or
manuscript-bibliography expansion

## Objective

Define which literature gaps matter most to the current v0.3 manuscript,
which manuscript claims they support, what kinds of sources are needed, and
which gaps are mandatory before any controlled external review is considered.

## Ground rules

- Do not add any unverified source to `references.bib`.
- Do not promote any candidate source to the verified bibliography without
  metadata confirmation against a primary academic, publisher, standards, or
  institutional record.
- Do not expand the manuscript's ambition to justify more citations; use the
  bibliography to support the narrowed v0.3 paper.

## Gap-to-manuscript map

| Gap | Primary manuscript sections | Key lines | Why the gap matters |
|---|---|---:|---|
| Contestability and appeals | `1. Introduction`, `3. Problem Statement`, `7. Governance, Accountability, and Human Oversight`, `11. Limitations` | 53-55, 140-143, 294-297, 384-389 | The paper now treats contestability as a central accountability requirement, so it needs a stronger academic and governance basis |
| Calibrated reliance | `2.3 Human-AI oversight`, `10. Evaluation Plan`, `11. Limitations` | 110-118, 351-356, 384-388 | RQ3 and the limitations section rely on calibrated-reliance concepts that are only lightly grounded today |
| Deliberative competence | `3. Problem Statement`, `6. Participation Readiness`, `12. Research Agenda` | 149-150, 272-279, 410-415 | If participation readiness remains in the paper, it needs better grounding in competence, participation quality, and exclusion tradeoffs |
| Assessment validity | `2.4 Credentials`, `6. Participation Readiness`, `11. Limitations` | 128-132, 266-279, 391-395 | The paper distinguishes machine verification from educational legitimacy, but needs stronger support for that distinction |
| DAO governance participation | `2.2 Decentralized governance`, `10. Evaluation Plan`, `12. Research Agenda` | 97-108, 361-368, 413-415 | If DAO governance remains part of the paper's motivating context, it needs empirical grounding on participation and governance behavior |
| Maturity-model reliability | `5. Modularity and Maturity`, `10. Evaluation Plan`, `12. Research Agenda` | 224-245, 364-365, 408-409 | The paper keeps the L/D distinction, so reliability literature is needed if that section remains visible |
| Web3 regulatory constraints | `8. Risk Boundaries`, `11. Limitations` | 319-323, 397-398 | The paper names Web3-facing regulatory and operational risk and therefore needs a stronger non-promotional legal or institutional basis |

## Source-type requirements by gap

| Gap | Source types needed |
|---|---|
| Contestability and appeals | foundational academic reference; governance/legal framework; survey paper |
| Calibrated reliance | foundational academic reference; recent empirical study; survey paper; methodological reference |
| Deliberative competence | foundational academic reference; survey paper; recent empirical study |
| Assessment validity | foundational academic reference; standards document; survey paper; methodological reference |
| DAO governance participation | recent empirical study; survey paper; methodological reference |
| Maturity-model reliability | foundational academic reference; recent empirical study; methodological reference |
| Web3 regulatory constraints | governance/legal framework; recent empirical study; survey paper |

## Prioritization

### Must close before controlled external review

- Contestability and appeals
  Reason: now part of the paper's central accountability claim.
- Calibrated reliance
  Reason: directly supports the human-AI oversight framing and RQ3.
- Assessment validity
  Reason: needed if participation readiness remains in the manuscript even as a supporting mechanism.
- DAO governance participation
  Reason: supports the manuscript's decentralized-governance context and helps keep governance framing from floating at a purely conceptual level.
- Web3 regulatory constraints
  Reason: already named in limitations and out-of-scope risk framing.

### Should close before publication

- Deliberative competence
  Reason: important for a stronger treatment of participation quality and exclusion, but less central if the participation-readiness section is compressed further.
- Maturity-model reliability
  Reason: important if the maturity section remains visible, but potentially lower priority if that section is heavily shortened in the next pass.

## Conditional priority note

If the next minor-edit pass keeps `Modularity and Maturity as Supporting
Controls` as a full standalone section, then maturity-model reliability should
be reclassified from `should close before publication` to `must close before
controlled external review`.

If the next minor-edit pass keeps the participation-readiness section at or
near its current length, then deliberative competence should be reclassified
from `should close before publication` to `must close before controlled
external review`.

## Recommended verification sequence

1. Contestability and appeals
2. Calibrated reliance
3. Assessment validity
4. DAO governance participation
5. Web3 regulatory constraints
6. Deliberative competence
7. Maturity-model reliability

This sequence follows the current argumentative hierarchy of the v0.3 paper.

## Candidate-literature collection instructions

- Prefer one high-value verified source per gap before expanding breadth.
- Prefer sources that directly support the manuscript's actual wording rather
  than broad adjacent literatures.
- Prefer empirical or review work over advocacy or market commentary for DAO
  and Web3 topics.
- Prefer jurisdiction-neutral or cross-jurisdictional legal/governance work
  for contestability and Web3-regulation issues.
- Keep candidate collection in `research/bibliography-candidates.md` until
  metadata is verified.

## Recommended next action

Proceed with a manuscript minor-edit pass and a parallel candidate-source
verification workflow. Do not wait for a complete bibliography expansion to
start compression edits, but do not move toward controlled external review
until the `must close` gaps are materially addressed.
