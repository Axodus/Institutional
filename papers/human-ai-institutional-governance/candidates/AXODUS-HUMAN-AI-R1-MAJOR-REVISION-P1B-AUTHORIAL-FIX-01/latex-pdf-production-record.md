# LaTeX and PDF production record

Mandate: AXODUS-CRO-MANDATE-HUMAN-AI-P1B-LATEX-PDF-01. Disposition: LATEX_PDF_PRODUCTION_INCOMPLETE / CORRECTION_REQUIRED; CRO review pending. This is a presentation derivative, not a new scientific baseline.

## Inputs and tools

Institutional branch `main`, source HEAD `92bd0b900bb4342a0006872271b367f594ef6fc5`; clean worktree before production. Approved source identity: AXODUS-HUMAN-AI-R1-MAJOR-REVISION-P1B-AUTHORIAL-FIX-01.

| File | SHA-256 |
|---|---|
| paper.md | `41616bffc80b5aa487ea1fae0b49099292fbb3af490dce5f6e860cb098eb28c6` |
| references.bib | `a7ea77ac1a3d17e9957c4ba216f91f8fb45b79c22bea010654dff13a8fcaa26c` |
| paper.tex | `3869c75ec745dcc5b814cd24b0da48020f99840f78d32d7509526a619b5ba006` |
| paper.pdf | `4de40eda5fc3f54abaf44fb2fa784723f1a85b181f08f6f9364557f6f08de57d` |

Pandoc 3.9 from `pypandoc_binary` 1.17 isolated in `/tmp/axodus-pandoc-runtime`; LuaHBTeX 1.22.0, TeX Live 2025/Debian; Poppler `pdftotext`, `pdfinfo`, `pdftoppm`. The Lua font-loader package `texlive-luatex` (Ubuntu 2025.20260124-1) was downloaded and extracted under `/tmp/axodus-p1b-luatex`, without system installation. These temporary dependencies are not guaranteed to persist.

## Commands and formatting

The source was copied to `/tmp/axodus-p1b-latex-build/source.md`, changing only the presentation metadata for candidate identity and status; the source file itself was not modified. Conversion:

```
pandoc source.md -f 'markdown-tex_math_dollars+tex_math_single_backslash' -t latex --standalone --variable documentclass=article --variable fontsize=10pt --variable geometry:margin=0.8in --variable linestretch=1.05 --variable colorlinks=true -o paper.tex
```

Dollar math was disabled to preserve monetary amounts; backslash-delimited mathematics remained enabled. The generated TeX was adjusted to show the approved identity and the existing author, affiliation and email. Long tables use `longtable`. Compilation, using the extracted font loader, was:

```
TEXINPUTS='/tmp/axodus-p1b-luatex/usr/share/texlive/texmf-dist/tex//:' \
LUAINPUTS='/tmp/axodus-p1b-luatex/usr/share/texlive/texmf-dist/tex//:' \
lualatex -interaction=nonstopmode -halt-on-error -output-directory=/tmp/axodus-p1b-latex-build paper.tex
```

The compiled PDF was copied to the candidate directory. The final run exited successfully and produced 25 letter-size pages. There are two `ignored error Infinite glue shrinkage found in box being split` messages, near pages 3–4 and 23–24. These are unresolved pagination warnings and cannot be dismissed as cosmetic solely on compilation. An earlier label-change warning did not recur on the final run; no missing-glyph, undefined-reference or overfull-box warning appeared in the final output. The original bibliographic entries are printed from Markdown as authored; no citation keys were introduced.

## Validation

| Gate | Result and evidence |
|---|---|
| V-01 | PASS: HEAD and both source hashes match the approved reference. |
| V-02 | PASS structurally: Pandoc parsed 74 headings and produced 74 section macros, three tables, two bullet lists and three ordered lists. This alone is not paragraph-level proof. |
| V-03 | PARTIAL: token-order comparison between Pandoc plain output and PDF extraction matched 12,742 of 12,993 source tokens. Table columns are read in a different order by `pdftotext -layout`; this check does not establish complete paragraph-level equivalence. |
| V-04 | PARTIAL: all 19 distinct source math expressions, representing 47 occurrences, appear literally in TeX. PDF page montage and final first and table pages were visually inspected; no clipping was observed, but complete formula-by-formula and cell-by-cell semantic verification was not established. |
| V-05 | PARTIAL: 20 approved BibTeX entries and the Markdown reference list were preserved, and Kang is absent from TeX. Author-date citations are literal manuscript text; `references.bib` was not integrated into BibTeX compilation and automatic citation resolution is not demonstrated. |
| V-06 | PARTIAL: PDF compiled, but two infinite-glue-shrinkage warnings remain unresolved. |
| V-07 | PASS with scope: a 25-page contact sheet of the initial rendering and the final first page and appendix table pages were visually inspected; the contact sheet predates the final title-metadata change. |
| V-08 | PASS: input and output hashes and commands are recorded here. |
| V-09 | PASS: paper.md and references.bib retained their original hashes. |
| V-10 | PASS: no source scientific text edited, no commit, push, publication, or baseline promotion. |

Remaining work before documentary acceptance: implement and verify a bibliography integration that preserves the approved reference list and author-date wording; investigate the pagination warnings; perform a complete paragraph, formula, citation and table correspondence audit and inspect the final render across all pages. Do not represent successful compilation as proof of equivalence.

## Corrective delivery — AXODUS-CRO-FIX-HUMAN-AI-P1B-LATEX-PDF-01

The preceding section records the first, superseded production attempt. Current disposition: **LATEX_PDF_PRODUCTION_COMPLETE / CRO_REVIEW_PENDING**. The approved source and its SHA-256 values above are unchanged. The working copy and Git objects at `92bd0b900bb4342a0006872271b367f594ef6fc5` were compared byte for byte for both canonical inputs.

### Current artifacts

| File | SHA-256 |
|---|---|
| paper.tex | `5648f220768e904474ff5d050e955db10f0eab1e85de62d85d3f9787a7f21eee` |
| paper.pdf | `82e7d2ecda5c99d3b33db068ff9530b6633e8e9c8cfcdfec9c3cda9640ec9258` |
| axodus-authorial.bst | `3ee8c2d680f5459959ac751ac7b8561721c78f70db5c00a9bf8a2eef3d1edb5b` |

The style is derived from plainnat 1.93 under its existing license. It preserves title casing, adds article identifiers and page counts, prints report editors and formats DOI links. The ampersand in the Green journal title is escaped for TeX in the style rather than edited in the source database. A URL identical to the canonical DOI link is printed once. References render in alphabetical order; the style displays full given names from the approved database, changes field punctuation and ordering, and adds the database's publication month for the W3C entry. These are presentation differences, not additions of sources. The approved manuscript's inline labels, punctuation, years and citation order are preserved, including the W3C expansion and abbreviation. Their author labels link to the matching bibliography anchor; natbib resolves the years by key via the BibTeX-generated entries. No literal years remain at the mapped citation sites.

### Reproduction

Copy paper.tex, references.bib and axodus-authorial.bst to a clean build directory. Run, in order, with LuaHBTeX 1.22.0 with luaotfload available and BibTeX 0.99d:

```sh
lualatex -interaction=nonstopmode -halt-on-error paper.tex
bibtex paper
lualatex -interaction=nonstopmode -halt-on-error paper.tex
lualatex -interaction=nonstopmode -halt-on-error paper.tex
```

The build uses the Lua font-loader paths recorded above in this environment. The first pass can report unresolved citations before BibTeX; the settled final log contained none. The temporary build evidence for this run is in `/tmp/axodus-p1b-final.OrV6LV/` (logs, output database, extraction and correspondence script; ephemeral). No auxiliary build cache was placed in the repository. Cite links were checked with Poppler destination output.

| Gate | Corrective result and evidence |
|---|---|
| CV-01 | PASS. BibTeX logged `Database file #1: references.bib` and loaded axodus-authorial.bst. The generated BBL supplied the published-in-PDF reference list. |
| CV-02 | PASS. The exact multiset of 30 source citation commands agrees with AUX requests; 20 unique keys have AUX labels, BBL entries and PDF destinations. No undefined or multiply defined citation in the settled run. |
| CV-03 | PASS. The 20 approved keys equal the 20 generated entry keys, without duplicates; Kang and 7339378 absent. Compared 123 data field occurrences from BibTeX to BBL (including all 20 titles and years, article IDs, counts, available pages, DOI and distinct URLs); redundant DOI URLs were consolidated and format changes are identified above. |
| CV-04 | PASS. A fresh Pandoc conversion from the canonical Markdown agreed exactly with the original TeX body and Appendix A. Reversing the corrected TeX citation and layout substitutions recovered that reference content. Poppler `pdftotext -raw` was used to retain row and cell order. From abstract through author declarations, 67,585 normalized characters matched in order; Appendix A matched for 10,537 normalized characters. Normalizations were Unicode typography and whitespace, soft line-end hyphens (six and three respectively), list markers, PDF page numbers, Markdown table rulers and one repeated header in each of two tables. The separately generated bibliography was verified under CV-03. |
| CV-05 | PASS. All 47 math occurrences matched exact TeX expression strings after trimming surrounding whitespace. The source parser reports 19 distinct raw strings; the displayed and inline canonical tuple merge to 18 after trim, with both forms and all occurrences retained. The sequential content comparison includes all 47 cells of the three tables (15, 12, 20), including headings. |
| CV-06 | PASS. The 74 headings and hierarchy are preserved by regenerated-source comparison and 74 auxiliary labels. The Appendix A text, four linked episodes, lists (two bullet and three ordered) and literal cross-references survive in their original order. Source AST has no footnote nodes. |
| CV-07 | PASS. All 25 final pages were rendered with Poppler at 72 dpi and inspected in 5-page strips. Pages 4–5 and 24–25 were also inspected individually; no truncation, overlap or missing rows was observed. |
| CV-08 | PASS WITH QUALIFICATION. Two residual LuaTeX `Infinite glue shrinkage found in box being split` diagnostics remain at multipage table starts (Section 3.2, p. 4; Appendix A.4, p. 24). Both reproduce in the original build. The intermediate table (§5.4, p. 9) does not emit it. Trace of the longtable entry probe narrowed the affected context to table start and page splitting; the exact emitting glue node was not isolated. Fixed local spacing, direct paragraph-column headers and removal of the exploratory footnote wrapper did not eliminate the warnings. Widening the two dense appendix columns removed a two-line overflow onto an otherwise mostly empty page. The final row/cell extraction and page images show correct breaks and repeated heads, no missing data or overlaps; the two diagnostics are non-material in this output. No final fatal error, missing glyph, undefined citation or overfull box observed. |
| CV-09 | PASS. Both canonical inputs were byte-identical to the reference commit after the build and retain the input hashes in the first table above. |
| CV-10 | PASS. The diff against the first TeX production is limited to citation substitution and links, automatic bibliography, and table composition. Only the three deliverables and the necessary style changed. No scientific change, commit, push, merge, baseline promotion, external submission or publication. |

**Global Coordination Handoff** — Institutional, `main`, HEAD `92bd0b900bb4342a0006872271b367f594ef6fc5`. Scope: two corrected derivatives, one required build style and this production record. Validation: CV-01–CV-10 above; CRO documentary acceptance pending. The index remains empty, the approved sources are unchanged, and only these local uncommitted artifacts are present (PDF ignored by Git). The build depends on LuaHBTeX with luaotfload, BibTeX and the approved source database. No change of priority or request for a portfolio action.
