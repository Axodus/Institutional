# Canonical-to-external adaptation flow

Status: E0 control baseline — publication and outreach are not authorized

## Required sequence

```text
Topic selected
  → classify claims and register new claims
  → draft canonical website article
  → evidence review and editorial/identity review
  → human approval of exact canonical version
  → canonical website publication and stable URL recorded
  → adapt for Medium/Substack/GitHub/community as scheduled
  → review each adaptation against the canonical version
  → obtain channel-and-batch human authorization
  → publish externally only after authorization
  → record URL, date, status, and observations
```

The website is the source of truth. External copy is a reviewed adaptation,
not a new source. A summary, excerpt, or thread must retain the canonical link
and the qualifications in the approved article. If the canonical article is
updated or withdrawn, related adaptations are `Blocked` pending review.

## Release gates

| Gate | Required evidence | Passing status |
|---|---|---|
| G0 source | Inventory ID, canonical path, owner | Planned item identified |
| G1 claims | Worksheet rows, claims-register links, limitations | Evidence review complete |
| G2 canonical | Exact version reviewed by named human | Canonical approved |
| G3 adaptation | Diff/check against canonical; links resolve | Adaptation review complete |
| G4 authorization | Human, channel, batch, version, date | Authorized (channel-specific) |
| G5 observation | URL/date/status/observation record | Logged; no causal inference |

No external item may be marked `Ready`, `Authorized`, or `Published` before
G2. `Canonical approved` does not itself authorize any external publication.

## Templates

- [Article template](../../outreach/templates/article-template.md)
- [Thread template](../../outreach/templates/thread-template.md)
- [Claims worksheet](claims-review-worksheet.md)
- [Observation log](observation-log.md)

## Out-of-scope actions

This flow does not authorize account login, profile edits, publication,
comments, submissions, direct messages, paid promotion, or outreach. Missing
access, unclear ownership, or a request to publish is escalated to the human
project owner.
