# Internal Peer Review 01

Review input: supplied for Phase 1.14 consolidation  
Manuscript reviewed: draft v0.3.1  
Classification: confidential internal review record  
External-use authority: none

## Overall assessment

The review identifies a material architecture-substance gap. The manuscript's
focus is clearer than earlier versions, but the component taxonomy still needs
an explicit theoretical account of dependency direction, control flow, and
information flow. Provenance concepts require stronger literature support, and
the remaining DeFi example should not carry general architectural weight.

## Findings

| ID | Finding | Severity | Decision | Destination |
|---|---|---|---|---|
| R1-01 | Schär/DeFi remains too prominent as the practical example for dependency propagation. | Major | Accepted | v0.3.2 targeted patch |
| R1-02 | Section 4 lists layers without sufficiently explaining dependency direction, control flow, or information flow. | Major | Accepted | v0.3.2 targeted patch |
| R1-03 | Evidence registry and AI-assistance provenance need grounding in data-provenance and algorithmic-accountability literature. | Major | Accepted | bibliography hardening |
| R1-04 | The abstract gives L-Level and D-Level more prominence than the brief Section 5 treatment supports. | Moderate | Partially accepted | v0.3.2 targeted patch |
| R1-05 | Repeated defensive disclaimer language remains within architecture sections. | Moderate | Accepted | v0.3.2 targeted patch |

## Decision rationale

R1-01 is accepted because a domain-specific financial example should not
function as general evidence for dependency behavior. The targeted patch
should remove or subordinate the example rather than replace it with another
unsupported generalization.

R1-02 is accepted as a central revision requirement. The next patch should
describe a conceptual sequence among authority, evidence, AI-assistance
provenance, rationale, decision, and review without implying software topology
or implemented orchestration.

R1-03 is accepted, but no citation may enter the manuscript until metadata and
propositional fit are verified. W3C PROV or equivalent provenance models and
algorithmic-accountability scholarship remain candidates.

R1-04 is partially accepted. The paper should not reproduce the full internal
maturity rubric. The targeted resolution is to reduce abstract prominence or
strengthen the concise conceptual link in Section 5 while preserving the
taxonomy's supporting role.

R1-05 is accepted. The patch should retain boundaries in metadata, abstract,
introduction, Prototype Status, and Limitations while replacing repeated
architecture-section disclaimers with positive interface definitions.

## Evidence-boundary note

Applying R1-02 or R1-03 literally as a description of existing pipelines,
logs, registries, hashes, or controls would imply implementation. Any flow or
provenance mechanism must remain a conceptual design requirement. The review
does not establish system behavior or validation.

## Review outcome

Proceed to a targeted internal v0.3.2 hardening patch after candidate-source
verification priorities are recorded. Do not open a broad v0.4 revision.
