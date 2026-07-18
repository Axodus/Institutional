# Website Integration Record

Publication: `PUB-ADS-001`

Canonical path: `/publications/architecture-specifications/ads-001/`

Status: `CONTRACT_READY`

## Required rendering

- Breadcrumbs: `Home > Publications > Architecture Specifications > ADS-001`.
- Page title from `metadata.yaml`.
- Summary and canonical path from metadata.
- Cover image from `assets/ads-001-cover.svg` with its accessible title and
  description.
- Link to the GitHub source and the ADS-001 version record.
- Documentation CTA remains configuration-dependent until an approved
  canonical destination exists.
- No link to the blocked paper v0.6 as a released related publication.

## Draft behavior

Until `release-decision.md` becomes authorized, the page must use `noindex`,
remain outside the public sitemap, and display the Draft v0.6 status.

The current `Axodus/website` checkout was not modified because it has no
publication-content pipeline and is a separate prototype surface.
