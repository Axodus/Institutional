# Axodus Entity and SEO Technical Plan

Status: Planning only; implementation and publication require separate approval

## Scope

This plan specifies how a future Axodus website could expose a consistent
institutional entity through structured data, metadata, links, and controlled
indexing. It is not an implementation, an SEO guarantee, or a claim that a
search engine or language model will change its classification.

## 1. Canonical entity inputs

Use the exact description from [institutional identity](institutional-identity.md):

> Axodus is a research-driven initiative developing a proposed ecosystem of
> interoperable, AI-native organizational platforms for governed knowledge,
> institutional workflows, and digital services.

Before deployment, a human maintainer must verify the canonical domain, public
repository URL, logo asset, contact details, and any external profile URLs.
Do not add an unverified affiliation, legal entity, partner, product status,
or social profile to structured data.

## 2. JSON-LD proposal

Render one `@graph` on the canonical institutional homepage and reference the
same stable `@id` from other pages. The following is a template; values marked
for verification must not be invented by the renderer.

```json
{
  "@context": "https://schema.org",
  "@graph": [
    {
      "@type": "ResearchOrganization",
      "@id": "https://axodus.country/#organization",
      "name": "Axodus",
      "url": "https://axodus.country/",
      "description": "Axodus is a research-driven initiative developing a proposed ecosystem of interoperable, AI-native organizational platforms for governed knowledge, institutional workflows, and digital services.",
      "sameAs": [
        "https://github.com/axodus/",
        "https://github.com/Axodus/Institutional",
        "https://docs.axodus.country/",
        "https://axodus.medium.com/",
        "https://axodus.substack.com/",
        "https://axodus.notion.site/Axodus-39355b1b6c9880f884ade5ce28b4dc6d"
      ]
    },
    {
      "@type": "WebSite",
      "@id": "https://axodus.country/#website",
      "url": "https://axodus.country/",
      "name": "Axodus",
      "publisher": {"@id": "https://axodus.country/#organization"}
    },
    {
      "@type": "WebPage",
      "@id": "https://axodus.country/#webpage",
      "url": "https://axodus.country/",
      "name": "What is Axodus?",
      "isPartOf": {"@id": "https://axodus.country/#website"},
      "about": {"@id": "https://axodus.country/#organization"}
    }
  ]
}
```

The `ResearchOrganization` type describes the intended institutional framing;
it does not establish legal incorporation, accreditation, research funding,
or external recognition. `sameAs` is an identity assertion and must contain
only URLs that the maintainer has verified as official. The current proposed
official-channel set is:

- GitHub organization: <https://github.com/axodus/>
- Institutional repository: <https://github.com/Axodus/Institutional>
- Documentation: <https://docs.axodus.country/>
- Medium: <https://axodus.medium.com/>
- Substack: <https://axodus.substack.com/>
- Notion: <https://axodus.notion.site/Axodus-39355b1b6c9880f884ade5ce28b4dc6d>

These links identify related publisher channels; they do not make their
contents equivalent to the controlled Institutional repository or guarantee
that every page is current, reviewed, or indexable.

## 3. Page metadata

The homepage and `What is Axodus?` page should have one stable title,
description, canonical URL, and language declaration. Suggested values:

- title: `Axodus — Research-driven AI-native organizational platforms`
- description: the canonical description above, optionally followed by the
  prototype-stage limitation;
- canonical: the one approved HTTPS URL for the page;
- `robots`: `noindex, nofollow` while the page is draft or not authorized for
  public release; normal indexing directives only after approval;
- Open Graph and Twitter metadata using the same title, description, URL, and
  an approved image.

Do not use keyword stuffing, unverifiable claims, hidden text, or legacy
financial-product slogans in metadata.

## 4. Cross-linking contract

The institutional homepage, `What is Axodus?`, GitHub organization/repository,
and approved product pages should link to one another using descriptive anchor
text. Each link must be checked for ownership and destination status before
publication.

Minimum relationship set:

```text
Axodus homepage → What is Axodus?
Axodus homepage → Institutional repository
Axodus homepage → Documentation
What is Axodus? → institutional identity and taxonomy
Institutional repository → approved canonical website and documentation
Product page → Axodus identity and its own status boundary
```

A product page must not imply that a domain, repository, or cross-link proves
implementation, adoption, partnership, or production readiness.

## 5. Indexing and release sequence

1. Approve the exact institutional wording and URLs.
2. Validate HTML, canonical links, JSON-LD syntax, and metadata in a staging
   environment.
3. Keep draft or unauthorized pages out of the public sitemap and use
   `noindex` as required by the publication/release gate.
4. Publish `robots.txt` and a sitemap containing only approved, indexable URLs.
5. Verify ownership of the domain in the relevant webmaster console.
6. Request crawling only after release authorization; record the request date
   and URL set in a readiness record.
7. Monitor indexing and structured-data reports for errors, without treating
   impressions, ranking, entity panels, or model responses as guaranteed
   outcomes.

## 6. Verification checklist

- [ ] Canonical description matches the identity record exactly.
- [ ] `@id`, canonical URL, sitemap URL, and Open Graph URL agree.
- [ ] `sameAs` URLs are verified official channels and resolve correctly.
- [ ] No financial, adoption, partner, performance, or readiness claims were
  added.
- [ ] Draft pages are `noindex` and excluded from the sitemap.
- [ ] Released pages have an authorized release decision.
- [ ] JSON-LD passes a syntax/structured-data validator.
- [ ] Changes are recorded in the relevant readiness report.

## Boundary and expected outcome

Structured data and consistent links make the publisher's intended identity
more explicit to consuming systems. They cannot compel Google, other search
engines, or language models to index, rank, merge, or describe Axodus in any
particular way. Incorrect external results should be documented with their
source URL and addressed through the provider's normal correction or feedback
process; no correction outcome is promised by this plan.
