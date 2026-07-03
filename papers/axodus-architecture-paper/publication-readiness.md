# Publication Readiness — Axodus Architecture Paper

Review date: 2026-07-03  
Version reviewed: draft v0.1  
Decision: **Ready for author review only; not ready for controlled external
review, publication, submission, outreach, grant use, or external
distribution.**

## Publication status

Ready for human review: yes  
Ready for public publication: no

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
- Those literatures should remain in `research/bibliography-candidates.md`
  until primary-source metadata is verified.
- No additional references should enter `references.bib` until they are both
  verified and actually needed by the manuscript.

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
4. Decide whether `Proof of Knowledge` remains an acceptable public term or
   should be replaced before external circulation.
5. Clarify whether `Academy` is a public generic component label or an
   Axodus-specific term that should be removed or rephrased.
6. Complete substantive review by independent readers with relevant expertise
   in socio-technical systems, governance, human–AI interaction, education,
   decentralized systems, and risk.
7. Verify that every Axodus-specific statement conforms to the intended public
   disclosure boundary.
8. Review the CC BY 4.0 licensing notice and third-party rights before release.
9. Select a venue and apply its authorship, disclosure, formatting, and
   submission requirements in a separate phase.

## Critical editorial blockers

- The introduction and abstract still need a sharper statement of research gap
  and narrower contribution framing.
- The current title remains broader than the paper's present evidentiary base.
- Related-work coverage is still insufficient for controlled external review in
  educational assessment, deliberative competence, contestability, DAO
  participation behavior, and Web3 regulatory constraints.
- Key author-facing terminology decisions remain unresolved, especially
  `Proof of Knowledge` and `Academy`.

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

- Make the research gap explicit in the introduction in 2-4 sentences.
- Prioritize one near-term evaluation path instead of presenting all five
  research questions as equally immediate.
- Consider narrowing the title before any controlled external review.
- Expand the candidate bibliography first, then verify and integrate only the
  sources that materially strengthen the paper.

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

- Keep or replace the term `Proof of Knowledge`.
- Keep or rephrase the term `Academy`.
- Keep one broad architecture paper or split into narrower papers.
- Choose the next review mode: author review only or controlled external
  review after revision.
- Approve the public correspondence address, affiliation wording, and license
  posture for any later circulation.

## Recommended next human review

Conduct an author-level editorial review against `reviewer-report.md` before
any controlled external circulation. Review should first resolve terminology,
scope, title, abstract, research-gap framing, and related-work sufficiency.
Only after those issues are resolved should invited external academic review be
considered.

## Checklist status

The automated/static portions of the publication checklist were executed.
Human judgment items remain unchecked in
`../../governance/publication-review-checklist.md`.
Checklist applied: yes, for the automated/static checks completed in Phase 1.

## Readiness status

Phase 1.1 readiness category: **Ready for author review only.**

Ready for controlled external review: no  
Ready for public publication: no

**Current status: author review ready; blocked for controlled external review
and publication.**
