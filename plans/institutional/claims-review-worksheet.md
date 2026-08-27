# Claims-review worksheet

Status: E0 baseline — review records are empty until a human reviewer is named

This worksheet operationalizes `research/claims-register.md` and the
publication checklist. One row is required for each material statement in an
article or adaptation. Copy the article's rows into its review record; do not
make an unregistered claim decision in prose.

## Required row fields

| Field | Required value or guidance |
|---|---|
| Article/thread ID | `ART-##` or `THR-##A/B` from the inventory |
| Claim text | Exact sentence or a short exact excerpt |
| Type | `Externally supported fact`, `Internal claim`, `Design proposal`, `Hypothesis`, or `Future work` |
| Claims-register ID | Existing `AX-###`, or `NEW—register before approval` |
| Evidence | Verified source/path, or literal `[REFERENCE NEEDED]` |
| Limitation | What the statement does not establish; include status boundary |
| Reviewer | Named human reviewer; blank means pending |
| Decision | `Allow`, `Revise`, `Block`, or `Pending` |
| Decision date | ISO date, blank until decided |
| Notes | Corrections, wording alternatives, or escalation |

## Article sampling baseline

These seed rows ensure all twelve planned articles have an explicit first
review checkpoint. They are not approvals and contain no invented evidence.

| Article ID | Topic | Expected claim-risk flags | Initial claims-register anchors | Evidence / decision |
|---|---|---|---|---|
| ART-01 | What is Axodus? | identity; stage; disambiguation; no superiority | AX-001, AX-006, AX-035, AX-038 | Pending — use canonical identity; review blocked claims |
| ART-02 | Why governed knowledge matters | unsupported productivity/cost metrics; literature fit | AX-017; related-work sources | Pending; use `[REFERENCE NEEDED]` for unsupported metrics |
| ART-03 | The Axodus platform ecosystem | implementation; module count; maturity inference | AX-002, AX-018, AX-024–AX-030 | Pending — conceptual taxonomy only |
| ART-04 | Constitutional governance, explained | enforcement; authority; security guarantee | AX-011, AX-012, AX-015, AX-019 | Pending — label as proposal |
| ART-05 | Proposed platform nucleus | ACS/Academy/Marketplace implementation; certification | AX-010, AX-018, AX-024–AX-030 | Pending — bounded conceptual functions |
| ART-06 | Governance as a standalone platform context | Harmony adoption/partnership; deployment | AX-016 and governance boundaries | Pending — no adoption inference |
| ART-07 | Evidence and traceability by design | immutability; cryptography; audit/security guarantee | AX-011, AX-013, AX-017 | Pending — provenance proposal only |
| ART-08 | AI assistance under human oversight | autonomy; performance; safety; live controls | AX-014 and evidence boundaries | Pending — bounded assistance proposal |
| ART-09 | Research to reference platform | completed lifecycle; deployment; certification | AX-018, AX-020 | Pending — planning model/future work |
| ART-10 | Academy, BBA, and institutional workflows | active workflow; compliance; implementation | AX-010, AX-018 | Pending — conceptual relationships |
| ART-11 | DeFi, Mining, and Lotto as bounded domains | financial outcomes; token; yield; security; regulated activity | Evidence boundaries; relevant register entries | Pending — legal/disclosure review required |
| ART-12 | Research agenda and open questions | numeric targets; measured results; adoption | AX-007, AX-017 and new claims if needed | Pending — hypotheses/future work only |

## Review decision rules

- A blocked claim remains in the claims register and is removed from public
  copy; it is never silently downgraded to a proposal.
- Unsupported scholarly assertions use `[REFERENCE NEEDED]` until a verified
  bibliographic record is available.
- Any metric, implementation, adoption, security, performance, financial,
  regulatory, or production wording is a mandatory flag for review.
- `Allow` means wording is permitted for the reviewed version; it is not
  canonical or external publication approval.

## Blank review record

| Article/thread ID | Claim text | Type | Claims-register ID | Evidence | Limitation | Reviewer | Decision | Decision date | Notes |
|---|---|---|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  | Pending |  |  |
