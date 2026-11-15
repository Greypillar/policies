---
slug: control-maps
path: /trust/controls
group: Security
audience: Security teams
kind: Self-alignment
title: Control maps for AI
summary: Where Greypillar stands against the NIST AI Risk Management Framework, the OWASP Top 10 for LLM applications and the ISO/IEC 42001 control list. A self-alignment, not an audit.
banner: "{claim:status.public_service} Nobody has assessed this. Neither NIST nor OWASP certifies anyone."
record:
  Version: "1.0"
  State: Draft
  Effective: Not set
  Updated: 14 November 2026
  Reviewed: Written by Greypillar. Not independently assessed.
  Governing text: English
changes:
  - {version: "1.0", date: "14 November 2026", text: "First published draft."}
sources:
  - {n: 1, text: "NIST, Artificial Intelligence Risk Management Framework (AI RMF 1.0), NIST AI 100-1, January 2023. NIST's page says a revision is in progress; no revised text had been published when we looked.", href: "https://www.nist.gov/itl/ai-risk-management-framework"}
  - {n: 2, text: "OWASP GenAI Security Project, OWASP Top 10 for LLM Applications 2026, page dated 3 August 2026", href: "https://genai.owasp.org/resource/owasp-genai-llm-top-10-2026/"}
  - {n: 3, text: "ISO/IEC 42001:2023, Information technology - Artificial intelligence - Management system, Annex A", href: "https://www.iso.org/standard/81230.html"}
---

# How to read this
> lead: Three public lists of what responsible AI work looks like, and what Greypillar has against each. Most of it is design, not running software.

## 1 What this is and is not {#what status=live}
> In plain words: we compared ourselves with three public checklists. Nobody checked our answers.

1.1 This is self-alignment. Greypillar wrote it. It is not an audit, a certification or an assessment by anyone else.
1.2 NIST publishes the AI RMF as voluntary guidance. NIST does not certify, approve or list anyone against it. OWASP publishes a list of risks, not a standard to certify against, and does not certify anyone. ISO/IEC 42001 is a standard that an accredited body can certify an organisation against. Greypillar holds no such certificate and no audit has been started. {claim:assurance.certifications}
1.3 {claim:status.public_service} Greypillar has no customers and runs no AI system for anyone. The agents covered here are the ones planned for step 1, described in the [system card](/trust/system-card).
1.4 **In place** - exists today and has evidence. **Designed** - written down in a design or a draft, not built or not in force. **Not yet** - nothing exists. Not yet may or may not be planned; the note says. **Not applicable** - the risk does not arise in the first planned use.
1.5 Evidence marked internal is in Greypillar's private repositories and cannot be checked by readers. To ask what we can show, write to {claim:channel.email}.
1.6 A control is counted once. A designed control is never counted as in place. A document that describes a design is not evidence that a control runs.
1.7 The control numbers and titles belong to NIST, OWASP and ISO. They are not covered by the licence of this repository.

## 2 NIST AI RMF 1.0 {#nist}
> In plain words: 72 practices in four groups. Nothing is in place yet. Most are designed, and none of the measuring practices run.

2.1 Subcategory names below are our own short paraphrase, in NIST's numbering. The framework text is at the link in the sources.[^1]

Table: NIST AI RMF 1.0, GOVERN

| Control | What Greypillar has or designs | Evidence | Status |
|---|---|---|---|
| GOVERN 1.1 Legal and regulatory requirements understood | Thai PDPA, GDPR Article 28 and SCCs, Thai Civil and Commercial Code section 373, and Delaware law are identified for the first service. No full register. | Decision record (private) | Designed |
| GOVERN 1.2 Trustworthy-AI characteristics in policy | The commitments name behaviours (you decide, you can stop it, it shows its basis, it says it is an agent). Draft, not in force. | [Commitments](/commitments) | Designed |
| GOVERN 1.3 Oversight scaled to risk | Approval tiers by action class: automatic, notify, approve, never. Designed for GP-run systems, not deployed. | Designed in the GP-run infrastructure design (private) | Designed |
| GOVERN 1.4 Risk management is transparent and has policy | This page and the system card. No risk management policy. | [System card](/trust/system-card) | Not yet |
| GOVERN 1.5 Ongoing monitoring and review | No monitoring or review cycle exists. | None | Not yet |
| GOVERN 1.6 Inventory of AI systems | No AI system is deployed. A version lock of models and tools is designed for GP-run systems. | Designed in the GP-run infrastructure design (private) | Designed |
| GOVERN 1.7 Safe decommissioning of AI systems | One control stops the work, and a kill switch stops an agent scope. Designed, not built. | [Commitments](/commitments), commitment 5 | Designed |
| GOVERN 2.1 Roles and responsibility documented | The founder is accountable. Agents are designed to say who is responsible for what they write. No agent runs yet. | {claim:responsibility.agent_disclosure} | Designed |
| GOVERN 2.2 Personnel trained on AI risk | The accountable role. No training programme. | None | Not yet |
| GOVERN 2.3 Leadership takes responsibility | The founder decides and approves. The working rules are private and cannot be checked by readers. | Internal working rules (private repository) | Designed |
| GOVERN 3.1 Diverse perspectives in decisions | Not claimed. | None | Not yet |
| GOVERN 3.2 Human-AI roles and oversight set by policy | A person checks every brief before anything is sent. Nothing irreversible happens without a person's yes. Designed. | [System card](/trust/system-card); [Gate rule](/docs/gate-rule) | Designed |
| GOVERN 4.1 Culture that weighs AI risk | A claims registry checked in the website's build keeps public statements true. That is one control. Culture is not measured. | Claims registry, checked in CI (private repository) | Not yet |
| GOVERN 4.2 Teams document risks and impacts | Risks are written in design records. No impact assessment. | Design records (internal) | Not yet |
| GOVERN 4.3 Practices for testing and incident sharing | Website code has automated tests. No AI testing or incident sharing. | The website's CI workflow (private repository) | Not yet |
| GOVERN 5.1 Feedback from outside collected | Anyone can write to the contact address. No feedback has been collected, and there is no feedback process. | {claim:channel.email} | Not yet |
| GOVERN 5.2 Feedback is acted on | No process exists. | None | Not yet |
| GOVERN 6.1 Third-party AI risk policy | Designed for step 1 - OpenRouter restricted to model providers that do not train on inputs and keep no data. | Decision record (private) | Designed |
| GOVERN 6.2 Contingency for third-party failure | When the agents are unavailable, a person writes the reply. No other contingency. | [System card](/trust/system-card) | Not yet |

Table: NIST AI RMF 1.0, MAP

| Control | What Greypillar has or designs | Evidence | Status |
|---|---|---|---|
| MAP 1.1 Purpose, context and laws documented | The step 1 purpose and context are written in a draft. | [System card](/trust/system-card) | Designed |
| MAP 1.2 Interdisciplinary people involved | The accountable role. Not claimed. | None | Not yet |
| MAP 1.3 Mission and goals understood | Written in internal design records, which readers cannot check. | North star (internal) | Designed |
| MAP 1.4 Business value defined | Step 1 leads into a paid pilot. | Decision record (private) | Designed |
| MAP 1.5 Risk tolerance set | Not written. | None | Not yet |
| MAP 1.6 Requirements include social and technical effects | The commitments state requirements on consent, reversibility and no profiling. Draft. | [Commitments](/commitments) | Designed |
| MAP 2.1 Tasks and methods defined | Step 1 tasks are listed in a draft, with what the agents may not do. | [System card](/trust/system-card) | Designed |
| MAP 2.2 Knowledge limits and human oversight documented | Known limits are listed in a draft of the system card. | [System card](/trust/system-card) | Designed |
| MAP 2.3 Testing and scientific-validity issues identified | No evaluation has run. | [System card](/trust/system-card) | Not yet |
| MAP 3.1 Benefits examined | Not written as an assessment. | None | Not yet |
| MAP 3.2 Costs and harms examined | Not written as an assessment. | None | Not yet |
| MAP 3.3 Scope of use specified | Step 1 is bounded in a draft of the system card. | [System card](/trust/system-card) | Designed |
| MAP 3.4 Operator proficiency and training | No operator training. | None | Not yet |
| MAP 3.5 Human oversight processes defined | A person checks the brief and replies within one working day. Designed. | {claim:channel.reply_time} | Designed |
| MAP 4.1 Risks of components and third-party software mapped | Providers listed. Their risks not assessed. | [Subprocessors](/trust/subprocessors) | Not yet |
| MAP 4.2 Internal controls for those components | Website dependencies are updated by weekly pull requests. Nothing for the AI components. | Dependabot configuration (private repository) | Not yet |
| MAP 5.1 Likelihood and size of impacts identified | No impact assessment. | None | Not yet |
| MAP 5.2 Engagement with affected people | None yet. | None | Not yet |

Table: NIST AI RMF 1.0, MEASURE

| Control | What Greypillar has or designs | Evidence | Status |
|---|---|---|---|
| MEASURE 1.1 Metrics chosen, unmeasurable risks noted | No metrics for the agents. | None | Not yet |
| MEASURE 1.2 Metrics and controls reassessed | None. | None | Not yet |
| MEASURE 1.3 Independent reviewers involved | Nobody outside has reviewed anything. | None | Not yet |
| MEASURE 2.1 Test sets and methods documented | None. | None | Not yet |
| MEASURE 2.2 Human-subject evaluations meet requirements | None run. | None | Not yet |
| MEASURE 2.3 Performance shown in deployment-like conditions | None run. | None | Not yet |
| MEASURE 2.4 Monitoring in production | Nothing is in production. | None | Not yet |
| MEASURE 2.5 Validity and reliability shown, limits stated | Limits are stated. Validity is not shown. | [System card](/trust/system-card) | Not yet |
| MEASURE 2.6 Safety risk evaluated regularly | None. | None | Not yet |
| MEASURE 2.7 Security and resilience evaluated | No test of the agents. The website's build tests a small number of response headers. | The website's end-to-end tests (private repository) | Not yet |
| MEASURE 2.8 Transparency and accountability examined | Agent disclosure and a statement of who is responsible are designed. Not examined. | {claim:responsibility.agent_disclosure} | Not yet |
| MEASURE 2.9 Model explained and documented | Which models run is not yet fixed. | [System card](/trust/system-card) | Not yet |
| MEASURE 2.10 Privacy risk examined | No impact assessment. | None | Not yet |
| MEASURE 2.11 Fairness and bias evaluated | None. | None | Not yet |
| MEASURE 2.12 Environmental impact examined | None. | None | Not yet |
| MEASURE 2.13 The measuring itself evaluated | None. | None | Not yet |
| MEASURE 3.1 Ways to find new risks over time | None. | None | Not yet |
| MEASURE 3.2 Tracking risks that are hard to measure | None. | None | Not yet |
| MEASURE 3.3 Users can report problems | A report route is written in the draft system card. No agent runs yet. | [System card](/trust/system-card) | Designed |
| MEASURE 4.1 Measurement tied to real settings | None. | None | Not yet |
| MEASURE 4.2 Results inform trust decisions | None. | None | Not yet |
| MEASURE 4.3 Measured improvements documented | None. | None | Not yet |

Table: NIST AI RMF 1.0, MANAGE

| Control | What Greypillar has or designs | Evidence | Status |
|---|---|---|---|
| MANAGE 1.1 Does the system meet its purpose | Cannot be judged; nothing runs. | None | Not yet |
| MANAGE 1.2 Documented risks are ranked and treated | A ranked threat list exists for GP-run systems. Nothing for the product. | Designed in the GP-run infrastructure design (private) | Designed |
| MANAGE 1.3 Responses to top risks | Designed for step 1 - read-only agents, human check, no outside action. | [System card](/trust/system-card) | Designed |
| MANAGE 1.4 Remaining risk documented | Known limits only. | [System card](/trust/system-card) | Designed |
| MANAGE 2.1 Resources and non-AI options weighed | A person can do the whole task. The agents are optional. | [System card](/trust/system-card) | Designed |
| MANAGE 2.2 Ways to keep value of deployed systems | Nothing deployed. | None | Not yet |
| MANAGE 2.3 Response to unknown risks | None written. | None | Not yet |
| MANAGE 2.4 Ways to switch off or replace the AI | One control stops the work. Designed. | [Commitments](/commitments), commitment 5 | Designed |
| MANAGE 3.1 Third-party AI risk monitored | None. | None | Not yet |
| MANAGE 3.2 Pre-trained models monitored | None. | None | Not yet |
| MANAGE 4.1 Post-deployment monitoring plans | None. | None | Not yet |
| MANAGE 4.2 Continual improvement activities | None. | None | Not yet |
| MANAGE 4.3 Incidents and errors communicated | A short incident plan is stated in the security overview, section 9. It has not been tested, and no process exists. | [Security overview](/security) | Not yet |

## 3 OWASP Top 10 for LLM Applications 2026 {#owasp}
> In plain words: the ten ways OWASP says LLM applications fail. Our answers are about the one planned first use, and all are design.

3.1 Version: OWASP Top 10 for LLM Applications 2026, page dated 3 August 2026 and presented with OWASP's Agent Control Standard on 1 to 2 September 2026.[^2] OWASP's list page still showed the 2025 edition when we checked. The 2026 titles agree with OWASP's own repository, checked in a review on 14 November 2026.
3.2 OWASP publishes a list of risks. It does not certify anyone, and nobody can be OWASP-compliant. This table says how Greypillar's design addresses each risk. None of it has been tested.
3.3 The context is step 1 of Start: an agent reads what a visitor writes and at most one file, and prepares a brief for a person to check. See the [system card](/trust/system-card).

| Risk | What Greypillar designs | Evidence | Status |
|---|---|---|---|
| LLM01 Prompt injection | The visitor's words and file are untrusted. Agents are read-only, take no action in outside systems and send nothing. A person checks before anything leaves. Files are stored as received and never opened on the intake server; they are read in sandboxes on a separate server. The gate rule says free text is no fact. No red-team test has run. | [System card](/trust/system-card); [Gate rule](/docs/gate-rule); decision record (private) | Designed |
| LLM02 Sensitive information disclosure | An agent reads only the one request it is preparing. Model providers are restricted to those that do not train on inputs and keep no data. A retention rule is decided. Nothing is tested. | {claim:data_use.no_training_default}; decision record (private) | Designed |
| LLM03 Excessive agency | No tools in outside systems. Read-only access to the intake. Past step 1, every effect must pass the gate rule and stay inside what was accepted. | [Gate rule](/docs/gate-rule); [System card](/trust/system-card) | Designed |
| LLM04 Supply chain | Website dependencies are pinned and updated by weekly pull requests. The model route (OpenRouter and its providers) is chosen and not yet built. Not assessed. | Dependabot configuration (private repository); [Subprocessors](/trust/subprocessors) | Designed |
| LLM05 Data and model poisoning | Greypillar does not train or fine-tune a model on visitor content. Step 1 has no retrieval corpus. Poisoned input is covered by LLM01. | {claim:data_use.no_training_default} | Designed |
| LLM06 Unbounded consumption | One file per submission. A monthly spending limit per model key is designed for GP-run systems, and a public cost cap is a gate before Start opens. | Website plan and GP-run infrastructure design (private) | Designed |
| LLM07 Misinformation | A brief is provisional and a person checks it. Public claims come from a registry with expiry dates. Agents' statements about Greypillar are not checked against it automatically. | [System card](/trust/system-card) | Designed |
| LLM08 Hidden context exposure | Credentials are designed to be injected at a boundary and never placed in a model's context. The prompt is not written yet. | Designed in the GP-run infrastructure design (private) | Designed |
| LLM09 Vector and embedding weaknesses | Step 1 has no vector store or embeddings. If one is added, this row changes. | [System card](/trust/system-card) | Not applicable |
| LLM10 Improper output handling | The brief is shown to a person as plain text. Nothing executes an agent's output. Not built. | [System card](/trust/system-card) | Designed |

## 4 ISO/IEC 42001:2023 Annex A {#iso}
> In plain words: ISO's list of controls for managing AI. We have no AI management system. Only titles are listed here.

4.1 ISO/IEC 42001 is a management-system standard. Greypillar has no AI management system, has not started certification and does not claim conformity. Paid assurance such as ISO starts when the first enterprise asks.[^3]
4.2 Only the control numbers and short titles are listed. ISO's wording is not reproduced and is available from ISO. The titles come from a secondary source and were not checked against the standard itself.

| Control | What Greypillar has or designs | Evidence | Status |
|---|---|---|---|
| A.2.2 AI policy | The AI disclosure is in force from the opening of greypillar.ai. The commitments are in draft. No AI policy. | [AI disclosure](/legal/ai-disclosure) | Designed |
| A.2.3 Alignment with other policies | None. | None | Not yet |
| A.2.4 Review of the AI policy | None. | None | Not yet |
| A.3.2 AI roles and responsibilities | The founder is accountable. Agents are designed to say who is responsible. No agent runs yet. | {claim:responsibility.agent_disclosure} | Designed |
| A.3.3 Reporting of concerns | Write to the contact address, or to security@greypillar.ai for a security problem (tested 14 November 2026). No process for concerns about AI exists. | {claim:channel.email} | Designed |
| A.4.2 Resource documentation | A version lock is designed for GP-run systems. | GP-run infrastructure design (private) | Designed |
| A.4.3 Data resources | The data the first service will hold is listed. | Decision record (private) | Designed |
| A.4.4 Tooling resources | As A.4.2. | GP-run infrastructure design (private) | Designed |
| A.4.5 System and computing resources | A rented server in Helsinki and a model route through OpenRouter, designed, not built. | Decision record (private) | Designed |
| A.4.6 Human resources | The accountable role. No competence record. | None | Not yet |
| A.5.2 AI system impact assessment process | None. | None | Not yet |
| A.5.3 Documentation of impact assessments | None. | None | Not yet |
| A.5.4 Impact on individuals or groups | No assessment. The commitments rule out profiling people. | [Commitments](/commitments) | Not yet |
| A.5.5 Societal impacts | None. | None | Not yet |
| A.6.1.2 Objectives for responsible development | Written as commitments, draft. | [Commitments](/commitments) | Designed |
| A.6.1.3 Processes for responsible design and development | A design method and the gate rule specification. Not an ISO process. | [Gate rule](/docs/gate-rule) | Designed |
| A.6.2.2 AI system requirements and specification | The gate rule is specified, with its clauses and tests. | [Gate rule](/docs/gate-rule) | Designed |
| A.6.2.3 Design and development documentation | Specification and decision records. | Specification (internal) | Designed |
| A.6.2.4 Verification and validation | The gate rule's tests run against a reference model in the specification, each with a seeded defect. No agent has been evaluated. | [Gate rule](/docs/gate-rule) | Designed |
| A.6.2.5 AI system deployment | Nothing deployed. | None | Not yet |
| A.6.2.6 AI system operation and monitoring | Nothing operating. | None | Not yet |
| A.6.2.7 AI system technical documentation | The system card is a draft. | [System card](/trust/system-card) | Designed |
| A.6.2.8 Recording of event logs | An append-only audit record with metadata only is designed. Not deployed. | GP-run infrastructure design (private) | Designed |
| A.7.2 Data for development and enhancement | No training on content. | {claim:data_use.no_training_default} | Designed |
| A.7.3 Acquisition of data | Visitor submissions only, and only on the visitor's action. Not built. | Decision record (private) | Designed |
| A.7.4 Quality of data | None. | None | Not yet |
| A.7.5 Data provenance | Commitment 6 says a result shows what it rests on. Draft. | [Commitments](/commitments), commitment 6 | Designed |
| A.7.6 Data preparation | None. | None | Not yet |
| A.8.2 System documentation for users | The system card and documentation pages. | [System card](/trust/system-card) | Designed |
| A.8.3 External reporting | Write to the contact address, or to security@greypillar.ai for a security problem (tested 14 November 2026). | {claim:channel.email} | Designed |
| A.8.4 Communication of incidents | A short incident plan is stated in the security overview, section 9. No process and no exercise. | [Security overview](/security) | Not yet |
| A.8.5 Information for interested parties | Agents are designed to say they are agents and who is responsible. No agent runs yet. | {claim:responsibility.agent_disclosure} | Designed |
| A.9.2 Processes for responsible use | Acceptable use is in progress. | [Terms and policies](/trust) | Designed |
| A.9.3 Objectives for responsible use | The commitments. | [Commitments](/commitments) | Designed |
| A.9.4 Intended use of the AI system | Stated for step 1 in a draft. | [System card](/trust/system-card) | Designed |
| A.10.2 Allocating responsibilities | Three tiers of responsibility are designed. | {claim:responsibility.tiers} | Designed |
| A.10.3 Suppliers | Model providers are restricted to those that do not train on inputs and keep no data. Subprocessors are listed. No supplier agreements are in force. | [Subprocessors](/trust/subprocessors) | Designed |
| A.10.4 Customers | Customer terms based on Common Paper are in progress. | [Terms and policies](/trust) | Designed |
