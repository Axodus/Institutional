# Invariant and validation report

Verification: 2026-11-17, local documentary comparisons. PASS means scoped textual verification, not CRO scientific acceptance or independent human translation review.

| Gate | Result | Evidence / limit |
|---|---|---|
| RA-01 | PASS | Introduction and §10 identify framework as main contribution; concluding thesis retained. |
| RA-02 | PASS | §1 and §3–5 preserved; four named dimensions precede IDE and are not derived from it. |
| RA-03 | PASS | §5 byte-identical and introductory three levels retained. |
| RA-04 | PASS | Abstract, §1, §6.1 and §10 designate supporting device; contexts throughout inspected. |
| RA-05 | PASS | §2.2 and §2.4 distinguish framework and instrument; no uniqueness claimed. |
| RA-06 | PASS | Two comparative paragraphs identical and moved to §8.11; §10 and Appendix A.4 retain findings and unestablished hold disposition. |
| RA-07 | PASS | §6.1 from display equation through §6.2 byte-identical: tuple, MVA, MC, statuses and limits unchanged. |
| RA-08 | PASS | Changes limited to contribution hierarchy, placement and candidate metadata; full diff provided. Conceptual framing is proposed pending CRO review. |
| RA-09 | PASS | Genealogy provides local v0.7 Git, document dates and qualified attribution; no claim of global priority. |
| RA-10 | PASS | Six protected historical files and five source candidate files match preflight hashes; copied bibliography byte-identical. |
| RA-11 | PASS WITH QUALIFICATION | Nine material change entries contain Portuguese versions; checked for content and retained numbers. No independent professional translation review. |
| RA-12 | PASS | Nine focused entries cover material wording and relocation; front matter identification logged separately. |

## Hashes — protected historical files

- `v0.7/paper.md`: `9b7daf8e6b3aeb4a4950071b14b33ff39958e2fc67263ecad29c9fe519be53aa`
- `v0.7/references.bib`: `8bbee88e67e4e96364d5edb18757c7d2f55d732252a644f3dbfde0ead1fd39e7`
- `v0.7/integrity.md`: `b80f50efe29e76d9cb9fd3213882a2531765c4aab4cdf69fae68fc56108f2b1a`
- `pre-review/v0.7.1/paper.md`: `bbc9a7d9ffbfb012bcfed0601195c0c4e5659781e5562ddc82c0afbc673e8485`
- `pre-review/v0.7.1/references.bib`: `11bb4e5c20fdec2283be00d5683e43225311ad724298faf3856fc6a5eb15bd78`
- `pre-review/v0.7.1/pre-review-record.md`: `2e0f5883fcaf94887ad616b1ebde3b26e493e2e3a8ffff1b7beb8130e9e49555`

## Source candidate — preflight and after (identical)

- `paper.md`: `bcc8e639f63d482565a97d692f6d21b8125cbe763ded1012f87e1b1f07735f79`
- `references.bib`: `a7ea77ac1a3d17e9957c4ba216f91f8fb45b79c22bea010654dff13a8fcaa26c`
- `targeted-authorial-revision-record.md`: `c63b6b359a2526ab32971abaa0bbfd5aa6e263722ea0829fa11006caef55149e`
- `targeted-authorial-revision-validation.md`: `92f9547a1b8843ad20b62f828b556eff5311a8a720e2bcbc2763b94e05f787ba`
- `targeted-authorial-revision.diff`: `2d19d5e47d1ce4896e8c2448e989bd3793d7c2dab8dc95a53a42ec425c008051`

## Candidate artifact hashes

- `alignment-record.md`: `b93b909b85c33b53e3ac1d6dbe67d198f5cd2fd9ac6353caf499dd0a1553a59c`
- `focused-author-review.md`: `794d3d073260a11b4c46c1d6257db2c723b312fbdbc8c746b8d39f7dddb4a1c5`
- `ide-genealogy.md`: `45838dc2acbc01d78c88485e7c089690bda2d9db70fbf8bc1c73b98888c47bbf`
- `ide-positioning-realignment.diff`: `2e2eb65ac533e14098da1359c53d4ab372414394d623a7af9eab41d643e736fc`
- `paper.md`: `abd95841701402245443d9abf51187db27b4c683779187a3eade95b243cab4a4`
- `references.bib`: `a7ea77ac1a3d17e9957c4ba216f91f8fb45b79c22bea010654dff13a8fcaa26c`

During verification the repository HEAD changed concurrently from b20755af2d9b5968973728cf1c2e5981edda15bf to e968251f457124990bfbb49edd1bbd716db0fa7f; that external commit included the five original candidate files and six in-progress derivative files. This executor did not stage or commit. The alignment record was subsequently updated to correct provenance, and this validation file remains uncommitted. Investigate the unexpected commit before CRO acceptance. This record does not embed its own hash; report it independently in the execution handoff. No empirical, interanalyst, external-review or publication claim is made.
