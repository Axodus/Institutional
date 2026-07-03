# Internal Peer Review Instructions

Document status: confidential internal review instructions  
Manuscript: Axodus architecture paper, draft v0.3.1  
Distribution: named internal reviewers only

## Confidentiality and non-distribution

By accepting the package, the reviewer agrees to:

- use it only for the assigned internal peer review;
- not forward, publish, quote publicly, post, submit, or redistribute any
  package file or review content;
- not upload the package to public or unapproved AI services, repositories,
  issue trackers, shared drives, or collaboration systems;
- protect author contact metadata and reviewer identities;
- avoid copying private implementation or project context into the review;
- report any accidental disclosure promptly to the package owner; and
- return or securely delete the package when instructed.

The package does not authorize contact with journals, conferences, arXiv,
institutions, funders, partners, media, communities, or other external parties.

## Review scope

Review the manuscript as a prototype-stage conceptual architecture and focused
research agenda. Evaluate the logic, clarity, evidence discipline, and proposed
evaluation method. Do not evaluate it as a deployed product, operating
institution, security-audited system, or validated maturity model.

The central review question is:

> Does the manuscript offer a sufficiently clear and substantive conceptual
> architecture for traceability and accountability in human–AI-assisted
> digital institutions while staying within its evidence boundaries?

Use `internal-peer-review-package.md` for the complete question set and file
manifest. Record the review in `internal-peer-review-form.md`.

## Required review method

1. Confirm the manuscript version and SHA-256 hash against the package
   manifest.
2. Read `governance/evidence-boundaries.md` before assessing Axodus-specific
   claims.
3. Read the manuscript once for its overall argument without editing.
4. Review Sections 3–8 for contribution unity and architectural substance.
5. Review Sections 9–12 for prototype status, evaluation feasibility,
   limitations, and future-work discipline.
6. Check cited propositions against `references.bib` and
   `research/bibliography-verified.md` where relevant.
7. Complete every applicable section of the review form.
8. Return the form through the approved private channel.

Do not edit the manuscript source directly unless the package owner separately
requests tracked editorial changes. Suggested wording belongs in the review
form and must identify the target section.

## Finding format

Each finding should state:

- severity: critical, major, minor, or editorial;
- manuscript section or exact phrase;
- the problem;
- why it matters;
- the smallest recommended correction; and
- whether the issue blocks the next internal readiness assessment.

Use **critical** for evidence-boundary violations, sensitive disclosure,
fabricated or materially misused sources, or wording that falsely implies
implementation, production, authority, security, users, adoption, or results.

Use **major** for contribution ambiguity, architectural gaps, invalid method,
unsupported central claims, or terminology that materially changes the
paper's interpretation.

Use **minor** for bounded clarity, organization, citation, or terminology
problems that do not undermine the central argument.

Use **editorial** for copyediting and formatting issues.

## Evidence and citation rules

- Treat the functional component classes as conceptual types, not implemented
  modules.
- Treat L-Level and D-Level as internal operational taxonomy, not validated
  measurement scales.
- Do not infer any actual component score, production state, or sensitive
  authority.
- Treat candidate bibliography entries as unverified leads, not citations.
- Flag unsupported scholarly assertions; do not invent or insert a reference.
- Distinguish a missing source from a defective argument.
- Treat proposed experiments and measures as future work, not completed
  research.

If a finding would require sensitive implementation detail to explain, mark it
`SENSITIVE — discuss privately` and omit the detail from the review form.

## Review outcome

Select one outcome in the form:

1. return for major internal revision;
2. continue internal review after required minor revisions;
3. internally acceptable for the next readiness assessment; or
4. unable to assess.

These outcomes do not authorize controlled external review or publication.
Only a later, explicit human readiness gate may consider either action.

## Reviewer conduct

Disclose relevant conflicts, prior Axodus involvement, and limits of
expertise. Focus criticism on the manuscript and its evidence. Do not use
confidential project knowledge to strengthen a claim that the repository does
not support.

The reviewer may request a narrowly scoped additional file from the package
owner. The reviewer should not browse the repository or solicit external
context independently.
