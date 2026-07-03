# Publication Readiness — Axodus Architecture Paper

Review date: 2026-07-03  
Version reviewed: draft v0.3  
Decision: **Ready for author review only; not ready for controlled external
review, publication, submission, outreach, grant use, or external
distribution.**

## Publication status

Ready for human review: yes  
Ready for public publication: no

## Phase 1.2 author-gate status

Phase 1.2 recorded the human internal review verdict and converted it into an
author gate rather than a circulation step.

Human internal review verdict:

- category: internal working paper;
- suitable for serious author review;
- not ready for external academic review;
- do not publish or use for institutional/public authority signaling;
- publication risk if released now: moderate to high.

Phase 1.2 also established a v0.2 editorial direction: narrow the title,
rewrite the abstract and introduction around a clearer research gap, and keep
the PoK-tokenomics relationship out of scope for the architecture paper.

## Phase 1.3 author-decision status

Phase 1.3 recorded the approved v0.2 author-direction decisions in
`author-decision-record-v0.2.md`.

Recorded decisions now include:

- v0.2 title direction must explicitly signal prototype-stage conceptual
  architecture;
- `Proof of Knowledge` remains internal Axodus terminology and should not be
  the primary public academic term;
- paper-facing terminology should prefer descriptive phrases such as
  `knowledge-gated participation` or `educational participation mechanism`;
- `Academy` should be replaced in manuscript-facing text with
  `educational layer` or `learning and credentialing layer`, except when named
  explicitly as an internal label;
- the relationship between educational participation, `$Neurons`, token
  minting, supply, scarcity, incentives, and tokenomics is out of scope for
  this paper;
- `Learn to Win` is not approved for academic or public brand use before legal
  review;
- the paper remains blocked from publication, outreach, grants, fundraising,
  and authority signaling.

## Phase 1.4 v0.2 rewrite status

Phase 1.4 completed an internal v0.2 manuscript rewrite in `paper.md` and
`paper.tex` under the approved author-decision constraints.

The rewrite:

- narrowed the title to explicitly signal prototype-stage conceptual
  architecture;
- rewrote the abstract and introduction around a clearer integrative research
  gap;
- replaced most public-facing `Proof of Knowledge` language with descriptive
  functional terminology while retaining one internal-label note;
- replaced manuscript-facing `Academy` language with `educational layer`;
- removed treasury-centered framing and made token-linked or financial design
  questions explicitly out of scope.

The rewritten LaTeX manuscript compiled successfully after the Phase 1.4
changes, and generated build artifacts were cleaned.

The rewrite did not add new references, did not change the publication
blockers, and did not authorize circulation.

## Phase 1.6 v0.3 planning status

Phase 1.6 recorded the internal review verdict on v0.2 and defined a v0.3
editorial direction in `v0.3-editorial-plan.md` and
`v0.3-author-review-record.md`.

The v0.2 internal review verdict is:

- v0.2 is a good internal working paper;
- v0.2 is substantially improved over v0.1;
- v0.2 is not ready for controlled external review or publication;
- v0.2 still has weaknesses in bibliography, contribution unity,
  methodological prioritization, and external validation.

The approved v0.3 direction is to narrow the dominant contribution axis to
traceability and accountability in human-AI-assisted digital institutions.
Participation readiness, maturity separation, risk boundaries, and governance
should remain as supporting components rather than co-equal contributions.

## Phase 1.7 v0.3 rewrite status

Phase 1.7 completed the internal v0.3 manuscript rewrite in `paper.md` and
`paper.tex` and recorded the rewrite in `v0.3-change-log.md`.

The v0.3 rewrite:

- retitled the manuscript to foreground traceability and accountability in
  human-AI-assisted digital institutions;
- rewrote the abstract and introduction around a narrower traceability and
  accountability contribution;
- rebalanced related-work framing toward human-AI oversight, calibrated
  reliance, contestability, and institutional reviewability;
- repositioned participation readiness, maturity separation, and risk
  boundaries as supporting components rather than co-equal contributions;
- reordered the evaluation plan so RQ1 is the primary initial study and RQ3
  is the secondary initial study, with RQ2, RQ4, and RQ5 treated as future
  work;
- strengthened the limitations section, including the explicit statement that
  the proposed architecture may be too complex to govern in practice without
  substantial scope reduction.

The rewritten LaTeX manuscript compiled successfully after the Phase 1.7
changes, and generated build artifacts were cleaned.

The rewrite did not add new verified references, did not change the evidence
boundaries, and did not authorize circulation.

## Phase 1.8 v0.3 author-review support status

Phase 1.8 completed internal author-review support for the v0.3 manuscript in
`v0.3-author-review-brief.md` and `v0.3-author-review-checklist.md`.

The support review concluded that:

- v0.3 is materially more unified than v0.2 around traceability and
  accountability;
- the manuscript is suitable for serious author review;
- related work is sufficient for author review but not yet sufficient for
  controlled external review;
- the evaluation plan is now narrow enough for author review, though still
  broader than an externally reviewable article would ideally be;
- the limitations section is strong enough for author review;
- residual editorial drift remains in the relative weight of the supporting
  sections on participation readiness, maturity, risk boundaries, and the
  broader research agenda.

The Phase 1.8 recommendation is: **ready for author approval after minor
edits**, while remaining internal and blocked from controlled external review
and publication.

## Phase 1.1 review status

Phase 1.1 critical editorial review was completed on 2026-07-03. A skeptical
reviewer pass was recorded in `reviewer-report.md`.

Small manuscript hardening edits were applied in both manuscript forms:

- the participation/legitimacy wording was qualified from `supports` to
  `may support`;
- the limitations section now explicitly names Web3 regulatory uncertainty,
  operational fragility, and AI reliability/auditability risks.

These edits did not alter the manuscript's controlled evidence boundaries or
publication blockers.

## Implementation summary

Phase 1 created a documentation-only editorial foundation, evidence controls,
research records, a verified/candidate bibliography split, and structurally
equivalent Markdown and LaTeX manuscript sources.

The manuscript presents Axodus as a conceptual, prototype-stage architecture
and research agenda. It reports no implementation, users, empirical results,
security properties, financial performance, or operational maturity.

## Files created

- `AGENTS.md`
- `CONTRIBUTING.md`
- `LICENSE-CONTENT`
- `governance/citation-policy.md`
- `governance/evidence-boundaries.md`
- `governance/ip-boundaries.md`
- `governance/publication-review-checklist.md`
- `research/claims-register.md`
- `research/gaps.md`
- `research/terminology.md`
- `research/related-work.md`
- `research/bibliography-candidates.md`
- `research/bibliography-verified.md`
- `papers/axodus-architecture-paper/paper.md`
- `papers/axodus-architecture-paper/paper.tex`
- `papers/axodus-architecture-paper/references.bib`
- `papers/axodus-architecture-paper/publication-readiness.md`
- `papers/axodus-architecture-paper/v0.2-change-log.md`
- `papers/axodus-architecture-paper/v0.3-editorial-plan.md`
- `papers/axodus-architecture-paper/v0.3-author-review-record.md`
- `papers/axodus-architecture-paper/v0.3-change-log.md`
- `papers/axodus-architecture-paper/v0.3-author-review-brief.md`
- `papers/axodus-architecture-paper/v0.3-author-review-checklist.md`
- `whitepaper/README.md`
- `articles/README.md`
- `outreach/README.md`

## Files modified

- `README.md`

The existing software `LICENSE` was not modified. No commit, push, pull
request, submission, publication, or external contact was performed.

## Verification performed

- Markdown and LaTeX headings were compared and are structurally equivalent.
- Both manuscript forms cite the same eight BibTeX keys.
- Every BibTeX entry is cited; no duplicate keys or unused entries were found.
- `git diff --check` found no whitespace errors in the Phase 1 changes.
- The manuscript contains no `[REFERENCE NEEDED]` marker.
- Searches were run for promotional superlatives, investment-return language,
  operational claims, common credential patterns, private keys, and repository
  URLs.
- Matches outside the manuscript were policy examples, prohibited-language
  lists, or blocked claims; no apparent secret or sensitive implementation
  detail was found.
- Proof of Knowledge is explicitly distinguished from cryptographic proofs of
  knowledge in the terminology file and both manuscript forms.
- A skeptical academic review was completed and documented in
  `reviewer-report.md`.
- A LaTeX compile check was completed successfully and documented in
  `latex-compile-check.md`.
- The v0.2 rewrite was summarized in `v0.2-change-log.md`.

## Bibliographic status

Eight cited sources have verification records. Metadata was checked against
publisher, journal, institutional, standards-body, or canonical preprint
records.

## References needing verification

All cited sources require a final metadata recheck before any submission or
public release because preferred citation formats and canonical records can
change.

The following research areas remain candidates and are not cited:

- deliberative and informed participation;
- automation bias and calibrated reliance;
- contestable automated decisions;
- empirical DAO voting and delegation;
- educational assessment validity and equity;
- maturity-model reliability.

All bibliographic metadata must be rechecked before submission. Venue-specific
formatting has not been applied.

## Remaining citation risks

- The verified bibliography is still thin for deliberative competence,
  contestability and appeals, educational assessment validity, DAO
  participation behavior, and Web3 regulatory constraints.
- Additional candidate work is now explicitly tracked for calibrated reliance,
  appeals, assessment validity, DAO participation behavior, maturity-model
  reliability, and Web3 regulatory constraints.
- Those literatures should remain in `research/bibliography-candidates.md`
  until primary-source metadata is verified.
- No additional references should enter `references.bib` until they are both
  verified and actually needed by the manuscript.
- Related-work adequacy is now sufficient for author review but still below
  the threshold for controlled external review.

## Claims blocked

The current controls block:

- a precise project duration;
- the number, identity, or maturity of Axodus cores;
- any claim of a functioning or integrated implementation;
- users, adoption, partners, endorsements, or measured impact;
- security, reliability, or risk-control effectiveness;
- treasury operation, token mechanics, or financial performance;
- comparative novelty or superiority;
- Harmony or any other external project as validation of Axodus.

The only historical wording admitted to the manuscript is: “The project
originates from a multi-year independent research and design effort.”

## Unresolved blockers

1. Replace `[public contact to be added]` with a reviewed public
   correspondence address.
2. Obtain author approval for name, affiliation, title, abstract, and release
   license.
3. Resolve whether the paper should remain one broad architecture manuscript
   or be narrowed before any external review.
4. Complete substantive review by independent readers with relevant expertise
   in socio-technical systems, governance, human–AI interaction, education,
   decentralized systems, and risk.
5. Verify that every Axodus-specific statement conforms to the intended public
   disclosure boundary.
6. Review the CC BY 4.0 licensing notice and third-party rights before release.
7. Select a venue and apply its authorship, disclosure, formatting, and
   submission requirements in a separate phase.

## Critical editorial blockers

- Related-work coverage remains insufficient for controlled external review in
  contestability and appeals, assessment validity, deliberative competence,
  calibrated reliance, DAO participation behavior, maturity-model reliability,
  and Web3 regulatory constraints.
- Even after narrowing, the paper remains broader than a strong external
  article and still needs sharper contribution discipline before any
  controlled external review is considered.
- The evaluation plan is now prioritized, but the paper still lacks empirical
  evidence, operational evidence, and independently challenged validation of
  its core constructs.
- The manuscript now states that the architecture may be too complex to govern
  in practice without substantial scope reduction; that limitation remains a
  live blocker rather than a resolved concern.
- Residual interpretive risk remains around the internal `Proof of Knowledge`
  note and visible out-of-scope token terminology, even though both are now
  properly bounded.

## Editorial risks

- **Breadth:** the paper spans governance, education, AI, and decentralized
  finance; reviewers may find its contribution insufficiently narrow.
- **Evidence:** the architecture has no empirical evaluation or public
  implementation evidence.
- **Terminology:** “Proof of Knowledge” may still be confused with the
  cryptographic term despite the explicit disclaimer.
- **Legitimacy:** educational gating can create exclusion, curriculum capture,
  and privacy harms.
- **Oversight:** “human in the loop” can become nominal without authority,
  competence, time, and accountability.
- **Maturity:** L0–L5 and D0–D5 remain labels without validated level
  definitions.
- **Single-author perspective:** the model may encode institutional assumptions
  that have not been independently challenged.

## Non-critical recommendations

- Keep the v0.3 manuscript centered on traceability, accountability, and
  bounded human-AI assistance in any subsequent revision.
- Preserve participation readiness, maturity, and risk boundaries as
  supporting components rather than expanding them again into co-equal
  contributions.
- Keep RQ2, RQ4, and RQ5 in future-work territory unless a later draft
  narrows them substantially.
- Compress supporting sections further if a later draft is intended to read as
  a single-article contribution rather than a broader program statement.
- Expand the candidate bibliography first, then verify and integrate only the
  sources that materially strengthen the narrowed v0.3 argument.

## IP/licensing risks

- The placeholder correspondence field must be replaced with an approved public
  contact before release.
- The CC BY 4.0 notice and any venue-specific licensing constraints require
  human approval before publication.
- Third-party rights must be rechecked for any future figures, excerpts, or
  formatting assets added after Phase 1.

## Remaining IP/licensing risks

- External review circulation still requires a deliberate decision on what
  affiliation, contact, and release terms are appropriate.
- If the manuscript is narrowed or re-titled, any future venue-specific
  metadata and rights language must be rechecked separately.

## Author decisions required

- Keep one broad architecture paper or split into narrower papers.
- Choose the next review mode: author review only or controlled external
  review after revision.
- Approve the public correspondence address, affiliation wording, and license
  posture for any later circulation.

The terminology and no-tokenomics boundary decisions for v0.2 have now been
recorded and may be treated as approved for manuscript-editing purposes.

## Recommended next human review

Conduct an author-level editorial review against `reviewer-report.md`,
`author-review-brief.md`, `v0.2-editorial-plan.md`, and
`author-decision-record-v0.2.md` before any circulation decision. The v0.3
rewrite should now be reviewed against `v0.3-editorial-plan.md`,
`v0.3-author-review-record.md`, `v0.3-change-log.md`,
`v0.3-author-review-brief.md`, and `v0.3-author-review-checklist.md`, but
circulation remains blocked.

## Checklist status

The automated/static portions of the publication checklist were executed.
Human judgment items remain unchecked in
`../../governance/publication-review-checklist.md`.
Checklist applied: yes, for the automated/static checks completed in Phase 1.

## Readiness status

Phase 1.8 readiness category: **Ready for author review only.**

Ready for controlled external review: no  
Ready for public publication: no

v0.3 manuscript edits authorized: yes  

**Current status: v0.3 internal rewrite complete; author-review support
complete; ready for author review only; blocked for controlled external
review and publication.**
