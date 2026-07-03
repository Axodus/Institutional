---
title: "Axodus: A Prototype-Stage Conceptual Architecture for Governance-Oriented Human-AI Coordination"
author:
  - "Mauricio Z. Filho"
affiliation: "Independent Researcher, Axodus"
correspondence: "[public contact to be added]"
version: "Draft v0.2"
status: "Internal author review required; not ready for publication"
license: "CC BY 4.0"
document_type: "Prototype-stage conceptual architecture and research-agenda paper"
---

# Abstract

Digital institutions increasingly combine governance rules, public records,
automated assistance, and participation requirements, yet the literatures most
relevant to these concerns are often treated separately. Socio-technical
systems work, decentralized-governance research, human–AI oversight guidance,
and credentialing standards each address part of the problem, but they do not
by themselves specify an inspectable institutional model that connects
authority, evidence, participation readiness, and bounded automation. This
paper presents Axodus as a prototype-stage conceptual architecture and
research agenda for that integrative problem. It makes three bounded
contributions: a layered model linking governance, evidence, modular
components, an educational layer, and risk boundaries; a distinction between
documentation maturity and development maturity; and a sequenced evaluation
agenda for traceability, participation readiness, human–AI reliance, and
governance risk. Axodus is described only as a conceptual, prototype-stage
model. The paper reports no deployed system, users, empirical outcomes,
security validation, or token-linked mechanism. An internal Axodus term,
“Proof of Knowledge,” is treated here only as a label for an educational
participation mechanism, not as a cryptographic protocol or financial design.

**Keywords:** socio-technical systems; digital institutions; human–AI
coordination; governance; accountability; decentralized organizations;
educational participation; maturity models

# 1. Introduction

Digital institutions can combine distributed governance, public
documentation, automated assistance, and participation requirements within the
same decision environment. Those capabilities do not by themselves determine
who may decide, what evidence is required, how automation should be bounded,
or how an affected party can challenge a decision. Socio-technical systems
research therefore treats organizational design and technical design as
interdependent rather than assuming that one can be derived from the other
[@baxter2011sociotechnical].

Relevant literatures address these concerns from different directions.
Research on decentralized governance highlights the continuing importance of
interpretation, change, and coordination around self-executing rules
[@hassan2021dao; @hsieh2018bitcoin]. Human–AI interaction guidance emphasizes
expectation setting, correction, and review rather than an undifferentiated
transfer of authority [@amershi2019guidelines]. Credentialing standards help
separate machine verification from institutional judgment
[@w3c2025vcdm]. What remains less clearly specified is an inspectable
institutional model that brings these concerns together without overstating
implementation, legitimacy, or operational maturity.

This paper introduces Axodus as a prototype-stage conceptual architecture and
research agenda for that integrative problem. The project originates from a
multi-year independent research and design effort. The present contribution is
limited to a model: it does not report a functioning platform, production
deployment, users, evaluation results, validated controls, or any token-linked
participation mechanism.

The paper makes three bounded contributions. First, it presents a layered
architecture connecting institutional rules, evidence, modular components, an
educational layer, bounded AI assistance, and risk boundaries. Second, it
separates documentation maturity from development maturity to reduce the risk
that extensive documentation is mistaken for operational readiness. Third, it
defines a sequenced evaluation agenda through which the proposed architecture
could be tested, rejected, or revised.

Several matters are outside the paper's scope. The manuscript does not claim
an implemented system, validated governance outcomes, demonstrated educational
effects, security guarantees, or operational readiness. It also does not
address token minting, token supply, value accrual, incentives, or other
tokenomics questions, which require separate legal, economic, and empirical
review.

# 2. Background and Related Work

## 2.1 Socio-technical and digital institutions

A socio-technical perspective asks how roles, incentives, work practices,
information, and technology jointly shape outcomes. Baxter and Sommerville
argue for integrating organizational concerns with systems engineering rather
than treating them as a late adoption problem
[@baxter2011sociotechnical]. Axodus adopts this perspective by modeling
governance and accountability as architectural elements, not external policy
documents attached after implementation.

The term *digital institution* is used here for an organized system of roles,
rules, records, and technical capabilities through which participants pursue
collective activity. It does not require that every rule be executable or that
every interaction occur on a blockchain.

## 2.2 Decentralized governance and coordination

Hassan and De Filippi describe a DAO as a blockchain-based system in which
people coordinate through decentralized governance and self-executing rules
[@hassan2021dao]. Hsieh et al. distinguish machine consensus from the social
consensus required to alter protocols and organizational arrangements
[@hsieh2018bitcoin]. These distinctions caution against equating technical
distribution with accountable governance.

Research on composable digital infrastructures also shows how dependencies can
propagate across connected components and governance arrangements
[@schar2021defi]. Axodus does not claim to operate any live financial or
asset-linked system. The relevance of this literature here is narrower: it
illustrates how technical composability can intensify governance and
coordination risk when authority and rationale remain unclear.

## 2.3 Human–AI interaction and governance

Guidelines for human–AI interaction emphasize communicating system
capabilities, supporting correction, and learning from behavior over time
[@amershi2019guidelines]. At the organizational level, the NIST AI Risk
Management Framework treats governance, mapping, measurement, and management
as connected risk functions [@tabassi2023airmf]. These sources motivate an
architecture in which AI outputs are attributable inputs to decisions rather
than sovereign decisions.

Constitutional AI uses written principles to guide model behavior through
supervised learning and AI feedback [@bai2022constitutional]. Axodus uses
*constitutional* differently: it refers to institutional rules about
authority, prohibitions, amendments, review, and appeal. The proposed model
does not claim to train or align an AI model through Constitutional AI.

## 2.4 Credentials and participation

The W3C Verifiable Credentials Data Model separates the cryptographic
verification of a credential from validation of whether its claims are fit for
a verifier's purpose [@w3c2025vcdm]. This is central to the educational
component proposed here. A technically verifiable record would not establish
that an assessment is fair, that learning occurred, or that a governance
restriction is legitimate.

# 3. Problem Statement

The architecture addresses a design problem rather than an established
empirical effect:

> How can a modular digital institution connect explicit authority,
> evidence-linked accountability, educational participation, human-supervised
> AI assistance, and risk boundaries without conflating documentation with
> implementation or automation with legitimate governance?

Five tensions structure the problem.

1. **Modularity versus coherence.** Independent components can limit coupling,
   but shared decisions require common identity, evidence, and review rules.
2. **Participation versus readiness.** Open participation may support legitimacy,
   while consequential decisions may require demonstrated understanding.
3. **Automation versus accountability.** AI assistance can reduce analytical
   load, but responsibility can become unclear when its outputs influence
   action.
4. **Transparency versus privacy and security.** Traceable decisions need
   records, while indiscriminate disclosure can harm participants or expose
   systems.
5. **Documentation versus operational truth.** A detailed specification can
   improve review while creating a misleading impression of completion.

Axodus is proposed as one architecture for making these tensions explicit. It
is not presented as their solution.

# 4. Conceptual Architecture

The model comprises six logical layers. They describe responsibilities and
interfaces, not an implementation topology.

## 4.1 Constitutional governance

The governance layer states roles, decision rights, prohibitions, amendment
rules, escalation paths, and appeal mechanisms. Its purpose is to make higher-
order authority visible. A valid action would need both technical
authorization and institutional justification; neither alone would establish
legitimacy.

## 4.2 Evidence and accountability

The evidence layer links proposals, supporting material, declared conflicts,
AI-generated analyses, decisions, responsible roles, and subsequent reviews.
The design objective is reconstructability: a reviewer should be able to ask
what was known, who was authorized, what assistance was used, and why an
outcome followed. The proposal does not assume that more data automatically
produces accountability.

## 4.3 Modular institutional components

Bounded components represent institutional capabilities such as learning,
proposal review, risk analysis, or record keeping. Each component should
declare its purpose, inputs, outputs, authority, dependencies, evidence
requirements, and failure behavior. No definitive inventory or implementation
status is asserted in this draft.

## 4.4 Educational layer and participation

An educational layer and an educational participation mechanism are proposed
as interfaces for learning and assessment. Their purpose would be to help
participants understand domain-specific risks and governance duties before
performing selected consequential actions. They must not become a general
social ranking system.

## 4.5 Human–AI assistance

AI services may support bounded tasks such as document comparison, proposal
summarization, inconsistency detection, risk flagging, and preparation of
review material. Each use should declare the task, source material, output,
uncertainty where available, human reviewer, and disposition. Humans retain
decision authority and responsibility.

## 4.6 Risk and sustainability boundaries

The risk layer expresses constraints on authority, exposure, timing,
conflicts, and escalation. Its purpose is to make consequential decisions
reviewable in relation to defined boundaries rather than to imply a working
control system. This is a design requirement only: the paper claims no
implemented enforcement, security property, or live operational control.

# 5. Modularity and Maturity

Axodus proposes two distinct maturity axes. L0–L5 represents documentation
maturity; D0–D5 represents development maturity. This paper deliberately does
not define the individual levels, assign scores, or report component status.
Those actions require observable criteria and evidence not available in the
current public repository.

The separation is intended to prevent three category errors:

- treating a comprehensive specification as implemented behavior;
- treating an implemented prototype as validated institutional performance;
- averaging unlike forms of maturity into one reassuring score.

A future maturity specification should define required artifacts, admissible
evidence, reviewers, expiration rules, and disagreement handling for every
level. Inter-rater reliability and resistance to self-assessment inflation
should be evaluated before the axes are used in public reporting.

Modularity is similarly a hypothesis rather than an assured property.
Component boundaries may support bounded change and review, but they can also
move complexity into interfaces. Evaluation must therefore examine dependency
visibility, cross-component failure, and governance consistency.

# 6. Educational Participation and Governance Readiness

**Terminology note.** Axodus notes use the internal label *Proof of Knowledge*
for the educational participation mechanism discussed here. In this paper, the
mechanism is described in functional terms to avoid confusion with
cryptographic proof-of-knowledge protocols, proof-of-work, proof-of-stake, or
token-linked participation schemes.

The mechanism would connect a defined learning objective, an assessment, a
reviewable result, and eligibility for a bounded activity. A possible flow is:

1. publish the knowledge and risk objectives for an activity;
2. provide accessible learning paths;
3. assess understanding using methods appropriate to the objective;
4. issue a time-bounded result with an appeal path;
5. apply the result only to the specified activity;
6. reassess validity, disparate effects, and continued necessity.

The W3C credential model could inform portable representations, but
verification of an issuer and credential does not validate educational quality
or justify authorization [@w3c2025vcdm]. The governance problem therefore
includes who defines curricula, who assesses assessors, how accommodations are
provided, and how a participant can contest an outcome.

The central hypothesis is that knowledge-gated participation may improve the
quality of participation in selected high-consequence contexts. Competing
hypotheses are equally important: the mechanism may reduce participation,
favor already advantaged groups, encourage test gaming, centralize curriculum
power, or create privacy risks. The mechanism should be rejected or redesigned
if those harms cannot be controlled.

# 7. Governance, Accountability, and Human Oversight

The proposed decision record has seven conceptual fields: decision scope,
authorized roles, evidence considered, conflicts disclosed, automated
assistance used, decision and rationale, and review or appeal path. This is a
minimum accountability model, not a database schema.

AI assistance is governed by task-specific boundaries. Low-consequence
drafting may permit lightweight review; risk classification or proposal
analysis would require stronger provenance, independent checking, and explicit
human disposition. An AI output cannot approve its own use, resolve an appeal
about itself, or become the final bearer of responsibility.

The model should support contestability. Participants affected by a decision
need a way to identify applicable rules, challenge evidence, correct records,
and request review by an appropriately independent role. Immutable records,
where used, must not be treated as immutable interpretations.

These requirements align with risk-oriented governance and human–AI
interaction guidance [@tabassi2023airmf; @amershi2019guidelines], but their
effectiveness in Axodus remains untested.

# 8. Risk Boundaries

Risk boundaries are proposed at four levels:

- **action boundaries:** what an actor or agent may do;
- **exposure boundaries:** resources or values that may be placed at risk;
- **process boundaries:** evidence, approvals, waiting periods, and conflicts;
- **escalation boundaries:** conditions requiring suspension or review.

Visible transactions or records do not by themselves make assumptions,
conflicts, and rationales inspectable. Research on composable digital
infrastructures likewise shows that dependencies can propagate across connected
components [@schar2021defi]. The proposed model therefore treats decision
context as part of risk governance rather than as a by-product of technical
execution.

Questions about live asset policies, token-linked participation, supply
mechanisms, or financial incentives are outside the scope of this paper.
Before any such design were documented publicly, it would require separate
legal, economic, and empirical review in addition to threat modeling and
simulation.

# 9. Prototype Status

Axodus is presented in this paper as a conceptual, prototype-stage model. The
public repository presently supports editorial artifacts and research
documentation. It does not supply evidence of an integrated implementation,
production operation, user adoption, empirical performance, or effective
controls.

The absence of those claims is substantive. Architectural consistency can be
reviewed before implementation, but it cannot substitute for observed
behavior. Future versions should maintain a component-by-component evidence
table distinguishing designed, prototyped, tested, deployed, and independently
evaluated states.

# 10. Evaluation Plan

The architecture yields five initial research questions.

**RQ1 — Traceability:** Does the proposed evidence model help independent
reviewers reconstruct decisions more accurately and efficiently than a
document-only baseline? A study could use matched governance scenarios,
blinded reviewers, reconstruction accuracy, time, disagreement, and missing-
evidence detection.

**RQ2 — Educational participation:** Does a knowledge-gated participation
mechanism improve
domain-relevant understanding without unacceptable exclusion? A staged study
should measure learning, retention, decision reasoning, completion,
accessibility, subgroup effects, appeals, and test gaming. Token-linked or
financial stakes should not be introduced in an initial study.

**RQ3 — Human–AI reliance:** For bounded proposal-analysis tasks, how do
provenance and mandatory human disposition affect error detection, calibrated
reliance, override behavior, and review quality? Experiments should include
planted AI errors and ambiguous cases.

**RQ4 — Maturity reliability:** Can independent reviewers apply future L and D
criteria consistently from the same evidence? Evaluation should measure
inter-rater agreement, reasons for disagreement, and susceptibility to
strategic self-rating.

**RQ5 — Risk governance:** Do explicit action, exposure, process, and
escalation boundaries reduce unauthorized or poorly evidenced decisions in
tabletop simulations? Scenarios should include conflicts of interest, urgent
actions, incomplete evidence, agent error, and cross-component failure.

The sequence should move from document inspection to tabletop simulation,
non-financial prototypes, controlled user studies, and only then bounded field
pilots. Each stage needs preregistered success and stop criteria appropriate to
its risk.

# 11. Limitations and Threats to Validity

This paper is broad and conceptual. It may combine concerns that require
separate theories, methods, and papers. The architecture can appear coherent
because it has not yet encountered implementation constraints or institutional
conflict.

The public evidence base for Axodus is currently limited to design
documentation. There are no results with which to assess feasibility,
usability, governance legitimacy, security, or social impact. The model is
also authored from a single-project perspective and may encode unexamined
assumptions about authority, education, and accountability.

Knowledge-gated participation presents particular risks of exclusion, surveillance,
curriculum capture, and false confidence. Human oversight can become nominal
when reviewers lack time or expertise. Audit trails can create privacy and
security harms. Modularity can hide systemic coupling. Explicit rules can
formalize unjust arrangements rather than correct them.

Web3-facing governance designs may also encounter regulatory uncertainty,
operational fragility, and jurisdiction-specific compliance burdens. AI
assistance may be unreliable, difficult to calibrate, or difficult to audit
under realistic workload and time pressure.

The paper does not provide legal, financial, security, or investment advice.
Its terminology may not map cleanly onto every jurisdiction or research
community.

# 12. Research Agenda

Near-term work should:

1. formalize observable L and D maturity criteria;
2. specify the minimal decision and evidence model;
3. design a non-financial educational participation prototype with
   accessibility and appeal requirements;
4. define bounded AI-assistance tasks and provenance records;
5. create governance and failure scenarios for tabletop evaluation;
6. recruit independent reviewers from governance, HCI, education, security,
   and decentralized-systems backgrounds;
7. publish negative findings and design changes alongside positive results.

Separate papers or technical notes should address educational validity,
human–AI governance, and any token-linked or financial design questions rather
than treating the present architecture paper as evidence in those domains.

# 13. Conclusion

Axodus is proposed as a conceptual architecture for connecting governance,
evidence, modular institutional components, educational participation,
human-supervised AI assistance, and risk boundaries. Its immediate value is
not demonstrated performance but inspectability: the model exposes claims,
interfaces, tensions, and evaluation questions before operational maturity is
asserted.

The architecture will become a credible contribution only if its constructs
are specified, independently criticized, implemented in bounded prototypes,
and evaluated against alternatives. This draft establishes a research agenda
for that process. It is ready for human review, not for public publication.

# References

References are maintained in `references.bib`. All entries cited in this draft
have corresponding verification records in
`../../research/bibliography-verified.md`.
