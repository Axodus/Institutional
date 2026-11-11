# Human–AI v0.7 Manuscript Integrity & Provenance Record

**Manuscript Version:** Draft v0.7  
**Canonical Classification:** `CANONICAL INTERNAL CONCEPTUAL MANUSCRIPT`  
**Consolidation Authority:** `AXODUS-CEO-DEC-RESEARCH-R1-V07-CONSOLIDATION-01`  
**Parent Proposal:** `AXODUS-RESEARCH-R1-V07-CONSOLIDATION-01`  
**Date Created:** 2026-11-10  
**Commit Authorization:** `COMMIT NOT AUTHORIZED (PENDING CRO DOCUMENTARY ACCEPTANCE & SEPARATE PRESIDENTIAL COMMIT DECISION)`  
**Publication Status:** `NOT AUTHORIZED`  

---

## 1. Authoritative Source Handoff Identifiers

The canonical text in `paper.md` was assembled strictly from two CRO-accepted scientific texts without autonomous substantive alteration:

| Section Range | Source Handoff Identifier | CRO Scientific Status |
|---|---|---|
| Abstract, Metadata, Sections 1–6 | `AXODUS-RESEARCH-R1-V07-STAGE1-FIX-01` | `CRO SCIENTIFICALLY ACCEPTED` |
| Sections 7–10 | `AXODUS-RESEARCH-R1-V07-STAGE2-FIX-01` | `CRO SCIENTIFICALLY ACCEPTED` |

Supporting institutional doctrine and gate records:
- `AXODUS-RESEARCH-FOUNDATIONAL-THESIS-BRIEF-01` (Approved Foundational Thesis)
- `AXODUS-RESEARCH-R1-FOUNDATIONAL-THESIS-CRO-REVIEW-01` (CRO Scientific Qualification)
- `AXODUS-CEO-DEC-RESEARCH-R1-FOUNDATIONAL-THESIS-01` (Presidential Acceptance)
- `AXODUS-CEO-DEC-RESEARCH-R1-GATE-01` (Approval of Conceptual Framing with Conditions `COND-01`–`COND-10`)
- `AXODUS-CEO-DEC-RESEARCH-R1-GATE-02` (Acceptance of `C2_INTEGRATIVE_CONTRIBUTION`)
- `AXODUS-RESEARCH-REQ-R1-FOUNDATIONS-01` (R1 Foundations Literature Evidence)

---

## 2. Calculated Artifact Integrity Hashes

The SHA-256 checksums below describe the final bytes after the authorized targeted documentary correction. The checksum of this record is supplied in the handoff, outside the record itself.

| File Name | Bytes | SHA-256 Checksum |
|---|---|---|
| `paper.md` | 67070 | `9b7daf8e6b3aeb4a4950071b14b33ff39958e2fc67263ecad29c9fe519be53aa` |
| `references.bib` | 6830 | `8bbee88e67e4e96364d5edb18757c7d2f55d732252a644f3dbfde0ead1fd39e7` |

---

## 3. Editorial Transformations Applied (`OP-01` & `OP-02`)

1. **Assembly (`OP-01`):** Combined Sections 1–6 from Stage 1 Fix with Sections 7–10 from Stage 2 Fix in exact sequential order.
2. **Metadata Normalization:** Front matter normalized with title, author, affiliation, correspondence, date (`2026-11-10`), version (`Draft v0.7`), and document type (`Normative-conceptual research framework`).
3. **Heading Hierarchy:** Standardized H1 for main numbered sections (`# Abstract`, `# 1. Introduction` ... `# 10. Conclusion`) and H2/H3 for subsections.
4. **Notation Unification and Correction:** After serialization defects were found, restored the Institutional Decision Episode notation across Section 6 and Section 9:
   $$\mathcal{E}=\langle P,R,M,C,T,A,E,Q,D\rangle, \qquad MC(A,M,R)$$
5. **No Substantive Rewriting:** Zero alterations to accepted normative premises, research questions, C2 definitions, HDE-01 scenario variants, or scientific limitations.

---

## 4. Bibliographic Reconciliation Summary (`OP-03`)

The 14 entries cover 13 author–date cited works and Kang, mentioned nominally as a limited-access comparator. Classifications reflect previous R1 records; no new independent verification was performed:

| Citation Key | Author & Year | Evidence Status in R1 | Notes |
|---|---|---|---|
| `baxter2011sociotechnical` | Baxter & Sommerville (2011) | `VERIFIED_WITHIN_R1_RECORD` | Socio-technical systems foundation |
| `leveson2012engineering` | Leveson (2012) | `METADATA_RECONCILIATION_REQUIRED` | Systems safety; edition/ISBN/URL note preserved |
| `ostrom2010beyond` | Ostrom (2010) | `VERIFIED_WITHIN_R1_RECORD` | Polycentric governance foundation |
| `stone2026legitimate` | Stone & Mittelstadt (2026) | `TEXT_PREVIOUSLY_EXAMINED` | R1 reports text examination; exact venue, date and pagination need reconciliation |
| `sebastian2026decision` | Sebastian et al. (2026) | `TEXT_PREVIOUSLY_EXAMINED` | MIT CISR research briefing; decision rights |
| `engin2026human` | Engin (2026) | `TEXT_PREVIOUSLY_EXAMINED` | R1 reports text examination; extent of full-text inspection not independently established |
| `santonidesio2018meaningful` | Santoni de Sio & van den Hoven (2018) | `TEXT_PREVIOUSLY_EXAMINED` | Meaningful human control; reasons & responsibility |
| `green2022flaws` | Green (2022) | `TEXT_PREVIOUSLY_EXAMINED` | Human oversight critique; nominal review risks |
| `kroll2017accountable` | Kroll et al. (2017) | `VERIFIED_WITHIN_R1_RECORD` | Algorithmic accountability foundation |
| `cobbe2021reviewable` | Cobbe, Lee & Singh (2021) | `TEXT_PREVIOUSLY_EXAMINED` | FAccT '21 reviewable automated decision-making |
| `alfrink2023contestable` | Alfrink et al. (2023) | `VERIFIED_WITHIN_R1_RECORD` | Contestable AI by design |
| `w3c2013provdm` | W3C (2013) | `VERIFIED_WITHIN_R1_RECORD` | Provenance data model standard |
| `amershi2019guidelines` | Amershi et al. (2019) | `VERIFIED_WITHIN_R1_RECORD` | Human-AI interaction guidelines |
| `kang2026institutional` | Kang (2026) | `ABSTRACT_ONLY` | SSRN record/abstract only; DOI and venue require reconciliation |

---

## Metadata and correction provenance

The accepted session Stage 1 supplied the manuscript title. Author, affiliation and correspondence were carried forward from the historical v0.6 front matter; their approval specifically for v0.7 is not independently established and requires responsible author confirmation. The date records local consolidation, not publication. The previous consolidation handoff incorrectly reported this integrity record as 5,110 bytes; read-only verification measured 7,053 bytes before correction. Its final size and SHA-256 are reported in the subsequent handoff, without a self-referential checksum.

The targeted correction restored the accepted mathematical delimiters and commands in Sections 6.1 and 9.5 without modifying scientific prose. The editorial transformation claim in Section 3 concerns the accepted scientific content; the pre-correction serialized equations contained defects and were not byte-identical.

## 5. Historical v0.6 Preservation Verification

The historical scientific baseline remains completely untouched and verified:
- Repository root: `papers/axodus-architecture-paper/`
- Historical commit: `c9652a7f97018c7c740d255f0baa7b5736187826`
- Verified `paper.md` SHA-256: `59b03b553eaf7e390b3af57f2691e0967119a813ff1e7ead4ad883edcbd79afb`
- Verified `paper.tex` SHA-256: `a33745f345a39b042b0eec65e0dab69c8024bccaf2da8d70da62bb6682d4ae44`
- Verified `references.bib` SHA-256: `1f1b99a79bb3aff74f66c92ff103502fb04263383ca3559790ff09a330eda279`

Zero historical files were modified, moved, renamed, archived, or deleted.

---

## 6. Open Normative and Domain Dependencies (`NC-01` to `NC-10`)

All ten institutional nonconformities remain open and governed by competent authorities:
- `NC-01` (Legitimate Principal): Open — CEO / Governance
- `NC-02` (Nondelegable Powers): Open — CEO / Governance
- `NC-03` (Human Finality Doctrine): Open — CEO / Governance
- `NC-04` (Smart Accounts & Political Standing): Open — Governance / CTO
- `NC-05` (Delegation & Receipt Semantics): Open — CTO / ACS / Governance
- `NC-06` (Meaningful Human Intervention): Open — CRO / Governance / Domain Owners
- `NC-07` (Collective Institutional Accountability): Open — CEO / Governance / CRO
- `NC-08` (Legal Personhood, Agency & Liability): Open — Legal Authority / CRO
- `NC-09` (Effective Contestability & Remedy): Open — CRO / Governance
- `NC-10` (Cross-Institutional Portability): Open — CEO / CRO

---

## 7. Scientific and Epistemic Limitations

The manuscript is a **conceptual and normative framework**. It explicitly records:
1. No claim of empirical validation, superior decision quality, or operational efficiency.
2. The Institutional Decision Episode scenario (`HDE-01`) is a fictional, nonempirical thought experiment.
3. Contribution classification is strictly `C2_INTEGRATIVE_CONTRIBUTION` (`DISTINCTIVE_ORIGINALITY_NOT_ESTABLISHED`).
4. Cross-institutional portability is a research proposition to be evaluated, not an established fact.
5. Technical capability and permission do not constitute institutional authority.
