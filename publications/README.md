# Axodus Publications

This directory is the reusable editorial infrastructure for public Axodus
publication series. It separates publication identity, versioned source
documents, readiness evidence, release authorization, and website delivery.

## Active series

- [Architecture Specifications](architecture-specifications/README.md)

## Future-compatible series

The infrastructure is also reserved for Architecture Notes, Engineering Notes,
Governance Notes, Research Notes, White Papers, Technical Reports, and Position
Papers. A series must not be treated as active until its own content and
release gates are opened.

## Control order

1. `metadata.yaml` identifies the publication and version.
2. The versioned Markdown file is the source document.
3. `publication-readiness.md` records technical and editorial readiness.
4. `release-decision.md` records whether publication is authorized.
5. Review records preserve independent editorial, scientific, technical, and
   brand decisions.

The presence of a document in this directory does not authorize external
publication, submission, outreach, or distribution.

The contracts are designed to serve as a future foundation for a BBA
Publishing Platform. No active BBA platform, release channel, or operational
publishing service is asserted by this repository.
