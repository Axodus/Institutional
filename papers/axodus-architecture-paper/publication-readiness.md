# Publication Readiness — Axodus Architecture Paper

Review date: 2026-07-03  
Version reviewed: draft v0.1  
Decision: **Ready for structured human review; not ready for publication,
submission, outreach, grant use, or external distribution.**

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

## Bibliographic status

Eight cited sources have verification records. Metadata was checked against
publisher, journal, institutional, standards-body, or canonical preprint
records.

The following research areas remain candidates and are not cited:

- deliberative and informed participation;
- automation bias and calibrated reliance;
- contestable automated decisions;
- empirical DAO voting and delegation;
- educational assessment validity and equity;
- maturity-model reliability.

All bibliographic metadata must be rechecked before submission. Venue-specific
formatting has not been applied.

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
3. Complete substantive review by independent readers with relevant expertise
   in socio-technical systems, governance, human–AI interaction, education,
   decentralized systems, and risk.
4. Decide whether the broad architecture should remain one paper or be narrowed
   before venue selection.
5. Verify that every Axodus-specific statement conforms to the intended public
   disclosure boundary.
6. Review the CC BY 4.0 licensing notice and third-party rights before release.
7. Compile the LaTeX source and inspect its log and rendered output. No LaTeX
   engine is installed in the current environment, so compilation was not
   performed.
8. Select a venue and apply its authorship, disclosure, formatting, and
   submission requirements in a separate phase.

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

## Recommended next human review

Conduct a claim-by-claim editorial review before expanding the manuscript.
Reviewers should first challenge the problem statement, architecture
boundaries, Proof of Knowledge terminology, and evaluation feasibility. Only
after those issues are resolved should the draft be lengthened, formatted for
a venue, compiled to PDF, or considered for external circulation.

## Checklist status

The automated/static portions of the publication checklist were executed.
Human judgment items remain unchecked in
`../../governance/publication-review-checklist.md`.

**Final Phase 1 status: complete for preparation; blocked for publication.**
