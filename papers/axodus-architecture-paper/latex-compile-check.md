# LaTeX Compile Check

Review date: 2026-07-03  
Target: `papers/axodus-architecture-paper/paper.tex`

## Toolchain availability

- `pdflatex`: available at `/usr/bin/pdflatex`
- `bibtex`: available at `/usr/bin/bibtex`
- `latexmk`: available at `/usr/bin/latexmk`
- `biber`: available at `/usr/bin/biber`

## Compile command used

From `papers/axodus-architecture-paper`:

```bash
latexmk -pdf paper.tex
```

## Result

- Pass/fail: **Pass**
- `paper.tex` technically compilable: **yes**
- Paper content changes required to compile: **none**

## Warnings

- `latexmk` reported a filesystem/system-time offset warning while comparing
  file timestamps between the execution environment and the mounted workspace.
- First-pass `natbib` undefined-citation warnings appeared before `bibtex`
  ran; they resolved during the normal `latexmk` build cycle and were not
  present as final compile errors.

## Errors

- None.

## Generated files

The successful compile generated these LaTeX outputs during the check:

- `paper.aux`
- `paper.bbl`
- `paper.blg`
- `paper.fdb_latexmk`
- `paper.fls`
- `paper.log`
- `paper.out`
- `paper.pdf`

## Cleaned files

Cleanup actions performed after the compile check:

- `latexmk -c paper.tex`
- `latexmk -C paper.tex`
- explicit removal of residual `paper.bbl`

Files removed by cleanup:

- `paper.aux`
- `paper.bbl`
- `paper.blg`
- `paper.fdb_latexmk`
- `paper.fls`
- `paper.log`
- `paper.out`
- `paper.pdf`

## Ignore rules

The repository did not contain a root `.gitignore`. A minimal root
`.gitignore` was added to exclude LaTeX build artifacts and generated paper
PDFs, including `papers/**/*.pdf`.

## Remaining blockers

- No compile-blocking LaTeX syntax issues were found in `paper.tex`.
- The `latexmk` filesystem/system-time skew warning should be kept in mind when
  interpreting timestamp-based rebuild behavior in this mounted workspace.
- This check does not change publication readiness. Human review, approved
  public correspondence metadata, and the other blockers listed in
  `publication-readiness.md` remain in force.
