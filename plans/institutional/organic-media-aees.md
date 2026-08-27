# AEES — Organic Media Editorial Production Backlog

Status: Controlled production plan; drafts require human review before external publication

AEES means **EPIC → SPRINT → TASK**. This backlog converts the annotated
editorial program into an ordered production system. The website is the
canonical source; Medium, Substack, GitHub, and optional community channels
receive reviewed adaptations only after the canonical article is approved.

## Complete EPIC request documents

Each EPIC has a separate implementation request with scope, sprint/task
breakdown, dependencies, validation, acceptance criteria, and escalation
rules:

- [EPIC E0 — Editorial control and production setup](epics/EPIC-E0-editorial-control.md)
- [EPIC E1 — Identity and disambiguation](epics/EPIC-E1-identity-disambiguation.md)
- [EPIC E2 — Architecture and ecosystem](epics/EPIC-E2-architecture-ecosystem.md)
- [EPIC E3 — Governance and proposed nuclei](epics/EPIC-E3-governance-nuclei.md)
- [EPIC E4 — Evidence, traceability, and AI assistance](epics/EPIC-E4-evidence-ai.md)
- [EPIC E5 — Lifecycle and platform workflows](epics/EPIC-E5-lifecycle-workflows.md)
- [EPIC E6 — Regulated domains and research agenda](epics/EPIC-E6-regulated-research.md)
- [EPIC E7 — Distribution, review, and measurement](epics/EPIC-E7-distribution-measurement.md)

Image briefs for the twelve canonical articles are maintained in
[organic-media-image-prompts.md](organic-media-image-prompts.md). They are
creative requests only and require the same evidence, disclosure, rights, and
human-review gates as the associated article.

## Production rules

- Primary language: English.
- Cadence target: one article and two threads per week.
- Every task must classify claims as fact, proposal, hypothesis, or future work.
- Claims of implementation, adoption, certification, enforcement, performance,
  security, revenue, partnership, or production readiness remain blocked unless
  separately evidenced and approved.
- Numeric results, guarantees, and operational examples are not publishable as
  facts without a registered source or study.
- Regulated-domain material remains conceptual and requires narrower review.

## Definition of done for every article

An article is complete only when it has:

1. canonical website draft and stable URL;
2. 900–1,600 words or an approved exception;
3. claims classification and claims-register check;
4. identity/taxonomy links;
5. limitations section;
6. title, description, canonical, and social metadata;
7. one reviewed Medium/Substack adaptation, if scheduled;
8. two reviewed threads linked to the canonical article;
9. named human approval before external publication;
10. publication URL and date recorded in the observation log.

## EPIC E0 — Editorial control and production setup

### Sprint E0-S1 — Source-of-truth and workflow

| Task | Action | Done when | Risk | Validation |
|---|---|---|---|---|
| E0-S1-T1 | Create article and thread inventory from this backlog | All 12 topics have IDs, owners, status, and target week | Low | Inventory has no duplicate IDs |
| E0-S1-T2 | Create claim-review worksheet | Every draft has fields for claim type, evidence, limitation, and reviewer | Medium | Worksheet maps to `research/claims-register.md` |
| E0-S1-T3 | Define canonical-to-external adaptation flow | Website-first order is recorded and applied to templates | Low | No external item precedes its canonical draft |
| E0-S1-T4 | Create monthly observation log | Log records URLs, dates, channel, status, and observations | Low | Empty baseline log exists before publication |

### Sprint E0-S2 — Channel readiness

| Task | Action | Done when | Risk | Validation |
|---|---|---|---|---|
| E0-S2-T1 | Align Medium, Substack, and GitHub bios | Each bio uses the canonical identity and prototype-stage boundary | High | Text comparison passes; no blocked claims |
| E0-S2-T2 | Verify official channel ownership and URLs | Owner confirms each channel before `sameAs` or CTA use | High | Verification record names channel and date |
| E0-S2-T3 | Confirm external publication authorization | Human approval exists for each channel and batch | High | No publication occurs without recorded approval |

## EPIC E1 — Identity and disambiguation

### Sprint E1-S1 — Canonical identity package

| Task | Action | Done when | Risk | Validation |
|---|---|---|---|---|
| E1-S1-T1 | Draft `What is Axodus?` for the website | Page explains identity, scope, stage, and boundaries in plain English | High | Matches institutional identity record |
| E1-S1-T2 | Draft “What Axodus is not” boundary block | Describes exclusions without repeating “scam” as an SEO term | High | No defensive keyword stuffing |
| E1-S1-T3 | Produce Medium adaptation | Summary links to canonical page and preserves qualifications | Medium | Link and wording audit passes |
| E1-S1-T4 | Produce Substack adaptation | Newsletter version links to canonical page and states status | Medium | No unsupported benefit or outcome claims |

### Sprint E1-S2 — Brand disambiguation

| Task | Action | Done when | Risk | Validation |
|---|---|---|---|---|
| E1-S2-T1 | Write thread on Axodus identity | Five to eight factual/proposal points with official links | Medium | No comparison or superiority claim |
| E1-S2-T2 | Write thread distinguishing Axodus from Exodus | Uses neutral name disambiguation and avoids repeating negative labels | High | No “scam”/“Ponzi” keyword targeting |
| E1-S2-T3 | Add canonical channel links | Site, docs, GitHub, Medium, Substack, and Notion references are consistent | Medium | URL and ownership check passes |

## EPIC E2 — Architecture and ecosystem

### Sprint E2-S1 — Governed knowledge problem

| Task | Action | Done when | Risk | Validation |
|---|---|---|---|---|
| E2-S1-T1 | Draft “Why governed knowledge matters” | Explains fragmentation as a research/problem statement | Medium | No invented productivity or cost statistics |
| E2-S1-T2 | Add research/documentation links | Article points to approved Institutional sources | Low | All links resolve |
| E2-S1-T3 | Produce two problem-focused threads | Threads distinguish hypothesis from observed fact | Medium | Claims register review passes |

### Sprint E2-S2 — Platform ecosystem taxonomy

| Task | Action | Done when | Risk | Validation |
|---|---|---|---|---|
| E2-S2-T1 | Draft “The Axodus platform ecosystem” | Uses the canonical foundation/platform/nucleus taxonomy | High | Matches `institutional-taxonomy.md` |
| E2-S2-T2 | Remove unapproved infrastructure assertions | Cloud, zero-trust, mesh, immutable ledger, and similar details are either sourced or labeled proposals | High | No implementation inference remains |
| E2-S2-T3 | Produce foundation-vs-nuclei thread | Relationship map is conceptual and bounded | Medium | Taxonomy terminology matches |

## EPIC E3 — Governance and proposed nuclei

### Sprint E3-S1 — Constitutional governance

| Task | Action | Done when | Risk | Validation |
|---|---|---|---|---|
| E3-S1-T1 | Draft “Constitutional governance, explained” | Defines explicit rules, review, escalation, and human authority as a proposal | High | No claims of hard-coded enforcement or runtime guarantee |
| E3-S1-T2 | Replace operational diagrams with conceptual flows | Diagrams use proposed/illustrative labels | High | No deployed process is implied |
| E3-S1-T3 | Produce two governance threads | One covers constraints; one covers review and amendment | High | Governance mechanics and claims register checked |

### Sprint E3-S2 — Proposed platform nucleus

| Task | Action | Done when | Risk | Validation |
|---|---|---|---|---|
| E3-S2-T1 | Draft “What is a proposed platform nucleus?” | Defines a bounded conceptual nucleus | Medium | No “consolidated core” or production claim |
| E3-S2-T2 | Cover ACS, Academy, and Marketplace | Uses controlled functions and status qualifications | High | No certification, monetization, or performance assertion |
| E3-S2-T3 | Produce nucleus lifecycle thread | Research-to-prototype path is explicitly proposed | Medium | No graduation or adoption presented as completed |

### Sprint E3-S3 — Governance standalone context

| Task | Action | Done when | Risk | Validation |
|---|---|---|---|---|
| E3-S3-T1 | Draft Governance platform context | Describes governance.country as a proposed Harmony-specific standalone context | Critical | No claim of Harmony acceptance, adoption, enforcement, or partnership |
| E3-S3-T2 | Separate proposal from adoption | Adoption is described only as a future state | Critical | No production/runtime table stated as current |
| E3-S3-T3 | Produce two Harmony-scope threads | Threads explain conceptual review and unresolved questions | High | Legal/disclosure review completed |

## EPIC E4 — Evidence, traceability, and AI assistance

### Sprint E4-S1 — Evidence and traceability

| Task | Action | Done when | Risk | Validation |
|---|---|---|---|---|
| E4-S1-T1 | Draft “Evidence and traceability by design” | Uses provenance as a conceptual reconstruction requirement | Critical | No immutability, integrity, security, or accountability guarantee |
| E4-S1-T2 | Remove unsupported cryptographic implementation details | ZKPs, Merkle trees, signatures, and ledgers are future-work examples only unless sourced | Critical | Claims register and security review pass |
| E4-S1-T3 | Produce two limitation-focused threads | Privacy, storage, and observability tensions are hypotheses/open questions | High | No numeric benchmark or result appears |

### Sprint E4-S2 — AI assistance under human oversight

| Task | Action | Done when | Risk | Validation |
|---|---|---|---|---|
| E4-S2-T1 | Draft bounded AI assistance article | AI support is limited to proposed analytical/documentation tasks | High | No autonomous authority or safety guarantee |
| E4-S2-T2 | Remove unsupported runtime controls | Confidence scores, kill switches, automatic rollback, and live anomaly response are proposals or future work | Critical | No operating-system claim remains |
| E4-S2-T3 | Produce human-authority threads | Threads explain human approval and responsibility boundaries | High | Terminology matches identity and governance records |

## EPIC E5 — Lifecycle and platform workflows

### Sprint E5-S1 — Research to reference platform

| Task | Action | Done when | Risk | Validation |
|---|---|---|---|---|
| E5-S1-T1 | Draft lifecycle article | Research → Architecture → Documentation → Prototype is a planning model | Medium | External review/deployment are clearly future states |
| E5-S1-T2 | Describe reference-platform concept | No certification, independent deployment, or third-party adoption is asserted | High | Evidence boundary review passes |
| E5-S1-T3 | Produce two lifecycle threads | Threads are illustrative and non-empirical | Medium | No actual case is implied |

### Sprint E5-S2 — Academy, BBA, and workflows

| Task | Action | Done when | Risk | Validation |
|---|---|---|---|---|
| E5-S2-T1 | Draft platform-workflows article | Academy, BBA, and institutional workflows are bounded concepts | High | No active certification, compliance, or production claim |
| E5-S2-T2 | Replace “BBA” ambiguity | Define BBA only according to an approved institutional description | High | No invented expansion or implementation detail |
| E5-S2-T3 | Produce relationship threads | Qualification → construction → review is presented as proposal | Medium | No operational workflow is reported |

## EPIC E6 — Regulated domains and research agenda

### Sprint E6-S1 — DeFi, Mining, and Lotto

| Task | Action | Done when | Risk | Validation |
|---|---|---|---|---|
| E6-S1-T1 | Draft bounded-domain article | DeFi, Mining, and Lotto are conceptual domains only | Critical | No financial, yield, token, VRF, TPS, or execution claim |
| E6-S1-T2 | Remove false absolutes and guarantees | “Absolute”, “tamper-proof”, “cryptographically secure”, and similar claims are removed or sourced | Critical | Legal/security review passes |
| E6-S1-T3 | Produce two boundary threads | Threads explain scope and review requirements | High | No operational scenario presented as actual |

### Sprint E6-S2 — Research agenda and open questions

| Task | Action | Done when | Risk | Validation |
|---|---|---|---|---|
| E6-S2-T1 | Draft research-agenda article | Summarizes open questions and limitations | Medium | No observed result is claimed |
| E6-S2-T2 | Convert numeric assertions into hypotheses | Remove unvalidated “80%” and “sub-50ms” targets or register them as future test hypotheses | Critical | Claims register updated before publication |
| E6-S2-T3 | Produce synthesis threads | Threads point back to all approved articles and open questions | Medium | Link and terminology audit passes |

## EPIC E7 — Distribution, review, and measurement

### Sprint E7-S1 — Adaptation and release

| Task | Action | Done when | Risk | Validation |
|---|---|---|---|---|
| E7-S1-T1 | Adapt approved articles to Medium | Summary/excerpt links to canonical site article | Medium | No uncontrolled duplicate or divergent claim |
| E7-S1-T2 | Adapt approved articles to Substack | Newsletter version links to canonical site article | Medium | Send-to-email/app decision recorded |
| E7-S1-T3 | Publish GitHub discussion/changelog references | Only reviewed summaries and source links are used | Medium | No private or implementation-sensitive disclosure |

### Sprint E7-S2 — Monthly observation and correction

| Task | Action | Done when | Risk | Validation |
|---|---|---|---|---|
| E7-S2-T1 | Capture channel metrics | Views, referrals, subscriptions, and publication counts are recorded where authorized | Low | Source and date recorded for each metric |
| E7-S2-T2 | Capture search observations | Queries, snippets, correction prompts, and dates are recorded without causal claims | Medium | Observation log distinguishes fact from interpretation |
| E7-S2-T3 | Run quarterly content audit | Old posts, bios, links, and claims are rechecked | High | No superseded identity remains in current channels |

## Release order

The required order is:

```text
E0 control setup
  → E1 identity
  → E2 architecture
  → E3 governance and nuclei
  → E4 evidence and AI
  → E5 lifecycle and workflows
  → E6 regulated domains and research agenda
  → E7 distribution and measurement
```

Tasks within the same sprint may run in parallel only after their source
article and claims review are complete.

## Blockers and required decisions

- Website/CMS access is required before canonical article implementation.
- A named human reviewer is required before every external batch.
- Medium, Substack, GitHub Discussions, and any community account must be
  verified before use.
- Any claim of implementation, performance, adoption, certification,
  partnership, legal status, or financial activity requires new evidence and a
  claims-register decision.
- The original annotated drafts are source material for rewriting, not approved
  publication copy.
