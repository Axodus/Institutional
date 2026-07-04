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

Federated digital institutions can combine central constitutional rules, local
governance domains, modular service selection, and human-AI-assisted decision
support within the same institutional environment. Existing literatures on
socio-technical systems, decentralized governance, provenance, accountable
algorithms, contestability, and human-AI interaction clarify parts of this
problem, but they do not by themselves yield a focused conceptual architecture
for traceability and accountability across constitutionally constrained
federated modular ecosystems. This paper presents Axodus as a prototype-stage
conceptual architecture for that setting. Its central contribution is a six-
layer model linking constitutional governance, Tenant governance, service
nuclei, evidence and provenance, bounded AI assistance, and risk or
contestability controls. Participation readiness and internal maturity
distinctions are treated as supporting mechanisms rather than co-equal
contributions. Axodus is described only as a conceptual, prototype-stage
model; the paper reports no deployment, empirical validation, institutional
adoption, or operational readiness.

**Keywords:** socio-technical systems; federated digital institutions;
human-AI coordination; traceability; accountability; governance;
contestability

# 1. Introduction

Digital institutions increasingly combine distributed authority, modular
capabilities, public records, and automated assistance. The design problem
becomes harder when these elements are not located in one unified authority
chain but instead operate across a constitutional center and semi-autonomous
local governance domains. In that setting, the institutional challenge is not
only whether a decision can be documented, but whether reviewers can identify
which authority applied, which module was configured, what evidence was used,
how AI assistance shaped the record, and how an affected party could request
correction or appeal. Socio-technical systems research treats those questions
as jointly organizational and technical rather than reducible to one domain
alone [@baxter2011sociotechnical].

Relevant literatures address parts of this problem without yet yielding a
single architecture for accountable governance across constitutionally
constrained modular ecosystems. Research on decentralized governance shows
that self-executing rules do not remove interpretation, amendment, or social
coordination [@hassan2021dao; @hsieh2018bitcoin]. Human-AI interaction
guidance emphasizes review, correction, and expectation setting rather than
an undifferentiated transfer of authority [@amershi2019guidelines]. Provenance
and credentialing standards help distinguish evidence lineage and machine
verification from institutional judgment [@w3c2013provdm; @w3c2025vcdm]. What
remains less clearly specified is how traceability, accountability,
contestability, and evidence boundaries should be preserved when bounded local
entities configure modular institutional functions under higher-order
constitutional constraints.

This paper addresses that gap by introducing Axodus as a prototype-stage
conceptual architecture and focused research agenda. The project originates
from a multi-year independent research and design effort. The present
contribution is limited to a conceptual model: it does not report a deployed
platform, functioning multi-tenant infrastructure, users, evaluation results,
validated controls, or operational authority.

The central contribution is a layered architecture for traceability and
accountability in federated modular digital institutions. It defines how
constitutional governance, bounded Tenant autonomy, service nuclei, evidence
packages, attributable AI assistance, and review paths can be organized into
one inspectable decision structure. Participation readiness, internal maturity
distinctions, and risk boundaries remain supporting components that frame how
this structure might later be evaluated, reduced, or rejected.

Implementation, deployment, institutional adoption, and empirical validation
are outside the paper's scope. The manuscript also excludes token design,
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
> preserve traceability, accountability, contestability, and evidence
> boundaries when semi-autonomous Tenant entities configure and govern service
> nuclei through human-AI-assisted decision processes?

Five tensions structure the problem.

1. **Central constraints versus local autonomy.** A constitutional layer may
   preserve coherence, while Tenant-level governance still requires bounded
   discretion over local decisions and configurations.
2. **Modularity versus governability.** Service separation may limit direct
   coupling, while modular selection can create hidden dependency chains,
   ambiguous authority, and fragmented review paths.
3. **Automation versus accountable disposition.** AI assistance can reduce
   analytical load, but responsibility can become unclear when its outputs
   influence authorization, escalation, or review.
4. **Participation versus bounded readiness.** Open participation may support
   legitimacy, while consequential governance actions may require reviewable
   preparation, accommodations, and appeal.
5. **Documentation versus operational truth.** A detailed specification can
   improve inspection while also creating a misleading impression of
   implementation, adoption, or production authority.

Axodus is proposed as one architecture for making these tensions explicit. It
is not presented as their solution.

# 4. Conceptual Architecture

The model comprises six logical layers. They describe conceptual
responsibilities and interfaces, not an implementation topology.

Information and control move through the architecture in different ways.
Control begins with constitutional constraints that define what a Tenant may
delegate, configure, or escalate. A Tenant decision can then select or govern
a service nucleus only within those constraints. Information moves through
evidence packages, provenance records, advisory analysis, rationale, and
review records so that later reviewers can reconstruct what happened and why.
Risk boundaries constrain which state transitions are permitted, while
contestability paths allow challenge, correction, escalation, and appeal.

**Illustrative synthetic scenario - Tenant module exception review.** A mock
Tenant governance body requests a temporary exception affecting one service
nucleus. The request includes the applicable constitutional rule, local
authority basis, declared conflicts, and a controlled evidence package. A
simulated AI review flags one conflict but omits a dependency between the
requested configuration and a review requirement. The designated human reviewer
withholds disposition, records the omission, and escalates the matter because a
risk boundary is triggered. An independent appeal role can then reconstruct
which constitutional constraint applied, which local choice was proposed, what
the simulated AI review changed, and why escalation occurred. This scenario is
an analytical illustration, not evidence of an Axodus implementation or
institutional process.

## 4.1 Constitutional governance layer

The constitutional governance layer defines higher-order rules: roles,
decision rights, prohibitions, amendment procedures, escalation paths, and
appeal conditions. Its purpose is to make non-delegable constraints visible
before local configuration begins. In this model, a valid action requires both
institutional justification and whatever technical authorization a future
implementation might use; neither alone would establish legitimacy.

## 4.2 Tenant governance layer

The Tenant governance layer represents a bounded local governance domain
operating under constitutional constraints. A Tenant may configure local
processes, select service nuclei, and allocate decision tasks only within the
scope permitted by the constitutional layer. The model treats Tenants as a
conceptual governance construct rather than as evidence of deployed multi-
tenant infrastructure, real communities, or operating customer entities.

## 4.3 Service nuclei layer

Service nuclei are abstract functional modules through which institutional
capabilities can be selected, bounded, and governed. The paper does not
present a product catalog. Instead, it treats a service nucleus as a
conceptual unit that should declare its purpose, inputs, outputs, delegated
authority, evidence requirements, dependencies, escalation conditions, and
failure behavior.

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
specify what a reviewable record should express; they do not prescribe a
storage system, cryptographic proof, or integrity guarantee.

## 4.5 AI-assistance layer

AI assistance remains advisory. It may support bounded tasks such as document
comparison, proposal summarization, inconsistency detection, constitutional
analysis support, adversarial checking, and operational planning support. Each
use should declare the task, source material, output, uncertainty where
available, human reviewer, and disposition. Humans retain decision authority
and responsibility.

This layer is intentionally role-abstract. The paper does not use named agent
labels, does not claim autonomous execution authority, and does not claim that
AI assistance itself enforces governance or security.

## 4.6 Risk-boundary and contestability layer

The risk-boundary and contestability layer constrains permissible actions and
keeps review paths available after a decision is proposed or made. A boundary
should identify the responsible role, triggering condition, required
evidence, permitted exception, and escalation path. Contestability requires a
participant or reviewer to identify the applicable rule, challenge evidence,
correct records, disclose conflicts, and request review by an appropriately
independent role.

Within this proposal, reviewer independence means separation from the original
decision, disclosure of conflicts, and recusal when a reviewer participated in
the contested analysis. Escalation paths should identify where a review moves
when authority, expertise, or capacity is insufficient. Human oversight
becomes nominal when a reviewer lacks authority, time, access to evidence, or
a practical ability to change the outcome [@tabassi2023airmf;
@amershi2019guidelines]. Contestability-by-design literature identifies human
review, intervention, and third-party scrutiny as relevant design features
[@alfrink2023contestable].

# 5. Participation Readiness as a Supporting Mechanism

A participation-readiness mechanism is proposed only as a supporting
institutional interface for learning, assessment, bounded eligibility, and
appeal in selected consequential contexts. It is not the paper's central
contribution and must not be treated as a general social ranking system.

The W3C credential model could inform portable representations, but
verification of an issuer and credential does not validate educational
quality or justify authorization [@w3c2025vcdm]. The governance problem
therefore includes who defines the criteria, how accommodations are provided,
how a participant can contest an outcome, and whether the requirement is
proportionate to the decision context.

The central hypothesis is that educational readiness may improve bounded
participation in selected high-consequence contexts. Competing hypotheses
remain equally important: the mechanism may exclude participants, centralize
curriculum power, encourage test gaming, or create privacy risks. It should be
rejected or redesigned if those harms cannot be controlled.

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

Before either initial study, the first empirical stage requires a controlled
environment rather than a deployed institutional system. The environment
should combine synthetic Tenant-governance scenarios, controlled evidence
packages, simulated AI-assistance records, planted errors, and a high-fidelity
mock-up or wizard-of-oz review interface. A preregistered protocol should
define reviewer tasks and proposed measurement criteria. These criteria are
study designs, not reported results.

**Primary initial study — RQ1: Traceability and reconstruction.** Does the
proposed evidence model help independent reviewers reconstruct Tenant-level
service-nucleus governance decisions more accurately and efficiently than a
document-only baseline? The controlled environment would support matched
governance scenarios and blinded review. Proposed measures are reconstruction
completeness, authority-conflict detection, missing-evidence detection, time
to reconstruct rationale, provenance error detection, reviewer disagreement,
and correct classification of whether an appeal can proceed. This is the
paper's primary evaluation priority because it most directly tests the central
claim about traceability and accountability in federated modular governance.

**Secondary initial study — RQ3: Human-AI reliance in advisory review.** For
bounded proposal-analysis tasks, how do provenance and mandatory human
disposition affect error detection, calibrated reliance, override behavior,
and review quality? The simulated AI records should include planted errors,
ambiguous cases, and contested recommendations. Proposed measures are planted-
error detection, unsupported-output detection, override or acceptance behavior
by condition, rationale quality, reviewer disagreement, and correction after
provenance information is shown. This is a secondary priority because the
architecture depends on bounded AI assistance being reviewable rather than
merely available.

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
paths are workable across constitutional and Tenant-level decisions.

The public evidence base for Axodus is currently limited to design
documentation. There are no results with which to assess feasibility,
usability, governance legitimacy, calibrated reliance, contestable appeals, or
social impact. The paper reports no deployment validation, no institutional
validation, no production operation, no token-design or token-distribution
claims, no operational-finance claims, no security guarantees, and no legal
or regulatory conclusion.

Human oversight can become nominal when reviewers lack time, authority,
evidence access, or practical power to change the outcome. AI assistance may
be unreliable, difficult to calibrate, or difficult to audit under realistic
workload and time pressure. Weak contestability or poorly designed appeal
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
synthetic Tenant-governance scenarios, and bounded AI-assistance tasks
suitable for initial traceability and reliance studies. Additional literature
hardening around governance quality, reviewer independence, empirical
institutional appeals, and participation-readiness validity remains a later
requirement before any broader external review is considered.

# 11. Conclusion

Axodus is proposed as a prototype-stage conceptual architecture for making
human-AI-assisted governance more traceable and accountable in federated
modular digital institutions. Its contribution is not a product catalog or
operational claim, but an inspectable arrangement linking constitutional
constraints, bounded Tenant autonomy, service nuclei, evidence and
provenance, advisory AI assistance, and review paths.

The next research step is to instantiate the minimum decision-and-evidence
model in a controlled experimental environment and test whether independent
reviewers can reconstruct and challenge Tenant-level governance decisions
under the proposed record structure.

# References

References are maintained in `references.bib`. All entries cited in this draft
have corresponding internal verification records in
`../../research/bibliography-verified.md`; final metadata rechecking is
required before any submission, public release, or external circulation.
