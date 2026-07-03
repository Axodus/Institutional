# Axodus Architecture Paper — Internal Peer Review Package

Package date: 2026-07-03  
Manuscript version: draft v0.3.2
Review classification: confidential internal peer review only  
External distribution: prohibited

## Purpose

This package supports a controlled internal peer review of the Axodus
architecture paper. The review should test whether the manuscript presents a
clear, coherent, and defensible prototype-stage conceptual architecture
centered on traceability and accountability in human–AI-assisted digital
institutions.

This package is not a publication package. It does not authorize controlled
external review, publication, submission, outreach, grant use, fundraising
use, external distribution, or authority signaling.

## Version lock

Reviewers should confirm that they are reviewing the following exact source
files:

| File | SHA-256 |
|---|---|
| `paper.md` | `4979e187ffea34e48b809d5ea64b798033a7f06f481c9a9982a1dbdd1ad701c2` |
| `paper.tex` | `905ad8f8ca70102c7d6623a4cb494ca063b5d516fce875fd21019f91d4658542` |
| `references.bib` | `9a29faddd4188fcbb87ebbc39e213806eadefecc420fb60d66cef048bf93b5c5` |

If a hash differs, the reviewer should stop and request a confirmed review
copy. Review findings must identify the manuscript version reviewed.

## Files to share with every internal reviewer

The controlled core package consists of:

1. `internal-peer-review-package.md` as the package manifest;
2. `paper.md` as the primary review manuscript;
3. `references.bib` for citation inspection;
4. `internal-peer-review-instructions.md`;
5. `internal-peer-review-form.md`;
6. `v0.3.2-readiness-record.md`;
7. `governance/evidence-boundaries.md`;
8. `governance/maturity-taxonomy.md`; and
9. `research/bibliography-verified.md`.

`paper.tex` may be shared instead of, or alongside, `paper.md` when the
reviewer needs the typeset-source form. It is substantively synchronized with
the Markdown manuscript.

## Files to share only when specifically needed

The following files provide editorial or policy context but are not required
for every reviewer:

| File | Share when needed for |
|---|---|
| `publication-readiness.md` | blocker history, release-risk review, or readiness audit |
| `v0.3.2-change-log.md` | focused comparison with v0.3.1 or review of the targeted patch |
| `governance/citation-policy.md` | citation-governance or metadata review |
| `governance/ip-boundaries.md` | IP, disclosure, or sensitive-detail review |
| `research/terminology.md` | terminology consistency or internal/public vocabulary review |
| `research/related-work.md` | comparison between the manuscript and the internal literature synthesis |
| `research/bibliography-candidates.md` | assigned literature-gap analysis only |

`research/bibliography-candidates.md` contains unverified leads. It must not be
treated as a citable bibliography or supplied as evidence that a literature
gap has been closed.

## Files not to share by default

Do not share the following unless a named reviewer has a specific, approved
need:

- claims registers beyond the exact evidence-boundary excerpts needed for a
  disputed statement;
- superseded manuscript drafts and historical review artifacts;
- repository-wide task, roadmap, status, or handoff documents;
- private implementation, infrastructure, security, financial, treasury, or
  operational materials;
- credentials, access details, private repository information, source code,
  internal prompts, or sensitive intellectual property;
- contact lists, reviewer identities, or another reviewer's report.

When additional context is requested, provide the smallest relevant excerpt or
file. Absence of a confidentiality label does not make repository content
shareable.

## Review questions

Reviewers should answer the following questions with section references and a
severity rating where a problem is identified.

### Contribution and focus

1. Is the central contribution stated clearly and consistently?
2. Does the paper remain centered on traceability and accountability in
   human–AI-assisted digital institutions?
3. Do participation readiness, maturity, risk, and modularity remain
   supporting elements rather than competing contributions?
4. Is the paper's classification as a prototype-stage conceptual architecture
   and research agenda credible?

### Architecture substance

5. Do the functional component classes in Section 4.3 provide enough
   architectural substance?
6. Are authority, evidence, AI-assistance provenance, decision rationale,
   conflict disclosure, risk boundaries, and review or appeal paths
   sufficiently differentiated?
7. Are the relationships among those classes clear enough to reconstruct a
   proposed decision path?
8. Does any component description imply a real module inventory,
   implementation, enforcement, or operational capability?

### Maturity taxonomy

9. Is the distinction between L-Level and D-Level understandable?
10. Is it clear that L-Level does not measure code, D-Level does not measure
    governance, and neither dimension grants production status or sensitive
    authority?
11. Does the short manuscript treatment clarify the architecture, or does it
    distract from the central contribution?
12. Could any wording make the internal taxonomy appear empirically validated?

### Evidence and overclaiming

13. Are design proposals, hypotheses, supported facts, internal taxonomy, and
    future work distinguishable?
14. Does any sentence imply implementation, operational maturity, users,
    adoption, validated security, effectiveness, or comparative superiority?
15. Are prototype-stage and evidence limitations sufficiently clear without
    making the manuscript excessively defensive?
16. Does any statement exceed `governance/evidence-boundaries.md`?

### Terminology

17. Are `digital institution`, `constitutional governance`, `traceability`,
    `accountability`, `contestability`, and `participation readiness` used
    consistently?
18. Does any internal Axodus terminology or financial interpretation leak into
    the manuscript?
19. Are potentially exclusionary implications of participation readiness
    stated and bounded adequately?

### Methodology and evaluation

20. Is the controlled simulated environment a credible prerequisite for RQ1
    and RQ3?
21. Are the proposed scenarios, evidence packages, simulated AI records,
    planted errors, reviewer tasks, and interface strategy sufficient to make
    the studies interpretable?
22. Are the proposed measures aligned with traceability, accountability, and
    calibrated human reliance?
23. Does the evaluation plan avoid implying an existing platform, completed
    experiment, recruited reviewers, or empirical result?
24. What additional controls, baselines, validity threats, or preregistration
    details are essential before a study protocol is written?

### Literature and readiness risk

25. Which claims need stronger citation support?
26. Which missing literature is essential before any controlled external
    review?
27. Are the remaining gaps in contestability, calibrated reliance, assessment
    validity, DAO participation, maturity-model reliability, or Web3
    regulation material to this manuscript's narrowed contribution?
28. Does each cited source support the proposition for which it is used?
29. What publication-readiness risks remain even if the manuscript is
    internally accepted?
30. What is the smallest set of revisions required before the next internal
    readiness assessment?

## Recommended reviewer profile

A complete internal review should include two to four reviewers with
complementary expertise:

- a socio-technical systems or institutional-governance reviewer;
- a human–AI interaction, calibrated-reliance, or evaluation-methods reviewer;
- a systems-architecture, traceability, auditability, or assurance reviewer;
- optionally, a decentralized-governance, contestability, credentialing, or
  regulatory specialist for the supporting sections.

Reviewers should be able to distinguish conceptual architecture from
implementation evidence and should not have direct authorship responsibility
for the passages they primarily assess. Conflicts of interest, prior project
involvement, and limits of expertise must be disclosed in the review form.

## Package control

The package owner should:

- assign each copy to a named internal reviewer;
- record the exact files and hashes supplied;
- use an approved private transfer and return channel;
- set a return or deletion date;
- avoid public links, public issue trackers, and unrestricted shared drives;
- collect completed forms without exposing reviewer identities to other
  reviewers unless explicitly approved; and
- record findings before considering any manuscript or readiness change.

No review result, including a favorable result, changes the current external
publication blockers automatically.
