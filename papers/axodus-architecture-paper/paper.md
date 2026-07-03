---
title: "Axodus: A Prototype-Stage Conceptual Architecture for Traceability and Accountability in Human-AI-Assisted Digital Institutions"
author:
  - "Mauricio Z. Filho"
affiliation: "Independent Researcher, Axodus"
correspondence: "mzfshark@gmail.com"
project_discussion_forum: "Telegram @thinkincoin"
author_social_handle: "@mzfshark"
version: "Draft v0.3.2"
status: "Ready for internal peer review after targeted revision; not ready for external circulation or publication"
license: "CC BY 4.0"
document_type: "Prototype-stage conceptual architecture and focused research-agenda paper"
---

# Abstract

Digital institutions increasingly rely on automated assistance while still
requiring identifiable authority, reviewable evidence, and accountable human
oversight. Existing literatures address socio-technical design, decentralized
governance, human–AI interaction, and credentialing standards, but they do not
by themselves yield a focused conceptual architecture for traceability and
accountability in human–AI-assisted institutional decision making. This paper
presents Axodus as a prototype-stage conceptual architecture and focused
research agenda for that problem. Its central contribution is a layered model
for linking decision authority, evidence, bounded AI assistance, rationale,
and review paths in digital institutions. Supporting discussion addresses
participation readiness, bounded risk constraints, and complexity reduction.
Axodus is described only as a conceptual, prototype-stage model; the paper
reports no deployed system, empirical validation, or operational readiness.

**Keywords:** socio-technical systems; digital institutions; human–AI
coordination; traceability; accountability; governance; contestability

# 1. Introduction

Digital institutions can combine distributed governance, public
documentation, automated assistance, and participation requirements within the
same decision environment. Those capabilities do not by themselves determine
who may decide, what evidence supports a decision, how an automated analysis
should be reviewed, or how an affected party can challenge an outcome.
Socio-technical systems research therefore treats organizational design and
technical design as interdependent rather than assuming that one can be
derived from the other [@baxter2011sociotechnical].

Relevant literatures clarify parts of this problem but do not yet yield a
single focused institutional model for traceability and accountability under
human–AI-assisted decision making. Research on decentralized governance
highlights the continuing importance of interpretation, change, and social
coordination around self-executing rules [@hassan2021dao; @hsieh2018bitcoin].
Human–AI interaction guidance emphasizes expectation setting, correction, and
review rather than an undifferentiated transfer of authority
[@amershi2019guidelines]. Credentialing standards help separate machine
verification from institutional judgment [@w3c2025vcdm]. What remains less
clearly specified is how authority, evidence, bounded AI assistance,
contestability, and review paths should be organized together in one
inspectable conceptual architecture.

This paper addresses that gap by introducing Axodus as a prototype-stage
conceptual architecture and focused research agenda. The project originates
from a multi-year independent research and design effort. The present
contribution is limited to a model: it does not report a functioning platform,
production deployment, users, evaluation results, validated controls, or
operational authority.

The central contribution is a layered architecture for traceability and
accountability in human–AI-assisted digital institutions. It links
institutional authority, evidence, bounded AI assistance, decision rationale,
contestability, and review paths. The contribution lies in this specific
arrangement rather than in any layer considered alone. Participation
readiness, maturity separation, and risk boundaries remain supporting
components needed to frame how the arrangement might be inspected and
eventually evaluated.

Implementation, deployment, institutional adoption, and empirical validation
are outside the paper's scope. The manuscript also does not evaluate
educational effects, security properties, financial mechanisms, or legal
compliance.

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

## 2.2 Decentralized governance, traceability, and review

Hassan and De Filippi describe a DAO as a blockchain-based system in which
people coordinate through decentralized governance and self-executing rules
[@hassan2021dao]. Hsieh et al. distinguish machine consensus from the social
consensus required to alter protocols and organizational arrangements
[@hsieh2018bitcoin]. These distinctions caution against equating technical
distribution with accountable governance.

Decentralized finance provides one domain-specific example in which
composability can propagate dependencies across connected protocols
[@schar2021defi]. Broader claims about coupling and failure propagation require
evidence from complex-systems and socio-technical failure research rather than
generalization from that domain. **[REFERENCE NEEDED: complex-system coupling
and socio-technical failure]**

## 2.3 Human–AI oversight, calibrated reliance, and governance

Guidelines for human–AI interaction emphasize communicating system
capabilities, supporting correction, and learning from behavior over time
[@amershi2019guidelines]. At the organizational level, the NIST AI Risk
Management Framework treats governance, mapping, measurement, and management
as connected risk functions [@tabassi2023airmf]. These sources motivate an
architecture in which AI outputs are attributable inputs to decisions rather
than sovereign decisions and in which human review conditions remain visible.

Constitutional AI uses written principles to guide model behavior through
supervised learning and AI feedback [@bai2022constitutional]. Axodus uses
*constitutional* differently: it refers to institutional rules about
authority, prohibitions, amendments, review, and appeal. The proposed model
does not claim to train or align an AI model through Constitutional AI.

## 2.4 Credentials, participation readiness, and institutional judgment

The W3C Verifiable Credentials Data Model separates the cryptographic
verification of a credential from validation of whether its claims are fit for
a verifier's purpose [@w3c2025vcdm]. This matters here because a technically
verifiable record would not by itself establish fair assessment, learning, or
legitimate governance restriction.

## 2.5 Data provenance and accountable reconstruction

The W3C PROV Data Model describes provenance through entities, activities,
agents, derivations, attribution, and responsibility relationships
[@w3c2013provdm]. This vocabulary is useful for distinguishing source
artifacts, transformations, automated assistance, and responsible roles in a
decision record. It supports reconstruction of how an output was produced, but
does not by itself establish that the decision was legitimate, contestable, or
accountable. **[REFERENCE NEEDED: algorithmic accountability and institutional
audit]**

# 3. Problem Statement

The architecture addresses a design problem rather than an established
empirical effect:

> How can a digital institution make human–AI-assisted decisions more
> traceable, contestable, and accountable by linking authority, evidence,
> rationale, and review paths without conflating documentation with
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

Conceptually, the layers form a directional decision path:

1. constitutional governance defines the applicable roles, decision rights,
   prohibitions, and appeal rules;
2. a bounded institutional component receives a decision request and, where
   justified, checks participation-readiness conditions;
3. the evidence layer assembles source material, declared conflicts, and the
   authority basis for the request;
4. human–AI assistance may transform or analyze that material, with its task,
   inputs, output, and responsible reviewer recorded as provenance;
5. risk boundaries constrain the actions available to the authorized human
   decision-maker; and
6. the resulting decision and rationale enter a review path through which an
   independent role can inspect, correct, escalate, or hear an appeal.

Information therefore moves from rules, requests, and evidence through any
assistance into a decision record. Control remains with authorized human roles
constrained by governance and risk boundaries. Review flow can return disputed
evidence or rationale for correction without treating the original record as
an unchangeable interpretation.

**Illustrative synthetic scenario — policy exception review.** A mock policy
exception request includes an authority statement, the applicable rule, and a
controlled evidence package. A simulated AI summary omits one cited source.
The responsible reviewer records the omission, withholds disposition pending
correction, and escalates the request because a risk boundary is triggered. An
independent appeal role can then reconstruct which evidence was supplied, what
the simulated assistance changed, and why escalation occurred. This scenario
is an analytical illustration, not evidence of an Axodus implementation or
institutional process.

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

At the conceptual level, source documents and outputs can be treated as
entities, analysis and review steps as activities, and human or automated
participants as agents. Derivation and attribution relations can then connect
an output to its inputs and responsible roles [@w3c2013provdm]. These concepts
specify what a reviewable record should express; they do not prescribe a
storage system or integrity mechanism.

## 4.3 Modular institutional components

Bounded components represent institutional capabilities. A minimal conceptual
taxonomy includes the following functional classes:

- an **authority and role registry** for decision rights and delegations;
- an **evidence registry** and **AI-assistance provenance layer** for sources,
  transformations, and attributable automated inputs;
- a **decision-rationale record** and **conflict and disclosure register** for
  the basis and conditions of a decision;
- a **review and appeal path** and **risk-boundary controller** for challenge,
  escalation, and bounded action; and
- **participation-readiness support** for educational preparation before
  selected consequential activities.

These are component types, not a definitive inventory of Axodus modules or
claims of implementation. Each type should declare its purpose, inputs,
outputs, authority, dependencies, evidence requirements, and failure behavior.
Together they provide a conceptual path from authorized action and source
evidence through AI assistance and rationale to review or appeal.

## 4.4 Participation readiness support

An educational layer and a participation readiness mechanism are proposed as
supporting interfaces for learning and assessment. Their purpose would be to
help participants understand domain-specific risks and governance duties
before performing selected consequential actions. In this paper, they are
supporting elements rather than co-equal contributions. They must not become a
general social ranking system.

## 4.5 Human–AI assistance

AI services may support bounded tasks such as document comparison, proposal
summarization, inconsistency detection, risk flagging, and preparation of
review material. Each use should declare the task, source material, output,
uncertainty where available, human reviewer, and disposition. Humans retain
decision authority and responsibility.

## 4.6 Risk and review boundaries

The risk layer expresses constraints on authority, exposure, timing,
conflicts, and escalation. A boundary should identify the responsible role,
triggering condition, required evidence, permitted exception, and escalation
path. This connects bounded action to the decision and review records used for
accountability.

# 5. Modularity, Maturity, and Scope Reduction

The Axodus internal governance process distinguishes two orthogonal maturity
dimensions. **L-Level** refers to organizational, documentation, governance,
and authority maturity. **D-Level** refers to development, implementation,
technical validation, and operational maturity. L-Level does not measure code,
and D-Level does not measure governance. Neither dimension authorizes
production or sensitive action; production status and action authority require
separate gates.

The L0–L5 and D0–D5 rubric is an internal operational taxonomy, not an
empirically validated measurement instrument. This paper does not assign
levels to components. Its relevance here is limited to preventing
documentation from being mistaken for implementation, local implementation
from being mistaken for production, or maturity from being mistaken for
authority. The complete rubric is maintained separately in the project's
governance documentation.

Modularity is likewise a supporting hypothesis rather than an assured
property. Component boundaries may aid review, but they can also move
complexity into interfaces and make governability harder to assess.

The architecture should therefore be reduced before it is expanded. Initial
prototypes should:

- start with decisions for which reconstruction and appeal are material;
- use a minimum sufficient evidence-and-rationale record;
- separate advisory AI outputs from authoritative human decisions;
- require an evidence package before introducing automated assistance;
- scale review requirements to decision consequence; and
- remove a component when evaluation does not show that it improves
  reconstructability or contestability.

# 6. Participation Readiness Mechanism

The mechanism would link defined learning objectives, assessment, reviewable
results, bounded eligibility, and an appeal path for selected activities.

The W3C credential model could inform portable representations, but
verification of an issuer and credential does not validate educational quality
or justify authorization [@w3c2025vcdm]. The governance problem therefore
includes who defines the criteria, how accommodations are provided, and how a
participant can contest an outcome.

The central hypothesis is that educational readiness may improve the quality
of bounded participation in selected high-consequence contexts. Competing
hypotheses remain equally important: the mechanism may exclude participants,
centralize curriculum power, encourage test gaming, or create privacy risks.
It should be rejected or redesigned if those harms cannot be controlled.

Proposed evaluation criteria include false exclusion and false inclusion,
accessibility and accommodation, appeal availability and completion,
curriculum concentration, privacy burden, and evidence of improvement in the
specific decision context. Candidate safeguards include separating curriculum
design from authorization decisions, disclosing assessment conflicts, and
subjecting criteria to independent review. Participation-readiness gates should
be limited to contexts in which their necessity and proportionality can be
tested.

# 7. Governance, Accountability, and Human Oversight

The conceptual minimum decision record has seven fields: decision scope,
authorized roles, evidence considered, conflicts disclosed, automated
assistance used, decision and rationale, and review or appeal path.

AI assistance is governed by task-specific boundaries. Low-consequence
drafting may permit lightweight review; risk classification or proposal
analysis would require stronger provenance, independent checking, and explicit
human disposition. An AI output cannot approve its own use, resolve an appeal
about itself, or become the final bearer of responsibility.

The model should support contestability. Participants affected by a decision
need a way to identify applicable rules, challenge evidence, correct records,
and request review by an appropriately independent role. Immutable records,
where used, must not be treated as immutable interpretations.

Reviewer independence requires separation from the original decision,
disclosure of conflicts, and recusal when a reviewer has participated in the
contested analysis. Escalation paths should identify where a review moves when
authority, expertise, or capacity is insufficient. Process scalability can be
examined through queue size, review time, unresolved-case rate, and sampling
for secondary review. Role rotation and multi-role review are candidate
capture-resistance mechanisms whose effects require testing.

Human oversight becomes nominal when a reviewer lacks authority, time, access
to evidence, or a practical ability to change the outcome. These requirements
align with risk-oriented governance and human–AI interaction guidance
[@tabassi2023airmf; @amershi2019guidelines], while the design of independent
appeals and capture resistance requires additional support. **[REFERENCE
NEEDED: contestability and institutional appeals]**

# 8. Risk Boundaries as Supporting Constraints

Risk boundaries constrain action, exposure, process, and escalation. For each
consequential decision, the architecture links the applicable boundary to its
authority basis, supporting evidence, exception record, and review path.
Visible records are insufficient when assumptions or rationales remain
implicit. Cross-component dependencies should therefore be declared at the
interface where evidence, authority, or escalation crosses a component
boundary. If the dependency cannot be reviewed or bounded proportionately, the
design should reduce scope rather than add another control layer.

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

The evaluation program is intentionally prioritized rather than broad.

Before either initial study, the initial empirical stage requires a controlled
environment rather than a deployed institutional system. The environment
should combine synthetic decision scenarios, controlled evidence packages,
simulated AI-assistance records, planted errors, and a high-fidelity mock-up or
wizard-of-oz review interface. A preregistered protocol should define reviewer
tasks and proposed measurement criteria. These criteria are study designs, not
reported results.

**Primary initial study — RQ1: Traceability.** Does the proposed evidence
model help independent reviewers reconstruct decisions more accurately and
efficiently than a document-only baseline? The controlled environment would
support matched governance scenarios and blinded review. Proposed measures are
reconstruction completeness, missing-evidence detection, time to reconstruct
rationale, reviewer disagreement, authority-conflict detection, provenance
error detection, and correct classification of whether an appeal can proceed.
This is the paper's primary evaluation priority because it most directly tests
the central claim about traceability and accountability.

**Secondary initial study — RQ3: Human–AI reliance.** For bounded
proposal-analysis tasks, how do provenance and mandatory human disposition
affect error detection, calibrated reliance, override behavior, and review
quality? The simulated AI records should include planted errors and ambiguous
cases. Proposed measures are planted-error detection, unsupported-output
detection, override or acceptance behavior by condition, rationale quality,
reviewer disagreement, and correction after provenance information is shown.
This is a secondary priority because the architecture depends on bounded AI
assistance being reviewable rather than merely available.

**Staged future evaluation.** Evaluation should progress from controlled
artifact inspection to bounded reviewer studies using synthetic scenarios,
then to controlled prototype evaluation under a separately approved protocol.
Any later institutionally situated study would require additional governance,
ethics, legal, privacy, and evidence gates. Educational participation, maturity
reliability, and broader risk governance remain later research topics.

# 11. Limitations and Threats to Validity

This paper is conceptual and still broader than a mature external article
would ideally be. The architecture can appear coherent because it has not yet
encountered implementation constraints, institutional conflict, or field
conditions that would test whether its proposed review paths are workable.

The public evidence base for Axodus is currently limited to design
documentation. There are no results with which to assess feasibility,
usability, governance legitimacy, security, calibrated reliance, contestable
appeals, or social impact. Human oversight can become nominal when reviewers
lack time, authority, or expertise. AI assistance may be unreliable,
difficult to calibrate, or difficult to audit under realistic workload and
time pressure. Weak contestability or poorly designed appeal paths could make
traceability visible without making accountability meaningful.

Participation readiness mechanisms present particular risks of exclusion,
surveillance, curriculum capture, and false confidence. Modularity can hide
systemic coupling. Explicit rules can formalize unjust arrangements rather
than correct them. The proposed architecture may also be too complex to govern
in practice without substantial scope reduction.

The synthetic scenario is explanatory rather than empirical. Provenance
vocabulary does not establish record integrity or accountability, and the
proposed measures do not demonstrate performance. Institutionally situated
evaluation may also expose conflicts, incentives, and workload effects that a
controlled artifact cannot reproduce.

Web3-facing governance designs may also encounter regulatory uncertainty,
operational fragility, and jurisdiction-specific compliance burdens.

The paper does not provide legal, financial, security, or investment advice.
Its terminology may not map cleanly onto every jurisdiction or research
community.

# 12. Research Agenda

Near-term work should prioritize a minimal decision-and-evidence model and
bounded AI-assistance tasks suitable for initial traceability studies, together
with verification of provenance, algorithmic-accountability, contestability,
and socio-technical coupling literature.
Participation-readiness design, maturity specification, and broader governance
scenarios belong to later papers or technical notes, alongside educational
validity questions.

# 13. Conclusion

Axodus is proposed as a conceptual architecture for making human–AI-assisted
institutional decisions more traceable and accountable through linked
authority, evidence, attributable assistance, rationale, contestability, and
review paths. The model's immediate contribution is an inspectable arrangement
of functional responsibilities and interfaces through which accountability
assumptions can be examined.

The next research step is to instantiate the minimum decision-and-evidence
model in a controlled experimental environment and test whether independent
reviewers can reconstruct and challenge decisions under the proposed record
structure.

# References

References are maintained in `references.bib`. All entries cited in this draft
have corresponding internal verification records in
`../../research/bibliography-verified.md`; final metadata rechecking is
required before any submission, public release, or external circulation.
