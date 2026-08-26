# Axodus Institutional Taxonomy

Status: Phase 1 controlled institutional taxonomy

## Purpose

This taxonomy is the canonical map for describing Axodus across institutional
documentation. It standardizes entity names, categories, and relationships; it
does not assert that a named component is implemented, integrated, deployed,
validated, adopted, secure, or production-ready.

## Root entity

**Axodus** — a research-driven initiative developing a proposed ecosystem of
interoperable, AI-native organizational platforms for governed knowledge,
institutional workflows, and digital services.

Axodus is currently presented as a conceptual, prototype-stage model. The
root entity is not a financial product, investment fund, exchange, or claim of
commercial operation.

## Canonical categories

### 1. Institutional identity

- `Axodus`: the coordinating research and design identity.
- `Institutional`: the controlled public repository for research, governance,
  disclosure, and publication records.

### 2. Foundation concepts

These are shared architectural and governance concepts, not a claim of a
deployed technical stack:

- central constitutional constraints;
- bounded local governance domains (also called `Tenants` in institutional
  terminology);
- human oversight and accountability;
- evidence, provenance, traceability, review, and appeal;
- interoperable protocols and modular service selection;
- AI assistance for bounded analytical or documentation tasks.

### 3. Intended platform and service nuclei

The following names are author-approved institutional context. Each is a
proposed product or service domain with a bounded conceptual function:

| Nucleus | Conceptual function | Boundary |
|---|---|---|
| ACS | Governed AI-agent and AI-assisted solution layer | No deployed-agent or autonomy claim |
| Business | Proposal-intake and solution-development coordination | No client, contract, or delivery claim |
| Marketplace | Configurable exchange layer for assets, products, and services | No settlement, payment, revenue, or operation claim |
| Academy | Educational and certification layer | No operating education or credential claim |
| BBA-Agency | AI-assisted advertising and creative-workflow service | No client, autonomy, or output-quality claim |
| Governance | Constitutional and ecosystem-governance layer | Conceptual governance only |
| DeFi | Decentralized-finance product and service domain | Separate legal and regulatory review required |
| DEX | Decentralized-exchange domain | No liquidity, listing, contract, or execution claim |
| Trading | AI-assisted automated-trading domain | No strategy, capital, execution, or performance claim |
| Mining | Tokenized-mining service domain | No yield, asset, or operation claim |
| Lottery | Cryptoasset lottery domain | Planning context only; legal review required |

The list is an institutional inventory, not a product catalogue or maturity
assessment. Regulated and financial-domain names require narrower treatment in
any document that discusses them.

### 4. Proposed role labels

`Morpheus`, `Agent Smith`, and `Trinity` are controlled working labels for
proposed constitutional-analysis, adversarial-assurance, and operational-
planning roles. They do not denote deployed autonomous agents or independent
authority.

### 5. Ecosystem lifecycle

The proposed lifecycle for a nucleus is:

`Research → Architecture → Documentation → Prototype → Reference platform → External review → Independent deployment → Federation`

This is a design proposal for organizing future work. It is not evidence that
any nucleus has reached a stage in the sequence.

## Relationship model

```text
Axodus
├── Foundation concepts
├── Intended platform and service nuclei
├── Proposed role labels
└── Institutional records
    ├── Research
    ├── Governance
    ├── Evidence and disclosure
    └── Publications
```

Where a bounded local governance domain selects a nucleus, the selection is a
conceptual relationship subject to constitutional, evidence, risk, review,
and appeal boundaries. It does not imply a customer, tenant deployment,
adoption, or operating community.

## Controlled status vocabulary

Use `conceptual`, `proposed`, `author-reported planned`, or `prototype-stage`
only with the qualifications in the evidence boundaries. Do not map these
labels to L-Level, D-Level, production status, or sensitive-action authority.

## Canonical source and change control

This file is the source of truth for the institutional taxonomy. Changes to
the root description, category membership, or relationship model require an
update to `research/claims-register.md` and review against
`governance/evidence-boundaries.md` and
`governance/public-disclosure-boundary.md`.
