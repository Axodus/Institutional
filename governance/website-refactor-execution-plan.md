# Axodus Institutional Website Refactor and Execution Plan

Status: Planning only; no website checkout or production deployment is authorized by this document

## Overview

Refactor `axodus.country` so its visible narrative, information architecture,
entity metadata, social previews, and crawl controls consistently use the
canonical Axodus identity. The work should improve clarity and make the
intended entity easier for consuming systems to interpret; search ranking,
indexing, Knowledge Graph inclusion, and social distribution remain
provider-controlled outcomes and are not guaranteed.

The Institutional repository is the source of truth for wording and
boundaries. The website implementation is a separate surface and was not
available in this repository during planning.

## Success criteria

- The homepage answers “What is Axodus?” in the first viewport and in plain HTML text.
- The canonical description matches `governance/institutional-identity.md` exactly.
- Legacy DAAS/ETF and investor-focused positioning is absent from current navigation, title tags, descriptions, and social cards.
- Every public page has one canonical URL, an appropriate title and description, and an explicit publication status.
- JSON-LD, Open Graph, sitemap, and internal links pass validation.
- Draft or unauthorized content is not indexable or included in the sitemap.
- No page introduces unsupported implementation, adoption, partnership, performance, financial, regulatory, or security claims.

## Non-goals

- No promise of higher ranking, faster indexing, entity-panel inclusion, or changed answers from Google or language models.
- No creation of Wikipedia, press coverage, backlinks, or external outreach as part of this refactor.
- No disclosure of private repositories, source code, credentials, infrastructure, tokenomics, financial strategy, or operational controls.
- No redesign of product applications or unrelated domain properties.

## Actors and interfaces

| Actor or system | Responsibility / interface |
|---|---|
| Institutional content owner | Approves exact wording, taxonomy, status labels, and release scope |
| Website frontend | Renders pages, metadata, JSON-LD, navigation, and social tags |
| Content source | Stores approved page content and status metadata; preserves provenance |
| Webmaster console | Verifies domain ownership and reports crawl/structured-data observations |
| Social link scrapers | Consume Open Graph/Twitter metadata; behavior is external |
| QA reviewer | Checks claims, links, accessibility, rendering, and release gates |

## Work packages

### WP1 — Baseline and inventory

Obtain the website checkout or CMS export from the maintainer. Capture the
route, title/description, redirect, sitemap, robots, structured-data, and
social-tag inventories. Search source and rendered content for legacy DAAS,
ETF, investor, financial-return, “first”, “unique”, and other ambiguous
language. Record each proposed change with URL, current text, replacement text,
evidence class, and reviewer.

**Interface:** route manifest plus content-audit record.

### WP2 — Information architecture

Adopt a shallow, crawlable structure:

```text
/
├── /what-is-axodus/
├── /architecture/
├── /governance/
├── /research/
├── /publications/
└── /platforms/ (only for approved, bounded institutional pages)
```

The homepage and `/what-is-axodus/` link to the identity record, taxonomy,
research/publications, and approved product pages. Do not create pages merely
to occupy keywords.

### WP3 — Content refactor

Use this page sequence: identity block; scope block; ecosystem block; evidence
block; status block; and boundary block. The blocks must use the canonical
description, prototype-stage qualification, proposed-concept language, links
to evidence records, and explicit limitations. Product names are allowed only
with the controlled conceptual boundaries in the taxonomy.

### WP4 — Entity and metadata implementation

Implement the JSON-LD template from `governance/entity-seo-technical-plan.md`,
using one stable organization `@id` and verified `sameAs` URLs only. Add
`WebSite` and `WebPage` nodes to the homepage and identity page. For each
indexable page implement a unique title, bounded description, canonical URL,
Open Graph fields, equivalent social-card metadata, and an agreed language
declaration. Draft content must remain `noindex`.

### WP5 — Crawl and link controls

Generate a sitemap from approved indexable routes only. Keep canonical URLs
stable, use explicit 301 redirects for approved route changes, and treat
`robots.txt` as a crawl directive rather than a privacy boundary. Remove broken
links, redirect chains, duplicate canonicals, and orphaned identity pages.

### WP6 — Social presentation

Create one approved default social card representing the research-driven,
prototype-stage identity. Do not use financial imagery, price or return
language, or legacy slogans. Verify the card at its final canonical URL.

## Data flow and ownership

```text
Approved identity/taxonomy → content model + page status
        → HTML renderer → metadata / JSON-LD / social cards
        → sitemap + robots + internal links
        → search and social consumers (observed, not controlled)
```

The content model must retain page status, canonical URL, source record, last
review date, and reviewer. Build output should fail when a required field is
missing or when draft content is marked indexable.

## Validation gates

### Pre-merge

- Content audit shows no current legacy slogan or unsupported claim.
- Canonical description matches the identity record after normalization.
- Internal links resolve and redirects are intentional.
- JSON-LD parses and uses only verified URLs.
- Accessibility checks cover headings, link names, contrast, images, and keyboard navigation.

### Staging

Inspect rendered HTML for every route class. Verify title, description,
canonical, robots, Open Graph, and JSON-LD. Confirm drafts are `noindex` and
absent from the sitemap. Run performance checks as observations, not
guarantees.

### Release review

A named human reviewer approves the exact content and route set. Each
publication page has an authorized release decision. Domain ownership and
webmaster-console access are verified. A rollback revision and redirect map
are stored before production change.

### Post-release observation

Record crawl errors, indexing state, structured-data warnings, social-card
rendering, and referral observations at defined intervals. These are
measurements of external systems, not proof that the strategy caused a
particular outcome.

## Rollout and rollback

1. Build behind staging or preview.
2. Freeze the approved content snapshot and route manifest.
3. Run validation gates and obtain human approval.
4. Deploy content, redirects, and sitemap as one versioned release.
5. Keep the previous route map available for rollback.
6. If claims or crawl directives are incorrect, revert to the last approved release and repair the source record.

## Open questions and dependencies

- Which repository or CMS contains the current `axodus.country` source?
- Which routes are public, draft, or blocked?
- Which logo and social-card assets are approved?
- Which translations are maintained and who approves them?
- Who owns domain verification, sitemap submission, and post-release review?
- Is analytics collection authorized, and what privacy policy governs it?

These questions must be resolved before implementation. This plan does not
authorize access to an external website, deployment, webmaster console, or
social account.
