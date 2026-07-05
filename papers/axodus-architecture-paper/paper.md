---
title: "Axodus: A Prototype-Stage Conceptual Architecture for Traceability and Accountability in Federated Modular Digital Institutions"
author:
  - "Mauricio Z. Filho"
affiliation: "Independent Researcher, Axodus"
correspondence: "mzfshark@gmail.com"
project_discussion_forum: "Telegram @thinkincoin"
author_social_handle: "@mzfshark"
version: "Draft v0.4"
status: "Ready for author review of internal v0.4 draft; not ready for peer review, external circulation, or publication"
license: "CC BY 4.0"
document_type: "Prototype-stage conceptual architecture and focused research-agenda paper"
---

# Abstract

Human-AI-assisted digital institutions become difficult to govern when
constitutional constraints, bounded local governance domains, modular
capabilities, and review obligations must be coordinated within the same
decision environment. Existing literatures on socio-technical systems,
decentralized governance, provenance, accountable algorithms, contestability,
and human-AI interaction clarify parts of this problem, but they do not by
themselves provide a compact conceptual architecture for traceability,
accountability, contestability, and reconstructability across
constitutionally constrained modular institutions. This paper presents Axodus
as a prototype-stage conceptual architecture for that setting. Its central
contribution is a six-layer governance-oriented model relating a
constitutional center, bounded local governance domains, modular
institutional capabilities, evidence and provenance, bounded AI assistance,
and risk or contestability controls. Participation readiness and internal
maturity distinctions are treated as supporting mechanisms rather than
co-equal contributions. Axodus is described only as a conceptual,
prototype-stage model; the paper reports no deployment, empirical validation,
observed institutional use, or operational readiness.

**Keywords:** socio-technical systems; federated digital institutions;
human-AI coordination; traceability; accountability; governance;
contestability

# 1. Introduction

Digital institutions increasingly combine distributed authority, modular
capabilities, public records, and automated assistance. Governance becomes
harder when these elements must remain reviewable across a constitutional
center and bounded local governance domains rather than inside a single
authority chain. In that setting, the institutional challenge is not only
whether a decision can be documented, but whether later reviewers can
reconstruct which authority applied, which bounded capability was invoked,
what evidence was considered, how AI assistance shaped the record, and how
correction, challenge, or appeal could proceed. Socio-technical systems
research treats those questions as jointly organizational and technical rather
than reducible to one domain alone [@baxter2011sociotechnical].

Relevant literatures address parts of this problem without yet yielding a
single architecture for accountable governance across constitutionally
constrained modular ecosystems. Research on decentralized governance shows
that self-executing rules do not remove interpretation, amendment, or social
coordination [@hassan2021dao; @hsieh2018bitcoin]. Human-AI interaction
guidance emphasizes review, correction, and expectation setting rather than an
undifferentiated transfer of authority [@amershi2019guidelines]. Provenance
and credentialing standards help distinguish evidence lineage and machine
verification from institutional judgment [@w3c2013provdm; @w3c2025vcdm]. Yet
those literatures do not by themselves provide a compact architecture for
traceability, accountability, contestability, and reconstructability in
constitutionally constrained, modular, human-AI-assisted institutions.

This paper addresses that gap by introducing Axodus as a prototype-stage
conceptual architecture for human-AI-assisted digital institutions under
bounded governance constraints. The project originates from a multi-year
independent research and design effort. The present contribution remains
conceptual: it does not report a platform in real institutional use, a
functioning institutional environment, evaluation results, or independently
tested controls.

The contribution is architecture-level design reasoning rather than an
implementation claim. The paper proposes a layered model for how a
constitutional center, bounded local governance domains, modular
institutional capabilities, evidence packages, attributable AI assistance,
and review paths may be arranged into one inspectable decision structure.
Participation readiness, internal maturity distinctions, and risk boundaries
remain supporting components that frame how this structure might later be
evaluated, narrowed, or rejected.

Implementation, deployment, institutional use, and empirical validation are
outside the paper's scope. The manuscript also excludes token design,
financial operations, educational-distribution mechanics, security
guarantees, and legal conclusions.

# 2. Background and Related Work

## 2.1 Socio-technical systems and federated digital institutions

A socio-technical perspective asks how roles, incentives, work practices,
information, and technical components jointly shape outcomes. Baxter and
Sommerville argue for integrating organizational concerns with systems
engineering rather than treating them as a late adoption problem
[@baxter2011sociotechnical]. Axodus adopts this perspective by modeling
governance, accountability, and review as architectural elements rather than
external policies attached after implementation.

The term *federated modular digital institution* is used here for an organized
system in which a central constitutional layer defines shared constraints,
while bounded local governance domains may configure modular institutional
capabilities. This use is conceptual. It does not imply a deployed federation,
legal federal status, or operating multi-tenant platform.

## 2.2 Decentralized governance, modular coupling, and review

Hassan and De Filippi describe a DAO as a blockchain-based system in which
people coordinate through decentralized governance and self-executing rules
[@hassan2021dao]. Hsieh et al. distinguish machine consensus from the social
consensus required to alter protocols and organizational arrangements
[@hsieh2018bitcoin]. These distinctions caution against equating technical
distribution with accountable governance.

Smart-contract-based financial markets provide one domain-specific example in
which composability can propagate dependencies across connected protocols
[@schar2021defi]. Systems-theoretic safety research instead offers the broader
claim needed here: failures in complex socio-technical systems can arise from
interactions, control mismatches, and poorly governed coupling rather than
from isolated component defects alone [@leveson2012engineering]. The present
paper therefore treats that domain only as one motivating example of
dependency propagation, not as the paper's institutional center.

## 2.3 Human-AI oversight and accountable decision support

Guidelines for human-AI interaction emphasize communicating system
capabilities, supporting correction, and learning from behavior over time
[@amershi2019guidelines]. At the organizational level, the NIST AI Risk
Management Framework treats governance, mapping, measurement, and management
as connected risk functions [@tabassi2023airmf]. These sources motivate an
architecture in which AI outputs remain attributable, reviewable inputs to
human decisions rather than sovereign decisions in themselves.

Constitutional AI uses written principles to guide model behavior through
supervised learning and AI feedback [@bai2022constitutional]. Axodus uses
*constitutional* differently: it refers to institutional rules about
authority, prohibitions, amendments, review, and appeal. The proposed model
does not claim to train or align an AI model through Constitutional AI.

## 2.4 Provenance, credentials, and institutional judgment

The W3C PROV Data Model describes provenance through entities, activities,
agents, derivations, attribution, and responsibility relationships
[@w3c2013provdm]. This vocabulary is useful for distinguishing source
artifacts, transformations, automated assistance, and responsible roles in a
decision record. It supports reconstruction of how an output was produced, but
does not by itself establish that the decision was legitimate, contestable, or
accountable.

The W3C Verifiable Credentials Data Model separates cryptographic
verification from validation of whether a credential's claims are fit for a
verifier's purpose [@w3c2025vcdm]. This matters here because machine-verifiable
eligibility artifacts would not by themselves establish fair assessment,
legitimate authorization, or accountable participation boundaries.

Work on accountable algorithms likewise argues that automated decision
processes must be assessable against external legal or policy standards and
that transparency alone is insufficient [@kroll2017accountable]. Provenance is
therefore one input to accountability, not its substitute.

## 2.5 Contestability and reviewable governance

Contestability-by-design literature identifies safeguards, human review and
intervention, and third-party scrutiny as design features for challenge and
correction [@alfrink2023contestable]. This framing is directly relevant to
federated modular governance because a traceable record remains insufficient
if a person affected by a decision cannot identify the applicable rule,
challenge evidence, or reach an appropriately independent reviewer.

# 3. Problem Statement

The architecture addresses a design problem rather than an established
empirical effect:

> How can a constitutionally constrained federated modular digital institution
> preserve traceability, accountability, contestability, and
> reconstructability when bounded local governance domains configure modular
> institutional capabilities through human-AI-assisted decision processes?

Five tensions structure the problem.

1. **Central constraints versus local autonomy.** A constitutional layer may
   preserve coherence, while bounded local governance domains still require
   meaningful discretion over local decisions and configurations.
2. **Modular capabilities versus governability.** Service separation may
   limit direct coupling, while modular selection can create hidden dependency
   chains, ambiguous authority, and fragmented review paths.
3. **Automation versus accountable disposition.** AI assistance can reduce
   analytical load, but responsibility can become unclear when its outputs
   influence authorization, escalation, or review.
4. **Participation versus bounded readiness.** Open participation may support
   legitimacy, while consequential governance actions may require reviewable
   preparation, accommodations, and appeal.
5. **Documentation versus institutional reality.** A detailed specification
   can improve inspection while also creating a misleading impression of
   implementation completeness or legitimate authority.

Axodus is proposed as one architecture for making these tensions inspectable
and reviewable. It is not presented as a complete or empirically tested
solution.

# 4. Conceptual Architecture

The model comprises six logical layers. They are presented as conceptual
design surfaces for allocating authority, structuring records, and preserving
reviewability, not as an implementation topology.

Information and control move through the architecture in different ways.
Control begins with constitutional constraints that define what local
decisions, capability selections, and escalation paths are in scope. Evidence
packages, provenance records, advisory analysis, rationale, and review
records then make those decisions reconstructable for later review. Risk
boundaries constrain permissible state transitions, while contestability
paths preserve challenge, correction, escalation, and appeal.

**Illustrative synthetic scenario - bounded-governance exception review.** A
mock bounded local governance domain requests a temporary exception affecting
one modular institutional capability. The request includes the applicable
constitutional rule, local authority basis, declared conflicts, and a
controlled evidence package. A simulated AI review flags one conflict but
omits a dependency between the requested configuration and a review
requirement. The designated human reviewer withholds disposition, records the
omission, and escalates the matter because a risk boundary is triggered. An
independent appeal role can then reconstruct which constitutional constraint
applied, what local choice was proposed, what the simulated AI review
changed, and why escalation occurred. This scenario is an analytical
illustration, not evidence of an Axodus implementation or institutional
process.

1. constitutional governance defines the applicable roles, decision rights,
   prohibitions, amendment rules, and appeal conditions;
2. bounded local governance domains interpret that scope for a local decision
   context and may propose a configuration or exception within constitutional
   limits;
3. modular institutional capabilities express what is being selected,
   reviewed, or changed;
4. the evidence and provenance layer links source materials, authority
   statements, conflicts, transformations, and responsible roles;
5. human-AI assistance may analyze that material, but only as attributable
   advisory input to human disposition; and
6. risk-boundary and contestability controls keep challenge, correction,
   escalation, and appeal available.

## 4.1 Constitutional governance layer

The constitutional governance layer is a conceptual constraint surface that
defines higher-order rules: roles, decision rights, prohibitions, amendment
procedures, escalation paths, and appeal conditions. Its purpose is to make
non-delegable institutional constraints visible before local configuration
begins and to frame how later review can distinguish a permitted action from
an out-of-scope one.

In this proposal, the layer structures accountability boundaries rather than
serving as a deployed constitution, legal instrument, active authority, or
enforcement body. A reviewable action therefore depends on both institutional
justification and whatever technical authorization a future implementation
might use; neither alone would establish legitimacy.

## 4.2 Bounded local governance domain layer

The bounded local governance domain layer represents a locally scoped decision
context operating under constitutional constraints. A bounded local
governance domain may configure local processes, select functional service
modules, and allocate decision tasks only within the scope permitted by the
constitutional layer. Axodus institutional documentation may use the term
Tenant for such bounded local governance domains; this paper uses the
governance-domain phrasing to avoid implying deployed SaaS tenancy, active
customer entities, operating communities, or production infrastructure.

## 4.3 Functional service module layer

Functional service modules are abstract bounded institutional capabilities
through which selected functions can be configured, limited, and governed.
The paper does not present a product catalog. Instead, it treats a functional
service module as a conceptual unit that should declare its purpose, inputs,
outputs, delegated authority, evidence requirements, dependencies,
escalation conditions, and failure behavior.

Axodus institutional documentation may use the term service nuclei in broader
institutional contexts; this paper uses functional service modules as the
architecture-facing abstraction to avoid implying a product catalog,
implementation inventory, or deployed system decomposition.

A minimal functional taxonomy includes authority and role registries, evidence
registries, decision-rationale records, conflict and disclosure registers,
review and appeal paths, risk-boundary controllers, and participation-
readiness support. These are component types rather than claims about a
definitive Axodus module inventory or implementation state.

## 4.4 Evidence and provenance layer

The evidence and provenance layer links proposals, supporting materials,
authority statements, declared conflicts, AI-generated analyses, decisions,
and subsequent reviews. Its design objective is reconstructability: a reviewer
should be able to ask what was known, who was authorized, what configuration
was proposed, what assistance was used, and why an outcome followed.

At the conceptual level, source documents and outputs can be treated as
entities, analysis and review steps as activities, and human or automated
participants as agents. Derivation and attribution relations can then connect
an output to its inputs and responsible roles [@w3c2013provdm]. These concepts
specify what a reviewable record should express so that a later reviewer can
reconstruct the path from source material to disposition. They do not by
themselves prove that a record is true, complete, tamper-resistant, or
accountable in the stronger normative sense.

Accordingly, the layer supports later inspection rather than automatic
validation. It does not prescribe a storage system, cryptographic proof,
implemented evidence infrastructure, or integrity guarantee, and it does not
convert record linkage into a full judgment about whether the decision was
substantively justified.

## 4.5 AI-assistance layer

AI assistance remains advisory. It may support bounded tasks such as document
comparison, proposal summarization, inconsistency detection, constitutional
analysis support, adversarial checking, and planning-oriented review support.
Each use should declare the task, source material, output, uncertainty where
available, human reviewer, and disposition so that later reviewers can inspect
how advisory analysis entered the record. Humans retain decision authority and
responsibility.

This layer is intentionally role-abstract. The paper does not use named agent
labels, does not claim autonomous execution authority, and does not claim that
AI assistance itself enforces governance, issues binding judgments, or
replaces human institutional review.

## 4.6 Risk-boundary and contestability layer

The risk-boundary and contestability layer is a conceptual surface for making
it visible when further review, refusal, documentation, or a challenge path
may be needed. In this model, a boundary should identify the relevant role,
the review trigger, the evidence required for inspection, and the condition
under which a proposed action exceeds its permitted scope. Contestability
therefore concerns whether a decision can be reconstructed, questioned, and
re-examined in principle, not whether the architecture already operates a
standing challenge mechanism.

Within that framing, reviewer independence is a design concern rather than a
claim about a standing body or named role. The architecture should make it
possible to distinguish the original decision context from later challenge or
re-examination conditions, including disclosed conflicts and situations in
which the same actor should not be the sole judge of a contested record.
Human oversight becomes nominal when a reviewer lacks the time, authority
context, evidence access, or practical capacity to change an outcome
[@tabassi2023airmf; @amershi2019guidelines]. Contestability-by-design
literature is relevant here because it treats review visibility,
intervention, and external scrutiny as design requirements for challengeable
systems rather than as guarantees that harmful outcomes are prevented
[@alfrink2023contestable].

# 5. Participation Readiness as a Supporting Mechanism

A participation-readiness mechanism is proposed only as a supporting
institutional interface for bounded preparation, assessment, accommodations,
and challenge conditions in selected consequential contexts. It is not the
paper's central contribution and must not be treated as a standalone
educational product or a general social ranking system.

In this proposal, any readiness artifact functions only as a reviewable input
to a broader decision context. It does not by itself establish legitimacy,
fairness, or authority. The governance problem therefore includes who defines
the criteria, how accommodations are provided, whether the requirement is
proportionate to the decision context, and how a participant can challenge an
outcome.

The working hypothesis is that bounded preparation may improve participation
quality in selected high-consequence contexts. Competing hypotheses remain
equally important: the mechanism may exclude participants, centralize
interpretive power, encourage test gaming, or create privacy risks. It should
be narrowed, redesigned, or rejected if those harms cannot be controlled.

# 6. Internal Maturity Distinction and Scope Reduction

The Axodus internal governance process distinguishes two orthogonal maturity
dimensions. **L-Level** refers to organizational, documentation, governance,
and authority maturity. **D-Level** refers to development, implementation,
technical validation, and operational maturity. L-Level does not measure code,
and D-Level does not measure governance. Neither dimension authorizes
production or sensitive action; production status and action authority require
separate gates.

The taxonomy is relevant here only as a guard against category error. It helps
prevent documentation from being mistaken for implementation, local
implementation from being mistaken for production, or maturity from being
mistaken for authority. The paper does not assign maturity levels to
components and does not present the taxonomy as a validated measurement
instrument.

Scope reduction is therefore a design requirement rather than a late-stage
optimization. Initial prototypes should start with decisions for which
reconstruction and appeal are materially important, use a minimum sufficient
decision-and-evidence record, separate advisory AI outputs from authoritative
human dispositions, and remove components that do not improve reconstructability
or contestability.

# 7. Prototype Status

Axodus is presented in this paper as a conceptual, prototype-stage model. The
public repository presently supports editorial artifacts, governance records,
and research documentation. It does not supply evidence of an integrated
implementation, functioning federated platform, production operation, user
adoption, empirical performance, or effective controls.

The absence of those claims is substantive. Architectural consistency can be
reviewed before implementation, but it cannot substitute for observed
behavior. Future versions should maintain a component-by-component evidence
table distinguishing designed, prototyped, tested, deployed, and independently
evaluated states.

# 8. Evaluation Plan

The evaluation program is intentionally prioritized rather than broad.

Before either initial study, the first study stage would require a controlled
environment rather than any active institutional setting. That environment
could combine synthetic bounded-local-governance scenarios, controlled
evidence packages, simulated AI-assistance records, planted errors, and a
high-fidelity mock-up or wizard-of-oz review interface. A preregistered
protocol would define reviewer tasks and illustrative study criteria. These
criteria are proposed study designs, not reported results.

**Primary initial study — RQ1: Traceability and reconstruction.** Does the
proposed evidence model help independent reviewers reconstruct bounded local
governance decisions involving functional service modules more accurately and
efficiently than a document-only baseline? The controlled environment would
support matched governance scenarios and blinded review. Illustrative study
criteria could include reconstruction completeness, authority-conflict
detection, missing-evidence detection, time to reconstruct rationale,
provenance error detection, reviewer disagreement, and correct classification
of whether a challenge path can proceed. This is the paper's primary
evaluation priority because it most directly tests the central claim about
traceability and accountability in federated modular governance.

**Secondary initial study — RQ3: Human-AI reliance in advisory review.** For
bounded proposal-analysis tasks, how do provenance and mandatory human
disposition affect error detection, calibrated reliance, override behavior,
and review quality? The simulated AI records would include planted errors,
ambiguous cases, and contested recommendations. Illustrative study criteria
could include planted-error detection, unsupported-output detection, override
or acceptance behavior by condition, rationale quality, reviewer
disagreement, and correction after provenance information is shown. This is a
secondary priority because the architecture depends on bounded AI assistance
being reviewable rather than merely available.

**Staged future evaluation.** Evaluation should progress from controlled
artifact inspection to bounded reviewer studies using synthetic scenarios,
then to controlled prototype evaluation under a separately approved protocol.
Any later institutionally situated study would require additional governance,
ethics, legal, privacy, and evidence gates. Participation readiness,
maturity reliability, and broader institutional-governance questions remain
later research topics.

# 9. Limitations and Threats to Validity

This paper is conceptual and still broader than a mature external article
would ideally be. The architecture can appear coherent because it has not yet
encountered implementation constraints, institutional conflict, workload
pressure, or field conditions that would test whether its proposed review
paths are workable across constitutional decisions and decisions within
bounded local governance domains.

The public evidence base for Axodus is currently limited to design
documentation. There are no results with which to assess feasibility,
usability, governance legitimacy, calibrated reliance, contestable challenge
paths, or social impact. The paper reports no field validation, no
institutionally situated validation, no production use, no token-design or
token-distribution claims, no claims about financial operation, no security
guarantees, and no legal or regulatory conclusion.

Human oversight can become nominal when reviewers lack time, authority,
evidence access, or practical power to change the outcome. AI assistance may
be unreliable, difficult to calibrate, or difficult to audit under realistic
workload and time pressure. Weak contestability or poorly designed challenge
paths could make traceability visible without making accountability
meaningful.

Participation-readiness mechanisms present particular risks of exclusion,
surveillance, curriculum capture, and false confidence. Modular separation can
also hide systemic coupling, while constitutional constraints can be overly
rigid or too ambiguous for effective local governance. The proposed
architecture may be too complex to govern in practice without substantial
scope reduction.

The synthetic scenario is explanatory rather than empirical. Provenance
vocabulary does not establish record integrity or accountability, and the
proposed measures do not demonstrate performance. Institutionally situated
evaluation may also expose conflicts, incentives, and workload effects that a
controlled artifact cannot reproduce.

The paper does not provide financial, security, investment, or legal advice.
Its terminology may not map cleanly onto every jurisdiction or research
community.

# 10. Research Agenda

Near-term work should prioritize a minimal decision-and-evidence model,
synthetic scenarios involving bounded local governance domains, and bounded
AI-assistance tasks suitable for initial traceability and reliance studies.
Additional literature hardening around governance quality, reviewer
independence, empirical institutional challenge paths, and participation-
readiness validity remains a later requirement before any broader external
review is considered.

# 11. Conclusion

Axodus is proposed as a prototype-stage conceptual architecture for making
human-AI-assisted governance more traceable and accountable in federated
modular digital institutions. Its contribution is not a product catalog or
implementation-status claim, but an inspectable arrangement linking
constitutional constraints, bounded local governance domains, functional
service modules, evidence and provenance, advisory AI assistance, and review
paths.

The next research step is to instantiate the minimum decision-and-evidence
model in a controlled experimental environment and test whether independent
reviewers can reconstruct and challenge decisions within bounded local
governance domains under the proposed record structure.

# References

References are maintained in `references.bib`. All entries cited in this draft
have corresponding internal verification records in
`../../research/bibliography-verified.md`; final metadata rechecking is
required before any submission, public release, or external circulation.
