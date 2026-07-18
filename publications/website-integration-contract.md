# Website Integration Contract

This contract defines how a future website publication renderer consumes the
generic publication package. It is not an implementation of the current
Axodus website.

## Required input

- `metadata.yaml` validated against `schema/publication-metadata.schema.json`;
- the versioned Markdown source;
- the publication readiness report;
- the release decision;
- the referenced cover asset.

## Route and navigation

- Use `canonical_path` as the stable route.
- Render breadcrumbs from the series and document identifiers.
- Link to the source repository and the current version record.
- Render a documentation CTA only when the website configuration supplies an
  approved canonical documentation destination; never invent a destination.
- Render previous and next publications only when their release status is
  authorized.

## SEO and release behavior

- Use `title`, `summary`, `canonical_path`, `publication_date`, and `cover` for
  page metadata.
- Draft and unauthorized documents must use `noindex` and must not be added to
  a public sitemap.
- Released documents may be added to the sitemap only after the matching
  release decision is authorized.
- Do not expose a related paper or note whose own release gate is blocked.
