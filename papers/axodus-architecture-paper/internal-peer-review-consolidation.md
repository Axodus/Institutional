# Internal Peer Review Consolidation

Phase: 1.14  
Manuscript: draft v0.3.1  
Consolidation date: 2026-07-03  
Status: internal review inputs consolidated; targeted revision required

## Executive summary

The three supplied review inputs support a targeted v0.3.2 academic-hardening
patch rather than a broad v0.4 revision. The strongest consensus is that the
paper's central axis is appropriate but remains under-specified at the
architecture and method levels.

The next patch should explain the direction of authority, evidence,
AI-assistance provenance, rationale, decision, and review flows; add bounded
synthetic illustrations; strengthen contestability and scope-reduction
principles; and define proposed evaluation measures and a staged validation
path. Provenance and accountability claims require bibliography hardening
before citations are added.

No review input authorizes controlled external review, publication, or an
empirical claim.

## Severity summary

| Severity | Count | Interpretation |
|---|---:|---|
| Critical | 0 | No confirmed evidence-boundary breach or sensitive disclosure was reported. |
| Major | 10 | Central architecture, literature, contestability, provenance, or testability issue. |
| Moderate | 6 | Material scope, terminology, readiness, or supporting-method issue. |
| Minor | 3 | Package-governance or baseline assessment issue. |

## Decision summary

| Decision | Count |
|---|---:|
| Accepted | 15 |
| Partially accepted | 3 |
| Deferred | 1 |
| Rejected | 0 |

## Consolidated findings

| ID | Condensed finding | Severity | Decision | Destination |
|---|---|---|---|---|
| R1-01 | DeFi example is too prominent. | Major | Accepted | v0.3.2 targeted patch |
| R1-02 | Architecture lacks dependency, control, and information flow. | Major | Accepted | v0.3.2 targeted patch |
| R1-03 | Provenance and accountability literature is insufficient. | Major | Accepted | bibliography hardening |
| R1-04 | Abstract prominence and Section 5 treatment of L/D are imbalanced. | Moderate | Partially accepted | v0.3.2 targeted patch |
| R1-05 | Defensive language remains in architecture sections. | Moderate | Accepted | v0.3.2 targeted patch |
| R2-01 | Package is suitable for internal review. | Minor | Accepted | v0.3.2 targeted patch |
| R2-02 | Package manifest should include itself. | Minor | Accepted | v0.3.2 targeted patch |
| R2-03 | Related-work notes retain outdated PoK wording. | Minor | Accepted | v0.3.2 targeted patch |
| R2-04 | Unresolved blockers need an external-use qualifier. | Moderate | Accepted | v0.3.2 targeted patch |
| R2-05 | Full maturity taxonomy needs a later gate before public-facing use. | Major | Accepted | future v0.4 |
| R3-01 | Controlled illustrative examples are needed. | Major | Accepted | v0.3.2 targeted patch |
| R3-02 | The paper's synthesis needs a more precise statement. | Major | Accepted | v0.3.2 targeted patch |
| R3-03 | Participation-readiness evaluation and mitigation need definition. | Moderate | Partially accepted | v0.3.2 targeted patch |
| R3-04 | Longer-term institutional validation path is needed. | Moderate | Accepted | future empirical validation phase |
| R3-05 | Contestability needs independence, scalability, and capture controls. | Major | Accepted | v0.3.2 targeted patch |
| R3-06 | Complexity requires simplification heuristics. | Major | Accepted | v0.3.2 targeted patch |
| R3-07 | AI provenance needs bounded technical options. | Major | Accepted | v0.3.2 targeted patch |
| R3-08 | Regulatory and compliance adaptation is underdeveloped. | Moderate | Deferred | future v0.4 |
| R3-09 | Proposed measures are needed for empirical testability. | Major | Partially accepted | future empirical validation phase |

## Reviewer conflicts and resolution

### Maturity detail versus scope discipline

R1-04 asks for stronger treatment because maturity appears in the abstract,
while R2-05 warns against public-facing use of the complete internal taxonomy.
The resolution is not to import the full rubric. The targeted patch should
reduce abstract prominence or make the short conceptual purpose clearer.

### Reduce DeFi versus expand regulatory treatment

R1-01 calls for reducing the DeFi example, while R3-08 asks for deeper
regulatory and compliance adaptation. Expanding Web3 regulation in v0.3.2
would broaden the paper and preserve the same domain drift. The DeFi example
should be removed or subordinated now; broader regulatory treatment is
deferred.

### More substance versus less complexity

R1-02 and R3-01 request flows and illustrations, while R3-06 warns that the
architecture is overly complex. The resolution is to explain a minimum
traceability path and one or two synthetic scenarios, not add layers,
institutions, or feature families.

### Longer-term validation versus current evidence limits

R3-04 and R3-09 request validation paths and measures. These requests are
compatible with the paper only as future-work design. They cannot be written
as completed studies, operational benchmarks, or institutional pilots.

## Evidence-boundary risks

The following suggestions would violate Phase 1 boundaries if applied
literally:

- presenting illustrative scenarios as actual cases, deployments, users,
  partners, pilots, or institutional evidence;
- describing evidence registries, provenance logs, hashes, signatures,
  cryptographic proofs, or control flows as implemented;
- claiming that provenance options provide security, integrity, auditability,
  or accountability guarantees;
- describing proposed measures as observed operational metrics or benchmarks;
- presenting future institutional validation as already arranged or underway;
- describing participation-readiness safeguards as proven to prevent
  exclusion, curriculum capture, or unfairness;
- presenting the L/D taxonomy as a validated scientific instrument or using it
  to publish component maturity assignments;
- describing the synthesis as novel, unique, first, superior, or empirically
  validated;
- presenting regulatory discussion as legal compliance or legal advice.

## Required bibliography hardening

Before provenance or accountability citations enter the manuscript, candidate
sources should be identified and verified for:

- data provenance and provenance records;
- W3C PROV or equivalent provenance models;
- algorithmic accountability;
- contestability, appeals, and institutional review;
- calibrated reliance and override behavior;
- governance measures and review-process quality;
- complex-system coupling and system accidents; and
- socio-technical failure propagation.

No candidate source is citable until its metadata and propositional fit are
verified under `governance/citation-policy.md`.

## Recommendation

Authorize v0.3.2 edits in the next phase for a targeted internal
academic-hardening patch only. Do not authorize v0.4, controlled external
review, publication, submission, outreach, grant use, fundraising use,
external distribution, or authority signaling.

Current readiness category: **Ready for v0.3.2 targeted internal revision
only.**
