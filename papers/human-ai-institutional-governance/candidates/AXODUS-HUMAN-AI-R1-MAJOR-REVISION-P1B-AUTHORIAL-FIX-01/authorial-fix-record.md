# Authorial fix — P1-B

Directive: AXODUS-CRO-REQ-HUMAN-AI-P1B-AUTHORIAL-FIX-01. Working copy: AXODUS-HUMAN-AI-R1-MAJOR-REVISION-P1B-AUTHORIAL-FIX-01, uncommitted and pending author and CRO review. Source: AXODUS-HUMAN-AI-R1-MAJOR-REVISION-P1B-01, Institutional main HEAD af252298edacf8103a76e4ee8a3fa3136e0cd153. The unchanged manuscript front matter retains its historical P1-B identifier and prior status; this record identifies the derived working copy. The original review record and historical diff remain with the original candidate.

FIX-01 removed the single Kang discussion in §2.4 and its paper and BibTeX references. FIX-02 removed only the operational search date in §2.5. The full diff is authorial-fix.diff. No other paper or bibliography text was changed.

Original paper SHA-256: 4b7c1fea6fa71aaf1aa0832b5091aab85c61d7cf484b7c1af073448007082051
Original bibliography SHA-256: 66691b1def7edaf824ed9fba113af4f51072ee848d5d331a7f941918a1cc80b3
Derived paper SHA-256: 41616bffc80b5aa487ea1fae0b49099292fbb3af490dce5f6e860cb098eb28c6
Derived bibliography SHA-256: a7ea77ac1a3d17e9957c4ba216f91f8fb45b79c22bea010654dff13a8fcaa26c
Diff SHA-256: 9a05e898b7e5a3c027373d098b69cd8fc767be20ac7c81335a0f82f005d7fb79

Bibliographic inventory: 20 entries, down from 21; surviving BibTeX keys: baxter2011sociotechnical, leveson2012engineering, ostrom2010beyond, stone2026legitimate, sebastian2026decision, engin2026human, santonidesio2018meaningful, green2022flaws, kroll2017accountable, cobbe2021reviewable, alfrink2023contestable, w3c2013provdm, amershi2019guidelines, simon1978rational, galbraith1974organization, hollan2000distributed, walsh1991memory, levitt1988learning, gonzalez2026teaming, vaccaro2024combinations. The internal paper reference list also contains 20 entries. This count does not itself verify external bibliographic metadata or every citation's source support.

The remaining literature and access limitations, independent analyst replication, source verification and author final approval remain open. The original Kang abstract-only finding remains historical and is not a claim about the present bibliography. No baseline promotion, commit, remote operation or publication is authorized by this record.

## Validation evidence

- V-01 PASS: case-insensitive search for `kang|7339378` in the derived paper and bibliography returned no matches. Historical source records and the diff intentionally preserve the removed text for provenance.
- V-02 PASS: §2.4 retains all other comparator sentences and its bounded-contribution paragraph unchanged; the complete patch exposes the only deletion.
- V-03 PASS: §2.5 differs only by removal of `on 13 November 2026`; all three methods, selection and search descriptions, access levels, exclusions and future evaluation requirements are byte-preserved.
- V-04 PASS WITHIN DIFF SCOPE: reconstructing the new manuscript from the historical text using exactly the three intended string substitutions yields the derived paper; no general scientific review was performed.
- V-05 PASS WITH LIMITS: 20 in-text reference-list entries correspond to 20 surviving BibTeX records by lead author and year; all 20 have a matching author-year mention in the body (W3C confirmed separately). No Kang citation or entry remains. External source accuracy and exhaustive semantic citation support were not independently audited.
- V-06 PASS: only the four new files in this candidate were created; all four files of the historical candidate match Git HEAD; no staging, commit or remote operation occurred. Source front matter still identifies the historical P1-B candidate and its previous workflow status; this separate record identifies the derivative, so downstream rendering must use the derivative directory and author review should resolve metadata before further circulation.
