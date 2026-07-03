# Axodus Internal Maturity Taxonomy

Status: Internal operational taxonomy; not an empirically validated
measurement instrument

## Purpose and boundaries

Axodus uses two orthogonal maturity dimensions:

- **L-Level** describes organizational, documentation, governance, and
  authority maturity.
- **D-Level** describes development, implementation, technical validation,
  and operational maturity.

L-Level does not measure code. D-Level does not measure governance. Neither
dimension automatically authorizes production or sensitive action.

The taxonomy is an internal rubric for separating evidence categories and
avoiding false equivalence between documentation, implementation, production,
and authority. It is not a scientific scale, does not establish interval
measurement, and has not been empirically validated for reliability.

## Rule of separation

The governing distinction is:

```text
L measures whether a unit is governable.
D measures whether a unit is implemented.
Production status determines whether it may operate in a real environment.
Authority status determines whether it may perform sensitive actions.
```

Production and authority are independent gates. A high L-Level or D-Level is
necessary evidence in some contexts but is never sufficient authorization.

## L-Level: Organizational and governance maturity

### L0 — Idea

The unit exists only as an intention, hypothesis, or initial concept.

Typical criteria:

- informally described idea;
- no clear operational scope;
- no structured documentation;
- no roadmap;
- no formal blocker record;
- no ownership;
- no validation.

### L1 — Defined scope

The unit has an initial purpose, scope, and general boundaries.

Typical criteria:

- defined mission;
- documented initial scope;
- known principal risks;
- initial boundaries recorded;
- incomplete operational structure;
- no robust local validation.

### L2 — Created structure

The unit has an initial operational and documentary structure.

Typical criteria:

- workspace or repository structure;
- initial instruction file;
- initial status, roadmap, or task records;
- initial folder or application structure;
- basic blockers recorded;
- insufficient evidence for L3 candidacy.

### L3 — Candidate for local validation

The unit has initial evidence of locally reviewable organization or behavior.

Typical criteria:

- materially developed instructions;
- known local scripts;
- executable or documented build, test, lint, or type-check procedure where
  applicable;
- initial handoff record;
- blockers recorded;
- initial risk and security mapping;
- not ready for L4 consolidation.

### L4 Candidate — Candidate for consolidation

The unit has enough structure and evidence to begin a consolidation cycle.

Typical criteria:

- consistent operational documentation;
- coherent roadmap and task records;
- explicit blockers;
- existing local validation;
- known boundaries;
- sufficient maturity for a consolidation epic;
- consolidation not yet completed.

### L4 Readiness — Ready for controlled integration

The unit has enough organizational maturity for controlled, read-only, or
gated integration.

Typical criteria:

- clear boundaries;
- reasonably defined ownership;
- tracked blockers;
- relevant local validation;
- planned or existing integration contracts or interfaces;
- readiness for controlled consumption;
- final consolidation may remain incomplete.

### L4 Consolidated — Consolidated and governable

The unit has sufficiently stable governance, documentation, validation,
blockers, boundaries, and evidence to be treated as a governable portfolio
unit.

Typical criteria:

- complete and current instruction file;
- coherent status, roadmap, blockers, security, validation, and handoff
  records;
- recorded validation evidence;
- completed delivery-reality review;
- preserved boundaries;
- known and tracked risks;
- defined integration or readiness posture;
- no critical authority ambiguity.

L4 Consolidated does not mean production, execution, or financial authority.

### L5 — Contractual, auditable, or foundational

The unit has a foundational, contractual, normative, or auditable role in the
ecosystem.

Typical criteria:

- central conceptual or architectural authority;
- strong documentation;
- cross-cutting ecosystem role;
- high traceability;
- elevated audit or compliance requirements;
- continued gating where required;
- no automatic production status.

L5 may remain non-production, on hold, or blocked from execution.

## D-Level: Development and implementation maturity

### D0 — Concept only

No functional implementation exists.

Typical criteria:

- no functional code;
- no application or service;
- no tests;
- no scripts;
- conceptual documentation only.

### D1 — Technical foundation

An initial technical structure exists with limited functionality.

Typical criteria:

- initial project or application;
- folder structure;
- basic dependencies;
- initial types or schemas;
- basic scripts;
- no material functional flow.

### D2 — Local or mock functionality

Basic local, mock, or configuration-first functionality exists.

Typical criteria:

- fixtures or mock data;
- schemas;
- simple local services;
- initial components;
- basic tests;
- partial local flow;
- no significant integration.

### D3 — Significant integrated or read-only functionality

More substantial local functionality exists with read-only integration,
consumption contracts, or meaningful non-production flows.

Typical criteria:

- functional services or read models;
- read-only contracts;
- useful dashboards or pages where applicable;
- relevant tests;
- mock or configuration-first integration with other units;
- read-only APIs where applicable;
- consistent local validation.

### D3+ — Strong D3, not yet D4

The unit exceeds a basic D3 profile but lacks the breadth or controlled
execution evidence required for D4.

Typical criteria:

- broad test suite;
- passing end-to-end tests where applicable;
- multiple services or read models;
- consistent preview flows;
- boundary enforcement;
- relevant local integration;
- insufficient breadth for D4.

### D4 — Extensive controlled mock or non-production product

A broad local, mock, or configuration-first product exists without real
production operation.

Typical criteria:

- broad functional product;
- multiple pages or routes where applicable;
- substantial services, hooks, or components;
- broad tests;
- preview-only or controlled mock flows;
- advanced non-production integration;
- preserved production boundaries.

D4 does not mean production or real financial execution.

### D5 — Real production operation

The unit operates in a real production environment.

Typical criteria:

- active production operation;
- real users and data;
- production credentials and integrations;
- real execution;
- production monitoring;
- incident response;
- operational compliance;
- audited security where required;
- explicitly approved authority.

D5 may be assigned only through an explicit, audited decision supported by
production evidence. This definition does not assert that any Axodus unit has
reached D5.

## Interpretation examples

`L4 Consolidated / D3+ / NON_PRODUCTION` means that a unit is governable and
substantially implemented in a local or controlled environment, but is not
authorized for production or real-world execution.

`L5 / D3 / HOLD` means that a unit has a foundational role and partial
implementation while execution remains blocked.

These examples explain status composition; they do not assign a status to any
actual Axodus unit.

## Use in publications

The full rubric belongs in internal governance documentation. A manuscript may
describe the distinction between L-Level and D-Level when needed to prevent
category errors, but must identify the rubric as an internal operational
taxonomy rather than an empirically validated measurement instrument.

Public-facing text must not publish component scores, infer production
readiness, or infer sensitive authority from either dimension without a
separate evidence and approval process.
