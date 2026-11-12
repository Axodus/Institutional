# Human–AI v0.7.1 — Internal Pre-Review Record

**Mandate:** AXODUS-RESEARCH-R1-V07-PRE-REVIEW-CORRECTIONS-01  
**Prepared:** 2026-11-11 (workspace date)  
**Status:** PRE_REVIEW_CORRECTIONS_COMPLETE / CRO_VALIDATION_PENDING  
**Handling:** Internal working candidate. External circulation, review, submission and publication are not authorized.  
**Protected source:** 1ef3d9237a880cf494d61ec3d53dbebb178c9b1d, branch main, papers/human-ai-institutional-governance/v0.7/.

## Applied changes and source fidelity

| Workstream | Classification | Applied change |
|---|---|---|
| AR-FIX-01 | BIBLIOGRAPHIC | Reconciled Stone, Leveson, Engin and Kang and corrected the conflated MIT CISR record; preserved all 14 citation keys. Exact field changes and primary records follow. |
| AR-FIX-02 | CITATION | §2.2: Sebastian et al.; §2.3 and §8.7: Cobbe et al.; §2.4: Kang author–date citation; §4.5: expanded World Wide Web Consortium with W3C abbreviation, retained at §8.5. |
| AR-FIX-02 | EDITORIAL | Appended one alphabetized References section generated from the same 14 BibTeX entries; separated internal evidence notes from the scholarly bibliography. |
| AR-FIX-03 | METADATA | Identified v0.7.1 as a non-public pre-review working copy; labeled authorship metadata as pending and distinguished preparation dates. |
| AR-FIX-04 | Read-only | Compared the historical scientific files across commits and recorded the pre-existing LaTeX edit. |
| AR-FIX-05 | EDITORIAL | No whitespace cleanup within the body. |
| Scientific change control | SCIENTIFIC_CHANGE_PROPOSED | None implemented or proposed on the evidence examined. |

Reversing the five listed citation substitutions recovers the protected abstract and all ten sections byte for byte. Front matter and the appended References are the only other manuscript differences. Section hierarchy, intentional line breaks, equations, normative premises, hypotheses, and scientific limitations are preserved.

## Bibliographic verification

| Source | Primary evidence and disposition |
|---|---|
| Stone & Mittelstadt | The [ACM version of record](https://ora.ox.ac.uk/objects/uuid%3A58631baa-7cf6-418f-a2f1-72533cb2eedb/files/rq811kn12b) gives Jake Iain Stone, the full subtitle, *ACM Journal on Responsible Computing*, 3(1), Article 2, 19 pages, January 2026, DOI 10.1145/3725858. Replaced the incorrect given name and generic venue and recorded the article locator and length. The [Oxford catalogue](https://ora.ox.ac.uk/objects/uuid%3A58631baa-7cf6-418f-a2f1-72533cb2eedb) gives March 29, 2025; the citation follows the journal issue date printed in the version of record. Abstract and introduction support the bounded legitimacy distinction in §2.2, without establishing legal consequences. |
| Leveson | [MIT Press](https://mitpress.mit.edu/9780262016629/engineering-a-safer-world/) distinguishes the January 2012 hardcover, ISBN 9780262016629, from the December 2016 paperback, ISBN 9780262533690. Retained the 2012 hardcover and matched its URL to the ISBN. The publisher description supports the systems orientation in §2.1; it does not validate the proposed framework. |
| Engin | [Elsevier's journal record](https://www.sciencedirect.com/science/article/pii/S266665962600020X) and [UCL Discovery](https://discovery.ucl.ac.uk/id/eprint/10228987/) confirm the full title with HAIG, June 2026, volume 26, Article 100167, DOI 10.1016/j.jrt.2026.100167. The abstract explicitly identifies decision authority, process autonomy and accountability configuration. This is a targeted metadata and abstract check; full-text consultation is not asserted. |
| Kang | The indexed [SSRN record and abstract](https://papers.ssrn.com/sol3/Delivery.cfm/7339378.pdf?abstractid=7339378&mirid=1&type=2) identify the full title, Timothy Kang, manuscript date August 23, 2026, and DOI 10.2139/ssrn.7339378. Reclassified as SSRN preprint, without a journal-venue claim. Direct landing page and PDF retrieval returned HTTP 403; the accessible indexed material was the abstract and metadata. ABSTRACT_ONLY remains in force. No inference about absent distinctions or priority. |
| Sebastian et al. | The [MIT CISR four-author briefing](https://dspace.mit.edu/handle/1721.1/175016) confirms *Designing Decision Rights for AI*, Thomas Haskamp, XXVI(6), 2026. The [inherited URL](https://dspace.mit.edu/handle/1721.1/175164) identifies a different two-author item. The four-author identity and volume/issue in the baseline point to the briefing; its abstract supports the bounded §2.2 claim. |
| Cobbe et al.; Alfrink et al. | [Cambridge-hosted conference paper](https://api.repository.cam.ac.uk/server/api/core/bitstreams/c91e87a1-d270-47a7-8562-c0242e759221/content), abstract and introduction, and [Springer version](https://link.springer.com/article/10.1007/s11023-022-09611-z), abstract and introduction, support the reviewability and contestability propositions. Retained the Alfrink 2023 issue year, distinct from online publication in 2022. |
| Other inherited entries | Retained on the basis of the R1 integrity record. No blanket claim of fresh independent bibliographic or full-text verification; no new or previously excluded source was introduced. |

### Inherited evidence notes

These historical classifications were transcribed from the protected BibTeX. They do not constitute independent verification. The primary-source table supersedes the recorded metadata gaps only to the extent stated.

| Key | Historical evidence note |
|---|---|
| baxter2011sociotechnical | Evidence status: VERIFIED_WITHIN_R1_RECORD |
| leveson2012engineering | Evidence status: METADATA_RECONCILIATION_REQUIRED (ISBN 9780262016629 corresponds to original 2011/2012 hardback; URL points to 2016 paperback work-level record) |
| ostrom2010beyond | Evidence status: VERIFIED_WITHIN_R1_RECORD |
| stone2026legitimate | Evidence status: TEXT_PREVIOUSLY_EXAMINED as reported in R1 Foundations; exact venue, editorial date and pagination require metadata reconciliation. |
| sebastian2026decision | Evidence status: TEXT_PREVIOUSLY_EXAMINED (MIT CISR briefing examined; organizational research scope) |
| engin2026human | Evidence status: TEXT_PREVIOUSLY_EXAMINED as reported in R1 Foundations; extent of full-text inspection not independently established in consolidation verification. |
| santonidesio2018meaningful | Evidence status: TEXT_PREVIOUSLY_EXAMINED (Philosophical analysis examined in R1 Foundations) |
| green2022flaws | Evidence status: TEXT_PREVIOUSLY_EXAMINED (Legal and empirical critique examined in R1 Foundations) |
| kroll2017accountable | Evidence status: VERIFIED_WITHIN_R1_RECORD |
| cobbe2021reviewable | Evidence status: TEXT_PREVIOUSLY_EXAMINED (FAccT '21 conference paper examined in R1 Foundations) |
| alfrink2023contestable | Evidence status: VERIFIED_WITHIN_R1_RECORD |
| w3c2013provdm | Evidence status: VERIFIED_WITHIN_R1_RECORD |
| amershi2019guidelines | Evidence status: VERIFIED_WITHIN_R1_RECORD |
| kang2026institutional | Evidence status: ABSTRACT_ONLY as reported in R1 Foundations; full text unavailable in prior assessment; DOI and publication venue require metadata reconciliation. |

## Comparative contribution

| Comparator | Inherited insight and analytical overlap |
|---|---|
| Stone & Mittelstadt | Legitimate authority cannot be reduced to accuracy, fairness, acceptance or efficiency. This informs mandate validity. |
| Engin | Decision authority, operational autonomy and accountability already appear together as analytical dimensions. |
| Cobbe et al. | Evidence about human and technical processes before and after a decision supports reconstruction and review. |
| Alfrink et al. | Contestability concerns practical human intervention across a system lifecycle, including beyond a single decision. |
| Kang | The abstract overlaps directly on reliance authorization, decision authority, governed delegation, retained judgment capacity and ongoing accountability. Whether the complete preprint organizes failures equivalently remains undetermined. |

The paper connects these concerns with proposal composition, analysis, contestation and memory. The Institutional Decision Episode asks three questions about the same action: Was its mandate validly constituted? Did the action conform under the applicable rules? Was effective challenge or correction available? This structure directs inquiry toward different evidence and institutional responses: competence and issuance, execution against scope, or access and intervention. The fictional HDE-01 illustrates the distinction. Several comparators already provide analytical resources for these inquiries. No material conflict requiring theoretical revision was identified in the examined material. C2 remains C2_INTEGRATIVE_CONTRIBUTION. Distinctive originality, empirical effectiveness and universal portability remain unestablished.

## Authorship and packaging

Author, affiliation and correspondence are inherited from the v0.6 front matter at c9652a7f97018c7c740d255f0baa7b5736187826, as documented in the v0.7 integrity record. At the previous pre-review correction, those values remained AUTHOR_CONFIRMATION_PENDING. The Presidency has now confirmed the author name and correspondence and specified the updated affiliation Axodus Founder; final approval of the manuscript and disclosure by the responsible author remains pending. Source consolidation was dated 2026-11-10; candidate preparation is dated 2026-11-11. Neither date denotes publication. Identified versus anonymized review is a future packaging decision. No author, venue or reviewer was contacted.

## Historical workspace integrity

The v0.6 scientific blobs match between c9652a7f97018c7c740d255f0baa7b5736187826 and 1ef3d9237a880cf494d61ec3d53dbebb178c9b1d. This finding concerns the three scientific files, rather than every later support record in the historical directory.

| v0.6 file | Committed SHA-256 | Working-tree SHA-256 |
|---|---|---|
| paper.md | 59b03b553eaf7e390b3af57f2691e0967119a813ff1e7ead4ad883edcbd79afb | 59b03b553eaf7e390b3af57f2691e0967119a813ff1e7ead4ad883edcbd79afb |
| paper.tex | a33745f345a39b042b0eec65e0dab69c8024bccaf2da8d70da62bb6682d4ae44 | 265271b510074d889075422dc86c08cc5b37e94a10007d03da0cf4bed94617e0 |
| references.bib | 1f1b99a79bb3aff74f66c92ff103502fb04263383ca3559790ff09a330eda279 | 1f1b99a79bb3aff74f66c92ff103502fb04263383ca3559790ff09a330eda279 |

HISTORICAL_WORKTREE_CHANGE — OWNER_REVIEW_REQUIRED. The unstaged edit was present at preflight. It removes one enumitem import and two enumerate options. Neither the diff nor the prior assessment establishes who made it or why. It was preserved without restoration or incorporation.

```diff
diff --git a/papers/axodus-architecture-paper/paper.tex b/papers/axodus-architecture-paper/paper.tex
index 1ae1b43..48a76a5 100644
--- a/papers/axodus-architecture-paper/paper.tex
+++ b/papers/axodus-architecture-paper/paper.tex
@@ -5,7 +5,6 @@
 \usepackage{lmodern}
 \usepackage[margin=1in]{geometry}
 \usepackage{microtype}
-\usepackage{enumitem}
 \usepackage{tabularx}
 \usepackage{pdflscape}
 \usepackage[round,authoryear]{natbib}
@@ -271,7 +270,7 @@ decision processes?
 
 Five tensions structure the problem.
 
-\begin{enumerate}[leftmargin=*]
+\begin{enumerate}
 \item \textbf{Central constraints versus local autonomy.} A constitutional
 layer may preserve coherence, while bounded local governance domains still
 require meaningful discretion over local decisions and configurations.
@@ -323,7 +322,7 @@ the simulated AI review changed, and why escalation occurred. This scenario
 is an analytical illustration, not evidence of an Axodus implementation or
 institutional process.
 
-\begin{enumerate}[leftmargin=*]
+\begin{enumerate}
 \item constitutional governance defines the applicable roles, decision
 rights, prohibitions, amendment rules, and challenge conditions;
 \item bounded local governance domains interpret that scope for a local
```

## Integrity and validation

| Artifact | Bytes | SHA-256 |
|---|---:|---|
| Protected paper.md | 67070 | 9b7daf8e6b3aeb4a4950071b14b33ff39958e2fc67263ecad29c9fe519be53aa |
| Protected references.bib | 6830 | 8bbee88e67e4e96364d5edb18757c7d2f55d732252a644f3dbfde0ead1fd39e7 |
| Protected integrity.md | 8274 | b80f50efe29e76d9cb9fd3213882a2531765c4aab4cdf69fae68fc56108f2b1a |
| Candidate paper.md (current) | 72746 | bbc9a7d9ffbfb012bcfed0601195c0c4e5659781e5562ddc82c0afbc673e8485 |
| Candidate paper.md (prior pre-review snapshot) | 70224 | f9cd5dac6d0dec955eaa95eafaf1bdfb8d4edec4c23d4e4e2ff95588e49fb768 |
| Candidate references.bib | 5552 | 11bb4e5c20fdec2283be00d5683e43225311ad724298faf3856fc6a5eb15bd78 |

The record's own current size and SHA-256 are supplied in the final handoff. The previous candidate paper hash below is retained as the prior pre-review snapshot; it is not the current file hash.

- VAL-01 (prior correction snapshot): Five reversible citation substitutions accounted for all manuscript body differences at that stage. The later authorized author-disclosure update adds two non-scientific sections and updates author metadata; the scientific body and References remain byte-identical to that snapshot.
- VAL-02: 14 unique BibTeX keys, 14 cited works and 14 formatted references generated from the revised entries. Notes moved to this record. Independent verification remains bounded as listed above.
- VAL-03: The four dimensions, three analytical levels, canonical IDE and MC(A,M,R), three diagnostic categories, nonempirical HDE-01 and C2 maturity are preserved by exact scientific body comparison.
- VAL-04: Protected hashes and historical committed blobs verified. Compare preflight and post-write HEAD, index, and tracked diff; only three authorized paths may be new.
- VAL-05: Candidate manuscript and bibliography sizes and hashes above; record checksum is external to this record.

COND-01–10 and FR-01–10 remain binding. NC-01–10 remain open with the competent authorities recorded in the protected integrity file. No source baseline, research register or portfolio record was updated. CRO acceptance and readiness reassessment remain pending. No commit, push, merge, deployment, external disclosure, external review, submission or publication was performed.

## Author confirmation and AI-assisted research disclosure — 2026-11-11

Mandate AXODUS-RESEARCH-R1-V07-AUTHOR-DISCLOSURE-01 was expressly authorized by the CEO / Presidency in session. The Presidency confirmed Mauricio Z. Filho, Axodus Founder, and mzfshark@gmail.com for the Human–AI manuscript. RES-01 is AUTHOR_IDENTITY_CONFIRMED for those fields. The prior affiliation was Independent Researcher, Axodus; no academic appointment, credential or organizational endorsement is inferred. The responsible author's approval of the final manuscript and the disclosure remains pending. Review anonymity remains a later venue-specific packaging decision.

The working manuscript now contains Author Contributions and Responsibility and Declaration of AI-Assisted Research and Manuscript Development after Conclusion and before References. These are editorial disclosures, not new scientific sections. The human author bears intellectual responsibility; AI assistance is acknowledged without assigning authorship to an AI. The disclosure does not claim independent validation of all outputs or empirical confirmation of the framework.

### Process evidence and limits

| Activity stated | Available evidence | Qualification |
|---|---|---|
| Research structuring and conceptual organization | The in-session R1 framing, thesis brief and CRO reviews specify research questions, four dimensions, three levels and integrative scope. | These are supplied institutional/session records; no unsupported claim about a particular earlier model. |
| Literature mapping and conceptual comparison | User-supplied R1 Foundations and Gate 02 descriptions; this pre-review record, Comparative contribution and Bibliographic verification sections. | Prior phase results are reported by institutional records. Current pre-review reconciliation directly examined selected sources; Kang remains ABSTRACT_ONLY. |
| Analytical development, critique and scientific-review support | User-supplied CRO findings SCI-01–08 and S2-SCI-01–08, the correction mandates and the integration assessment in this record. | Evidence establishes documented review and correction workflow, not independent validation of every proposition or output. |
| Drafting and editorial preparation | User-supplied Stage 1 and Stage 2 handoff and correction records; protected v0.7 integrity record, sections 1 and 3, describes consolidation from accepted texts. | The complete original drafting transcripts and every tool identity are not independently established by the files examined. |
| Bibliographic reconciliation and documentary integrity | This pre-review record, bibliography table, change inventory, and integrity evidence; in-session execution of the pre-review corrections. | Source checks were bounded, not a systematic re-verification of all references. |
| Human-directed decisions | User-supplied Presidential authorizations, CRO review dispositions and present explicit metadata confirmation. | These establish recorded decision gates, not that each AI output was independently reviewed or validated. |

### AI system identification

| Phase | Service / agent | Model | Evidence and limitation |
|---|---|---|---|
| Pre-review bibliographic/editorial reconciliation and current disclosure preparation | OpenAI Codex coding assistant | AI_TOOL_METADATA_NOT_VERIFIED | The present Codex execution environment and tool transcript identify the assistant/service and document these operations; exact model and version are not supplied. |
| Earlier R1 Foundations, Gate 02, Stage 1 and Stage 2 | AI_TOOL_METADATA_NOT_VERIFIED | AI_TOOL_METADATA_NOT_VERIFIED | The institutional and session records describe AI-assisted work but the inspected artifacts do not independently identify the complete set of providers, tools or model versions. A prior contextual checkpoint reports a Gemini model, but that report alone does not independently verify which phase used it or its precise identity. Author confirmation and contemporaneous records remain necessary. |

### Disclosure compatibility and outstanding review

The structure is consistent in principle with ICMJE's published guidance that authors disclose the use and purpose of AI tools and retain responsibility for accuracy and integrity, and that AI tools not be listed as authors: https://www.icmje.org/recommendations/browse/artificial-intelligence/ai-use-by-authors.html . ICMJE is a medical-journal framework, not an automatically applicable policy for this manuscript. The future target venue's disclosure, placement and tool-identification requirements remain to be checked. The current declaration is incomplete for external submission until the unverified earlier tool identities and model details are resolved or explicitly disclosed as unavailable and the responsible author approves the final manuscript and declaration.

### Scope and validation

The author's name and email are unchanged, affiliation is exactly Axodus Founder, and the author status states confirmed identity while reserving final approval. All ten scientific sections, the abstract and References section match the immediate pre-edit candidate byte for byte. The bibliography and protected v0.7 checksums remain unchanged. The pre-existing v0.6 paper.tex working-tree change remains untouched. Current paper size and hash are shown in the integrity table; the record's own hash is supplied externally in the handoff. No commit, push, merge, deployment, external circulation, external review or publication is authorized or performed.
