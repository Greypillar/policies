---
slug: star-self-assessment
path: /trust/star
group: Security
audience: Security teams
kind: Self-assessment
title: CSA STAR Level 1 self-assessment
summary: Greypillar's answers to the Cloud Security Alliance's 283-question CAIQ v4.1, written by Greypillar and not independently assessed. Most answers are Planned or No because there is no service yet.
banner: "{claim:status.public_service} A draft self-assessment, labelled self-assessed. Not submitted to the CSA STAR Registry. Written by Greypillar. Not independently assessed."
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
  - {n: 1, text: "Cloud Security Alliance, STAR Level 1: Security Questionnaire (CAIQ v4.1), questionnaire version 4.1.0, specification Cloud Controls Matrix 4.1.1, page dated 27 January 2026", href: "https://cloudsecurityalliance.org/artifacts/star-level-1-security-questionnaire-caiq-v4-1"}
  - {n: 2, text: "Cloud Security Alliance, STAR Registry and Level 1 self-assessment", href: "https://cloudsecurityalliance.org/star"}
---

# How to read this
> lead: This is a list of what Greypillar can and cannot show today, one line per question, with no credit for what is only intended.

## 1 How to read this {#read status=live}
> In plain words: Yes means a control exists now and we can point to it. Everything else is No, Planned or Not applicable.

1.1 This is a self-assessment: Greypillar wrote it and nobody has checked it. It is not a certification, an audit or a CSA listing. It is not submitted to the CSA STAR Registry. Greypillar may submit it, and this page will say when that happens.
1.2 **Yes** - a control demonstrably exists today for something Greypillar actually runs, and the note names the evidence. A statement by Greypillar that nobody has checked is not evidence and does not make a Yes.
1.3 **Planned** - the control is decided or designed, with a pointer, and is not in place. Nothing designed counts as done.
1.4 **No** - not in place, or in place but not evidenced. Where something partly exists, the note says what. A No is not a hidden Yes.
1.5 **Not applicable** - the question concerns something Greypillar does not have or do, such as a facility or a person it has engaged, and the note says why. When Greypillar starts to have or do it, the answer changes. A question about something Greypillar intends to build is Planned or No.
1.6 Product controls are all Planned or No. The product does not exist: {claim:status.public_service} {claim:status.customers} {claim:assurance.certifications}
1.7 Evidence in private repositories cannot be checked by readers. Where evidence is private, the note says so. To ask what we can show, write to {claim:channel.email}.
1.8 The CAIQ accepts only Yes, No and N/A. When Greypillar may submit, each Planned answer is entered as No, with the plan in the description column. The official spreadsheet also asks who owns each control (the cloud provider, a third party or both). The ownership line under each domain heading here is Greypillar's reading. It is entered control by control at submission.
1.9 Every answer is as of 14 November 2026, before greypillar.ai opens. Where an answer depends on the opening, such as the Start intake, the note says so and says the date. An answer changes only when this page is updated and dated.

## 2 What was assessed {#scope status=live}
> In plain words: the website, email, the code repository and the accounts behind them. Nothing else exists to assess.

2.1 The service under assessment is {claim:entity.legal_name}, its website at greypillar.ai and the accounts and tools behind it. There is no hosted product and no customer data.
2.2 What runs today: the website on Vercel behind Cloudflare, shown as a holding page; email on Google Workspace; the website's source in a private GitHub repository with automated checks; one accountable role.
2.3 What is designed and not built on 14 November 2026: the Start intake on a server Greypillar rents in Helsinki, a credentials broker and secrets manager, audit logging, backups, and the product itself. Each answer that depends on them is Planned.
2.4 Questionnaire version: CAIQ v4.1.0 against Cloud Controls Matrix 4.1.1, 283 questions in 17 domains, downloaded from the Cloud Security Alliance on 12 November 2026.[^1] The spreadsheet records the release as 1 November 2025; the CSA page is dated 27 January 2026.
2.5 The CSA's licence does not allow the questionnaire to be modified or redistributed. This page therefore gives each question's ID and a short paraphrase, never the CSA's wording. The official spreadsheet, from the link in the sources, is what Greypillar fills in and submits. The question IDs and the paraphrases belong to the CSA. They are not covered by the licence of this repository.

## 3 Counts {#counts status=live}
> In plain words: 2 of 283 answers are Yes. That is the honest picture of a company with no service yet.

Table: Answers across all 283 questions

| Answer | Questions |
|---|---|
| Yes | 2 |
| Planned | 70 |
| No | 179 |
| Not applicable | 32 |
| Total | 283 |

Table: Answers by domain

| Domain | Yes | Planned | No | Not applicable |
|---|---|---|---|---|
| A&A Audit and assurance | 0 | 1 | 7 | 0 |
| AIS Application and interface security | 1 | 2 | 10 | 0 |
| BCR Business continuity and resilience | 0 | 3 | 15 | 1 |
| CCC Change control and configuration | 0 | 1 | 11 | 0 |
| CEK Cryptography and key management | 0 | 0 | 23 | 0 |
| DCS Datacenter security | 0 | 1 | 7 | 20 |
| DSP Data security and privacy lifecycle | 0 | 18 | 6 | 0 |
| GRC Governance, risk and compliance | 0 | 3 | 7 | 0 |
| HRS Human resources | 0 | 1 | 12 | 7 |
| IAM Identity and access management | 0 | 8 | 11 | 0 |
| IPY Interoperability and portability | 0 | 5 | 3 | 0 |
| I&S Infrastructure security | 0 | 3 | 11 | 1 |
| LOG Logging and monitoring | 0 | 8 | 10 | 1 |
| SEF Security incident management | 0 | 4 | 12 | 0 |
| STA Supply chain management, transparency and accountability | 0 | 7 | 12 | 0 |
| TVM Threat and vulnerability management | 1 | 5 | 9 | 0 |
| UEM Universal endpoint management | 0 | 0 | 13 | 2 |

## 4 A&A: Audit and assurance {#aa}
> In plain words: Greypillar owns these. Nothing has been audited.

| Question | Short question | Answer | Evidence or note |
|---|---|---|---|
| A&A-01.1 | Audit and assurance policy exists | No | Not written. No decision to write it has been made. |
| A&A-01.2 | Policy reviewed yearly | No | Not written. No decision to write it has been made. |
| A&A-02.1 | Independent audit every year | No | No independent assessment has been done. Paid assurance starts on triggers, not yearly: a penetration test with the hosted service, SOC 2 or ISO when the first enterprise asks (decision record, private). |
| A&A-03.1 | Audits planned by risk | Planned | The triggers above are the plan. No risk-based schedule is written. |
| A&A-04.1 | Compliance with audit requirements verified | No | Not in place and not yet designed. |
| A&A-05.1 | Audit management process | No | Not in place and not yet designed. |
| A&A-06.1 | Corrective-action plan for audit findings | No | No audit has been done, so there are no findings. The gaps in this document are the working list. |
| A&A-06.2 | Remediation status reported | No | Not in place and not yet designed. |

## 5 AIS: Application and interface security {#ais}
> In plain words: Scope is the website. The product does not exist yet. Vercel and Cloudflare run the website; Greypillar owns its code and configuration.

| Question | Short question | Answer | Evidence or note |
|---|---|---|---|
| AIS-01.1 | Application security policy exists | No | Not written. No decision to write it has been made. |
| AIS-01.2 | Policy reviewed yearly | No | Not written. No decision to write it has been made. |
| AIS-02.1 | Baseline security requirements for applications | No | Partly. The site's configuration sets a content security policy, frame refusal, no-sniff, referrer and permissions policies, and the hosting platform adds HSTS. Observed on greypillar.ai on 14 November 2026. The site's browser test checks only two headers. There is no written baseline for the website. |
| AIS-03.1 | Application security metrics | No | Not in place and not yet designed. |
| AIS-04.1 | Secure development lifecycle defined | No | Partly. Changes go through version control and automated checks (see AIS-05.2). There is no written lifecycle, threat-modelling step or security review step. |
| AIS-05.1 | Test strategy with acceptance criteria | No | Automated checks exist (AIS-05.2). No written security acceptance criteria. |
| AIS-05.2 | Testing is automated | Yes | Website only. Each pull request and each push to main runs type checks, ESLint, stylelint, Prettier, the claims-registry check, unit tests, a build and browser tests in Chromium and WebKit. Evidence - the website repository's CI workflow (private repository). |
| AIS-06.1 | Secure, standard deployment | No | No written deployment standard. The site is built and served by Vercel behind Cloudflare. |
| AIS-06.2 | Deployment automated | No | Not claimed until the production deploy path is written down. |
| AIS-07.1 | Vulnerabilities fixed by a defined process | No | Partly. Weekly Dependabot update pull requests are configured (see TVM-06.1). No written fix timelines. |
| AIS-07.2 | Remediation automated where possible | No | Partly. Dependabot proposes updates; a person decides and merges. Next.js is pinned on purpose and its updates are a person's decision. |
| AIS-08.1 | APIs secured by process and technical measures | Planned | The site has no customer API. The product's interface contract is specified and its reference pages stay closed until a first callable interface exists (/docs/gate-rule for the rule it must keep). |
| AIS-08.2 | API reviews yearly | Planned | Follows the first API. |

## 6 BCR: Business continuity and resilience {#bcr}
> In plain words: Greypillar owns these. Providers run their own resilience, which Greypillar has not assessed. No continuity programme exists.

| Question | Short question | Answer | Evidence or note |
|---|---|---|---|
| BCR-01.1 | Continuity and resilience policy | No | Not in place and not yet designed. |
| BCR-01.2 | Policy reviewed yearly | No | Not in place and not yet designed. |
| BCR-02.1 | Continuity criteria based on impact | No | Not in place and not yet designed. |
| BCR-02.2 | Risk and impact analysis reviewed yearly | No | Not in place and not yet designed. |
| BCR-03.1 | Strategies to reduce disruption | No | Not in place and not yet designed. |
| BCR-04.1 | Continuity plan | No | Not in place and not yet designed. |
| BCR-05.1 | Continuity documentation | No | Not in place and not yet designed. |
| BCR-05.2 | Documentation available to stakeholders | No | Not in place and not yet designed. |
| BCR-05.3 | Documentation reviewed yearly | No | Not in place and not yet designed. |
| BCR-06.1 | Continuity plans tested yearly | No | Not in place and not yet designed. |
| BCR-07.1 | Communication channels during an event | No | Email only ({claim:channel.email}). No status page and no written procedure. |
| BCR-08.1 | Backups run regularly | Planned | Designed for GP-run systems - regular backups kept as two locked copies at separate providers. Designed, not deployed (GP-run infrastructure design, private; nothing deployed). The website's source is in GitHub; no backup of it is claimed. |
| BCR-08.2 | Backups protected | Planned | Same design - protected copies that the host cannot change. Not deployed. |
| BCR-08.3 | Backups can be restored | Planned | Same design - a regular restore check and a periodic rebuild. No restore has been tested. |
| BCR-09.1 | Disaster response plan | No | Not in place and not yet designed. |
| BCR-09.2 | Plan updated yearly | No | Not in place and not yet designed. |
| BCR-10.1 | Disaster plan exercised yearly | No | Not in place and not yet designed. |
| BCR-10.2 | Emergency authorities in the exercise | Not applicable | No exercise exists and Greypillar has no premises. |
| BCR-11.1 | Redundant equipment in dispersed sites | No | Greypillar owns no business-critical equipment. It rents servers, and no redundancy design is written for them. Its providers' redundancy has not been assessed by Greypillar. |

## 7 CCC: Change control and configuration {#ccc}
> In plain words: Greypillar owns these for the website code. The accountable role makes changes.

| Question | Short question | Answer | Evidence or note |
|---|---|---|---|
| CCC-01.1 | Change management policy | No | Not written. No decision to write it has been made. |
| CCC-01.2 | Policy reviewed yearly | No | Not written. No decision to write it has been made. |
| CCC-02.1 | Quality change control with testing | No | Partly. Website changes are made on branches and pull requests, and the automated checks above run on them. Nothing evidences that a failing check blocks a merge. |
| CCC-03.1 | Change procedure implemented | No | Version control keeps a history of every website change. No written procedure. |
| CCC-04.1 | Authorisation of asset changes | No | Not in place and not yet designed. |
| CCC-05.1 | Agreements limit changes to customer environments | Planned | The Common Paper SLA and DPA are the base for the customer terms (decision record, private). No customer environment exists. |
| CCC-06.1 | Configuration baselines | No | Not in place and not yet designed. |
| CCC-06.2 | Baselines reviewed yearly | No | Not in place and not yet designed. |
| CCC-07.1 | Alert on drift from baseline | No | Not in place and not yet designed. |
| CCC-08.1 | Exception process for changes | No | Not in place and not yet designed. |
| CCC-08.2 | Aligned with policy exceptions | No | Not in place and not yet designed. |
| CCC-09.1 | Roll back to a known good state | No | Not claimed. Version control would allow a revert; no rollback procedure is written or tested. |

## 8 CEK: Cryptography and key management {#cek}
> In plain words: No programme exists. Providers handle encryption for the services Greypillar uses.

| Question | Short question | Answer | Evidence or note |
|---|---|---|---|
| CEK-01.1 | Cryptography and key policy | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-01.2 | Policy reviewed yearly | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-02.1 | Key management roles | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-03.1 | Data protected at rest and in transit with certified libraries | No | Greypillar holds no customer data. Providers terminate TLS for the website. Nothing here is claimed as a Greypillar control. |
| CEK-04.1 | Industry-standard algorithms | No | Same. Provider-managed; not independently verified. |
| CEK-05.1 | Cryptography change management | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-06.1 | Cost-benefit review of cryptography changes | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-07.1 | Cryptography risk programme | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-08.1 | Customers manage their own keys | No | Not specified yet. The four places work can run (cloud, yours, machine, offline) are designed; key custody for each is not. |
| CEK-09.1 | Key systems audited by risk | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-09.2 | Key systems audited yearly | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-10.1 | Keys generated with approved libraries | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-11.1 | Private keys have a unique purpose | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-12.1 | Keys rotated on a cryptoperiod | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-13.1 | Keys revoked when compromised | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-14.1 | Keys destroyed securely | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-15.1 | Keys created pre-activated | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-16.1 | Key state changes approved | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-17.1 | Keys deactivated at expiry | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-18.1 | Archived keys held securely | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-19.1 | Use of compromised keys controlled | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-20.1 | Key recovery risk assessed | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |
| CEK-21.1 | Key inventory and status tracking | No | No cryptography or key-management programme exists. Greypillar holds no customer data and manages no customer keys. |

## 9 DCS: Datacenter security {#dcs}
> In plain words: Third-party owned. Greypillar operates no facility, so most questions do not apply. The providers are Vercel, Cloudflare, Google, GitHub and Hetzner.

| Question | Short question | Answer | Evidence or note |
|---|---|---|---|
| DCS-01.1 | Physical and environmental security policy | Not applicable | Greypillar operates no data centre, office or other facility. Facilities belong to its providers and were not assessed by Greypillar. |
| DCS-01.2 | Policy reviewed yearly | Not applicable | Greypillar operates no data centre, office or other facility. Facilities belong to its providers and were not assessed by Greypillar. |
| DCS-02.1 | Disposal policy for equipment used off premises | No | The accountable role works on its own equipment. No disposal procedure is written. |
| DCS-02.2 | Data destruction so recovery is impossible | No | Same. |
| DCS-02.3 | Disposal policy reviewed yearly | No | Same. |
| DCS-03.1 | Relocation of hardware, software or data offsite | Not applicable | No hardware, software or data is moved to alternate sites as a managed process. |
| DCS-03.2 | Relocation needs verifiable authorisation | Not applicable | Same. |
| DCS-03.3 | Relocation policy reviewed yearly | Not applicable | Same. |
| DCS-04.1 | Safe, secure working environments | Not applicable | Greypillar operates no data centre, office or other facility. Facilities belong to its providers and were not assessed by Greypillar. |
| DCS-04.2 | Policy reviewed yearly | Not applicable | Greypillar operates no data centre, office or other facility. Facilities belong to its providers and were not assessed by Greypillar. |
| DCS-05.1 | Secure transport of physical media | Not applicable | Greypillar ships no physical media. |
| DCS-05.2 | Policy reviewed yearly | Not applicable | Same. |
| DCS-06.1 | Assets classified by business risk | No | Not in place and not yet designed. |
| DCS-06.2 | Classification reviewed yearly | No | Not in place and not yet designed. |
| DCS-07.1 | Assets catalogued and tracked | No | Partly. An inventory of the servers Greypillar rents exists in the GP-run infrastructure design (private). No tracked asset catalogue. |
| DCS-07.2 | Catalogue reviewed yearly | No | Not in place and not yet designed. |
| DCS-08.1 | Physical security perimeters | Not applicable | Greypillar operates no data centre, office or other facility. Facilities belong to its providers and were not assessed by Greypillar. |
| DCS-09.1 | Equipment identification for connection authentication | Planned | Designed - private access limited by device (GP-run infrastructure design, private; nothing deployed). |
| DCS-10.1 | Only authorised people enter secure areas | Not applicable | Greypillar operates no data centre, office or other facility. Facilities belong to its providers and were not assessed by Greypillar. |
| DCS-10.2 | Access control records kept | Not applicable | Greypillar operates no data centre, office or other facility. Facilities belong to its providers and were not assessed by Greypillar. |
| DCS-11.1 | Perimeter surveillance at data centres | Not applicable | Greypillar operates no data centre, office or other facility. Facilities belong to its providers and were not assessed by Greypillar. |
| DCS-12.1 | Data centre staff trained for adverse events | Not applicable | Greypillar operates no data centre, office or other facility. Facilities belong to its providers and were not assessed by Greypillar. |
| DCS-13.1 | Cabling protected | Not applicable | Greypillar operates no data centre, office or other facility. Facilities belong to its providers and were not assessed by Greypillar. |
| DCS-14.1 | Environmental controls monitored | Not applicable | Greypillar operates no data centre, office or other facility. Facilities belong to its providers and were not assessed by Greypillar. |
| DCS-15.1 | Utilities secured and tested | Not applicable | Greypillar operates no data centre, office or other facility. Facilities belong to its providers and were not assessed by Greypillar. |
| DCS-16.1 | Critical equipment kept from high-risk locations | Not applicable | Greypillar operates no data centre, office or other facility. Facilities belong to its providers and were not assessed by Greypillar. |
| DCS-17.1 | Data centre security metrics | Not applicable | Greypillar operates no data centre, office or other facility. Facilities belong to its providers and were not assessed by Greypillar. |
| DCS-18.1 | Continuous data centre operations | Not applicable | Greypillar operates no data centre, office or other facility. Facilities belong to its providers and were not assessed by Greypillar. |

## 10 DSP: Data security and privacy lifecycle {#dsp}
> In plain words: Greypillar holds no customer or visitor data today. Everything about the first service (Start) is designed and not built.

| Question | Short question | Answer | Evidence or note |
|---|---|---|---|
| DSP-01.1 | Data security and privacy policies | Planned | As of 14 November 2026 the privacy notice and the retention schedule (version 1.0) are written and take effect on the opening of greypillar.ai. No data security policy is written. Decision record (private). |
| DSP-01.2 | Policies reviewed yearly | Planned | Follows the policy; first review 12 months after it takes effect. |
| DSP-02.1 | Secure data disposal | Planned | Decided - a deletion rule for what a visitor sends through Start (see DSP-16.1). No data exists yet, so no disposal has run. |
| DSP-03.1 | Inventory of sensitive and personal data | Planned | The data the first service will hold (messages, one file, a name and work email, aggregate site analytics) is listed in the decision record. No inventory file yet. |
| DSP-03.2 | Inventory reviewed yearly | Planned | Follows the inventory. |
| DSP-04.1 | Data classified by type and sensitivity | No | Not in place and not yet designed. |
| DSP-05.1 | Data flow documentation | Planned | As of 14 November 2026, designed for Start - the site's server function calls the intake through an encrypted Cloudflare tunnel that requires a secret token, and agents prepare a brief through OpenRouter. The intake has no open port to the internet. Not deployed on that date, and the agents are not built (decision record, private). |
| DSP-05.2 | Data flows reviewed yearly | Planned | Follows the first service. |
| DSP-06.1 | Data ownership and stewardship documented | Planned | The privacy notice (version 1.0) names the controller and takes effect on the opening of greypillar.ai. |
| DSP-06.2 | Stewardship reviewed yearly | Planned | Follows the notice. |
| DSP-07.1 | Security by design in products | Planned | Designed - the gate rule, an intake that has no open port to the internet, files never opened on the intake server (/docs/gate-rule; decision record). Nothing running on 14 November 2026. |
| DSP-08.1 | Privacy by design in products | Planned | Designed - cookieless aggregate analytics, replay only with consent, inputs masked, Start never recorded, no training on content. Not live. |
| DSP-08.2 | Privacy settings default to protective | No | Partly. On 14 November 2026 the site sets no cookies (it keeps the visitor's light level in local storage), no analytics runs, and its content security policy sets form-action to none (response headers observed that day). These are absences, not a privacy-settings control. When analytics and Start open, the privacy notice (sections 5 and 6) sets their defaults: nothing stored without a yes, recording only with consent, Start never recorded. Evidence - the cookies page text. |
| DSP-09.1 | Data protection impact assessment | No | None done. To be done before the first service takes personal data. |
| DSP-10.1 | Transfers of personal data protected | Planned | Designed - an encrypted tunnel that requires a secret token for the one internal call. Not deployed on 14 November 2026. |
| DSP-11.1 | Access, correction and deletion requests | Planned | Decided - deletion on request. The privacy notice names the route and takes effect on the opening of greypillar.ai. Thai PDPA applies in full (decision record, private). |
| DSP-12.1 | Personal data used only for the stated purpose | Planned | {claim:data_use.no_training_default} Not in force. |
| DSP-13.1 | Controls on sub-processing | Planned | The Common Paper DPA is the base; each subprocessor change is published 30 days before use (decision record). No DPA is in force. |
| DSP-14.1 | Sub-processors disclosed before processing | Planned | Subprocessor table at /trust/subprocessors, drafted, with a 30-day notice and a right to object and leave without charge. |
| DSP-15.1 | Owner approval before production data enters test | No | No production customer data exists yet. The question applies when it does. |
| DSP-16.1 | Retention and deletion follow requirements | Planned | Decided - a deletion rule for what visitors send through Start, stated in the retention schedule, in force from the opening of greypillar.ai. Nothing is held yet. |
| DSP-17.1 | Sensitive data protected through its life | Planned | Designed (see DSP-05.1, DSP-10.1). Not built. |
| DSP-18.1 | Law-enforcement request procedure | No | Not in place and not yet designed. |
| DSP-19.1 | Physical data locations documented | No | Partly. The site holds no customer data. Providers hold request records and email: email runs on Google Workspace, and hosting and network providers log requests. Where Start will store requests is stated in the privacy notice (section 5). A complete record of every location is not written. |

## 11 GRC: Governance, risk and compliance {#grc}
> In plain words: Greypillar owns these. The accountable role is accountable.

| Question | Short question | Answer | Evidence or note |
|---|---|---|---|
| GRC-01.1 | Governance policies set by leadership | No | Not in place and not yet designed. |
| GRC-01.2 | Policies reviewed yearly | No | Not in place and not yet designed. |
| GRC-02.1 | Enterprise risk management programme | No | Not in place and not yet designed. |
| GRC-03.1 | Organisational policies reviewed yearly | No | Not in place and not yet designed. |
| GRC-04.1 | Policy exception process | No | Not in place and not yet designed. |
| GRC-05.1 | Information security programme | No | This document is the first written statement. No programme exists. |
| GRC-06.1 | Governance roles defined | Planned | The founder is accountable. Agreements will name an accountable role per customer (/commitments). |
| GRC-07.1 | Applicable laws and standards identified | Planned | Partly done - Thai PDPA, GDPR Article 28 terms and SCCs Module 2, Thai Civil and Commercial Code section 373, Delaware law. Not a legal opinion; no full register. |
| GRC-07.2 | Requirements reviewed yearly | Planned | Follows the register. |
| GRC-08.1 | Contact with special interest groups | No | None kept. CSA STAR is the first programme to be applied to. |

## 12 HRS: Human resources {#hrs}
> In plain words: most of these questions apply when Greypillar engages someone with access to company data. Where nothing is written, the answer is No.

| Question | Short question | Answer | Evidence or note |
|---|---|---|---|
| HRS-01.1 | Background checks policy | Not applicable | The question concerns people Greypillar has engaged. It applies when Greypillar engages someone with access to company data. |
| HRS-01.2 | Checks follow local law | Not applicable | The question concerns people Greypillar has engaged. It applies when Greypillar engages someone with access to company data. |
| HRS-01.3 | Checks policy reviewed yearly | Not applicable | The question concerns people Greypillar has engaged. It applies when Greypillar engages someone with access to company data. |
| HRS-02.1 | Acceptable use of company assets | No | Not in place and not yet designed. |
| HRS-02.2 | Policy reviewed yearly | No | Not in place and not yet designed. |
| HRS-03.1 | Unattended workspaces conceal data | No | Not in place and not yet designed. |
| HRS-03.2 | Policy reviewed yearly | No | Not in place and not yet designed. |
| HRS-04.1 | Protection of data at remote sites | No | Not in place and not yet designed. |
| HRS-04.2 | Policy reviewed yearly | No | Not in place and not yet designed. |
| HRS-05.1 | Asset return at termination | Not applicable | The question concerns people Greypillar has engaged. It applies when Greypillar engages someone with access to company data. |
| HRS-06.1 | Roles when employment changes | Not applicable | The question concerns people Greypillar has engaged. It applies when Greypillar engages someone with access to company data. |
| HRS-07.1 | Employment agreement before access | Not applicable | The question concerns people Greypillar has engaged. It applies when Greypillar engages someone with access to company data. |
| HRS-08.1 | Agreement terms bind to security policies | Not applicable | The question concerns people Greypillar has engaged. It applies when Greypillar engages someone with access to company data. |
| HRS-09.1 | Security and privacy roles documented | Planned | See GRC-06.1. |
| HRS-10.1 | Confidentiality agreements | No | Not in place and not yet designed. |
| HRS-11.1 | Security awareness training programme | No | Not in place and not yet designed. |
| HRS-11.2 | Training updated regularly | No | Not in place and not yet designed. |
| HRS-12.1 | Training for people with sensitive data access | No | Not in place and not yet designed. |
| HRS-12.2 | Regular updates for those people | No | Not in place and not yet designed. |
| HRS-13.1 | People told their compliance duties | No | Not in place and not yet designed. |

## 13 IAM: Identity and access management {#iam}
> In plain words: The accountable role administers the accounts. Facts about sign-in are Greypillar's own statements and are not independently checked.

| Question | Short question | Answer | Evidence or note |
|---|---|---|---|
| IAM-01.1 | Identity and access policy | No | Not written. No decision to write it has been made. |
| IAM-01.2 | Policy reviewed yearly | No | Not written. No decision to write it has been made. |
| IAM-02.1 | Credential and password policy | No | Not written. No decision to write it has been made. |
| IAM-02.2 | Policy reviewed yearly | No | Not written. No decision to write it has been made. |
| IAM-03.1 | Inventory of identities and their access | No | Not in place and not yet designed. |
| IAM-04.1 | Separation of duties | No | The accountable role administers every account today. The product's gate separates who proposes from who accepts (/docs/gate-rule); that is designed, not running. |
| IAM-05.1 | Least privilege | Planned | Designed - secrets separated by project, services that read only their own, agents that cannot list secret values (GP-run infrastructure design, private; nothing deployed). Not deployed. |
| IAM-06.1 | Access provisioning process | No | Not in place and not yet designed. |
| IAM-07.1 | Timely removal or change of access | No | Not in place and not yet designed. |
| IAM-08.1 | Access reviews | No | Not in place and not yet designed. |
| IAM-09.1 | Privileged roles segregated | Planned | Designed (GP-run infrastructure design, private; nothing deployed). Not deployed. |
| IAM-10.1 | Privileged access granted for limited time | Planned | Designed - privileged approvals expire and are single-use (GP-run infrastructure design, private; nothing deployed). Not deployed. |
| IAM-10.2 | Privileged access not accumulated | Planned | Designed (GP-run infrastructure design, private; nothing deployed). Not deployed. |
| IAM-11.1 | Customers join approval of high-risk privileged access | Planned | Designed - nothing irreversible without the customer's yes (/commitments, /docs/gate-rule). Not running. |
| IAM-12.1 | Activity traceable to unique IDs | No | Not evidenced. |
| IAM-13.1 | Strong authentication incl. multi-factor | No | Partly. Greypillar states that passkeys or two-factor sign-in are on Google Workspace, GitHub, Vercel and Cloudflare. This is Greypillar's own statement of 12 November 2026, not independently verified. Greypillar does not claim passkeys or two-factor sign-in on any other account. One role administers every account. |
| IAM-13.2 | Certificates or equivalent for system identities | Planned | Designed - passkey (WebAuthn) signatures on approvals and a device identity for each system (GP-run infrastructure design, private; nothing deployed). Not deployed. |
| IAM-14.1 | Secure credential management | Planned | Designed - a secrets manager and a broker that injects credentials so a model never sees them (GP-run infrastructure design, private; nothing deployed). Not deployed. |
| IAM-15.1 | Access to data and functions verified as authorised | Planned | Designed - a credential is released only against a valid approval record (GP-run infrastructure design, private; nothing deployed). Not deployed. |

## 14 IPY: Interoperability and portability {#ipy}
> In plain words: There is no customer service to port data from yet.

| Question | Short question | Answer | Evidence or note |
|---|---|---|---|
| IPY-01.1 | Policy for API communications | Planned | The product's interface contract is specified (/docs/gate-rule). No customer API exists. |
| IPY-01.2 | Policy for processing interoperability | No | Not in place and not yet designed. |
| IPY-01.3 | Policy for development portability | No | Not in place and not yet designed. |
| IPY-01.4 | Policy for data exchange and portability | Planned | Commitment 4 (/commitments) - you leave with everything, in its native format. Planned, not in force. |
| IPY-01.5 | Policies reviewed yearly | No | Not in place and not yet designed. |
| IPY-02.1 | Customers can retrieve their data programmatically | Planned | Planned with the first callable interface. |
| IPY-03.1 | Secure protocols for data import and export | Planned | Planned with the first service. The website uses HTTPS only. |
| IPY-04.1 | Agreements cover data access at termination | Planned | Commitment 4 and the Common Paper terms are the base (/commitments). No agreement is in force. |

## 15 I&S: Infrastructure security {#is}
> In plain words: Shared with providers. Scope is the website; the intake was not deployed on 14 November 2026.

| Question | Short question | Answer | Evidence or note |
|---|---|---|---|
| I&S-01.1 | Infrastructure security policy | No | Not written. No decision to write it has been made. |
| I&S-01.2 | Policy reviewed yearly | No | Not written. No decision to write it has been made. |
| I&S-02.1 | Capacity planned and monitored | No | Not in place and not yet designed. |
| I&S-03.1 | Communications between environments monitored | No | Not in place and not yet designed. |
| I&S-03.2 | Communications between environments encrypted | No | Partly. Visitor connections to greypillar.ai use HTTPS only: plain HTTP redirects (308) and HSTS is set (max-age 63072000), observed 14 November 2026. The question is about communications between environments. Greypillar has no such environments yet, and it has not tested the links between providers. |
| I&S-03.3 | Connections limited to authenticated, authorised ones | Planned | Designed - private access for administration, an intake that has no open port to the internet, and one encrypted tunnel that requires a secret token for Start (GP-run infrastructure design, private; decision record). Not deployed on 14 November 2026. |
| I&S-03.4 | Network configuration reviewed yearly | No | Not in place and not yet designed. |
| I&S-03.5 | Allowed services and ports justified in writing | Planned | Designed - network zones and allowed connections are written as host code (GP-run infrastructure design, private; nothing deployed). Not deployed. |
| I&S-04.1 | Hosts and control planes hardened | No | Not in place and not yet designed. |
| I&S-05.1 | Production and non-production separated | No | Partly. Production (greypillar.ai, currently a holding page) and review builds are separate deployments by the hosting platform's default. No written rule separates them. No customer data exists in either. |
| I&S-05.2 | Production data sanitised before test use | No | No production customer data exists yet. The question applies when it does. |
| I&S-06.1 | Customers segmented from each other | Planned | Designed - each customer runs as its own installation with its own keys (/commitments, commitment 7). Not built. |
| I&S-07.1 | Secure channels for migrations to cloud | Not applicable | No customer migration occurs. |
| I&S-08.1 | High-risk environments identified | No | The Start intake is the one planned component that receives input from the public. No formal register. |
| I&S-09.1 | Defence in depth against network attacks | No | Cloudflare sits in front of the website (observed). No written design for defence in depth. |

## 16 LOG: Logging and monitoring {#log}
> In plain words: Greypillar has built no logging or monitoring. Providers keep their own logs, which were not reviewed.

| Question | Short question | Answer | Evidence or note |
|---|---|---|---|
| LOG-01.1 | Logging and monitoring policy | No | Not written. No decision to write it has been made. |
| LOG-01.2 | Policy reviewed yearly | No | Not written. No decision to write it has been made. |
| LOG-02.1 | Audit log security and retention | Planned | Designed - write-only collection into locked storage in a separate project, with a regular integrity check and metadata only (GP-run infrastructure design, private; nothing deployed). Not deployed. |
| LOG-03.1 | Security events monitored | No | Not in place and not yet designed. |
| LOG-03.2 | Alerts to responsible people | No | Not in place and not yet designed. |
| LOG-04.1 | Audit log access restricted and recorded | Planned | Same design. |
| LOG-05.1 | Logs correlated to detect anomalies | No | Not in place and not yet designed. |
| LOG-05.2 | Anomalies reviewed and acted on | No | Not in place and not yet designed. |
| LOG-06.1 | Reliable time source | No | Not assessed. Provider-managed. |
| LOG-07.1 | Logging requirements defined | No | Not in place and not yet designed. |
| LOG-07.2 | Logging scope reviewed yearly | No | Not in place and not yet designed. |
| LOG-08.1 | Customers can scrub sensitive data from logs | Planned | Designed - audit records hold metadata and fingerprints, never content (GP-run infrastructure design, private; nothing deployed). Not deployed. |
| LOG-09.1 | Audit records contain security information | Planned | Designed - every allow, hold, decline and block is recorded with a reason (GP-run infrastructure design, private; nothing deployed). Not deployed. |
| LOG-10.1 | Audit records protected from change | Planned | Designed - locked, hash-chained storage (GP-run infrastructure design, private; nothing deployed). Not deployed. |
| LOG-11.1 | Reporting on cryptographic controls | No | Not in place and not yet designed. |
| LOG-12.1 | Key lifecycle events logged | Planned | Designed - broker decisions logged (GP-run infrastructure design, private; nothing deployed). Not deployed. |
| LOG-13.1 | Physical access logged | Not applicable | Greypillar operates no data centre, office or other facility. Facilities belong to its providers and were not assessed by Greypillar. |
| LOG-14.1 | Monitoring failures reported | Planned | Designed - a backup alarm and non-AI tripwires outside the agents' control (GP-run infrastructure design, private; nothing deployed). Not deployed. |
| LOG-14.2 | Accountable people told at once | Planned | Same design - alerts to the accountable role. |

## 17 SEF: Security incident management {#sef}
> In plain words: Greypillar owns these. No incident process is written yet.

| Question | Short question | Answer | Evidence or note |
|---|---|---|---|
| SEF-01.1 | Incident management policy | Planned | As of 14 November 2026, security@greypillar.ai receives mail and a person reads it (tested 14 November 2026). The vulnerability disclosure policy (/legal/vulnerability-disclosure) takes effect on the opening of greypillar.ai. No incident management policy is written. |
| SEF-01.2 | Policy reviewed yearly | Planned | Follows the policy; first review 12 months after it takes effect. |
| SEF-02.1 | Timely incident handling policy | No | Partly. A short plan is stated in /security section 9. It has not been tested and is not a written policy. |
| SEF-02.2 | Policy reviewed yearly | No | Not in place and not yet designed. |
| SEF-03.1 | Incident response plan with communications | No | Partly. A short plan, with who is told and when, is stated in /security section 9. It has not been tested and is not a full response plan. |
| SEF-04.1 | Incident plans tested | No | Not in place and not yet designed. |
| SEF-05.1 | Incident metrics | No | Not in place and not yet designed. |
| SEF-06.1 | Event triage | No | Not in place and not yet designed. |
| SEF-07.1 | Response by category and severity | No | Not in place and not yet designed. |
| SEF-07.2 | Response procedures tested yearly | No | Not in place and not yet designed. |
| SEF-08.1 | Breach notification process | Planned | Partly. /security section 9 states the duties and the timeline: the Thai Personal Data Protection Committee without delay and within 72 hours where feasible, and affected people where the risk is high. No procedure is written or exercised. |
| SEF-08.2 | Material breaches reported as required | Planned | Same. |
| SEF-09.1 | Secure repository of incident records | No | Not in place and not yet designed. |
| SEF-09.2 | Incident records reviewed for causes | No | Not in place and not yet designed. |
| SEF-10.1 | Contacts for authorities | No | Not in place and not yet designed. |
| SEF-10.2 | Contacts reviewed yearly | No | Not in place and not yet designed. |

## 18 STA: Supply chain management, transparency and accountability {#sta}
> In plain words: Greypillar owns these. Its supply chain is a short list of providers.

| Question | Short question | Answer | Evidence or note |
|---|---|---|---|
| STA-01.1 | Supply chain risk policy | Planned | Designed for GP-run systems - pinned versions, a delay on routine upgrades, a watcher for advisories (GP-run infrastructure design, private; nothing deployed). Not deployed. |
| STA-01.2 | Policy reviewed yearly | No | Not in place and not yet designed. |
| STA-02.1 | Shared security responsibility policy | Planned | The security overview (/security) will carry a shared-responsibility table across the four places work runs (decision record). Draft. |
| STA-02.2 | Policy reviewed yearly | Planned | Follows the overview. |
| STA-03.1 | Shared responsibility applied through the supply chain | Planned | Same. |
| STA-04.1 | Customers get shared-responsibility guidance | Planned | Same - /security. |
| STA-05.1 | Ownership of each CCM control delineated | Planned | Domain-level notes in this document only. A per-control table comes with the first service. |
| STA-06.1 | Shared responsibility documentation reviewed | No | Not in place and not yet designed. |
| STA-07.1 | Own part of the model implemented and assessed | No | Not in place and not yet designed. |
| STA-08.1 | Inventory of supply chain relationships | No | Partly. The public table at /trust/subprocessors lists the providers Greypillar uses, in draft. A maintained inventory with owners and review dates is not evidenced. |
| STA-09.1 | Bill of materials for the service | No | Partly. The website's dependencies are pinned by lockfile and installed frozen in CI. No bill of materials is produced. |
| STA-09.2 | Bill reviewed yearly | No | Not in place and not yet designed. |
| STA-10.1 | Supply chain risk factors reviewed | No | Not in place and not yet designed. |
| STA-11.1 | Agreements carry the listed provisions | Planned | The Common Paper family is the base, with GP's terms as named overrides (decision record). Terms, DPA and acceptable use are in progress; none is in force. |
| STA-12.1 | Supply chain agreements reviewed yearly | No | Not in place and not yet designed. |
| STA-13.1 | Internal assessments of conformance yearly | No | This document is the first. |
| STA-14.1 | Providers required to meet security duties | No | Greypillar uses providers' standard terms. No supplementary security terms. |
| STA-15.1 | Providers' governance reviewed yearly | No | Not in place and not yet designed. |
| STA-16.1 | Risk-based supply chain assessments | No | Not in place and not yet designed. |

## 19 TVM: Threat and vulnerability management {#tvm}
> In plain words: Greypillar owns these for the website code.

| Question | Short question | Answer | Evidence or note |
|---|---|---|---|
| TVM-01.1 | Vulnerability and threat policy | Planned | As of 14 November 2026 a vulnerability disclosure policy is written and takes effect on the opening of greypillar.ai. It is not a threat policy. |
| TVM-01.2 | Policy reviewed yearly | Planned | Follows the policy; first review 12 months after it takes effect. |
| TVM-02.1 | Malware protection policy | No | Not in place and not yet designed. |
| TVM-02.2 | Policy reviewed yearly | No | Not in place and not yet designed. |
| TVM-03.1 | Vulnerability scanning at least monthly | No | No scan is run on a monthly schedule. Weekly Dependabot update pull requests are configured. They are not a scan. |
| TVM-04.1 | Threat analysis process | Planned | A ranked threat list exists for GP-run systems (GP-run infrastructure design, private; nothing deployed). None exists for the website or the product. |
| TVM-04.2 | Threat models for mitigation | Planned | Same. |
| TVM-05.1 | Detection tools updated weekly | No | Not in place and not yet designed. |
| TVM-06.1 | Updates for third-party and open-source libraries | Yes | Website only. Dependabot proposes npm and GitHub Actions updates weekly; dependencies are pinned by lockfile. Evidence - the website repository's dependabot.yml (private repository). |
| TVM-07.1 | Independent penetration testing | Planned | Decided trigger - a penetration test when hosted service begins (decision record, private). None done. |
| TVM-08.1 | Remediation schedule | No | Not in place and not yet designed. |
| TVM-09.1 | Prioritisation by risk framework | No | Not in place and not yet designed. |
| TVM-10.1 | Threat response by risk framework | No | Not in place and not yet designed. |
| TVM-11.1 | Vulnerability reporting with notification | No | Not in place and not yet designed. |
| TVM-12.1 | Vulnerability metrics | No | Not in place and not yet designed. |

## 20 UEM: Universal endpoint management {#uem}
> In plain words: Greypillar owns these. The endpoints are the devices the accountable role uses.

| Question | Short question | Answer | Evidence or note |
|---|---|---|---|
| UEM-01.1 | Endpoint policy | No | Not assessed. The accountable role uses its own devices; none of this is evidenced for this assessment. |
| UEM-01.2 | Policy reviewed yearly | No | Not assessed. The accountable role uses its own devices; none of this is evidenced for this assessment. |
| UEM-02.1 | Approved applications and sources | No | Not assessed. The accountable role uses its own devices; none of this is evidenced for this assessment. |
| UEM-03.1 | Endpoint compatibility validation | No | Not assessed. The accountable role uses its own devices; none of this is evidenced for this assessment. |
| UEM-04.1 | Endpoint inventory | No | Not assessed. The accountable role uses its own devices; none of this is evidenced for this assessment. |
| UEM-05.1 | Endpoint policy enforcement | No | Not assessed. The accountable role uses its own devices; none of this is evidenced for this assessment. |
| UEM-06.1 | Automatic lock screen | No | Not assessed. The accountable role uses its own devices; none of this is evidenced for this assessment. |
| UEM-07.1 | Endpoint OS changes under change management | No | Not assessed. The accountable role uses its own devices; none of this is evidenced for this assessment. |
| UEM-08.1 | Storage encryption on endpoints | No | Not assessed. The accountable role uses its own devices; none of this is evidenced for this assessment. |
| UEM-09.1 | Anti-malware on endpoints | No | Not assessed. The accountable role uses its own devices; none of this is evidenced for this assessment. |
| UEM-10.1 | Software firewall on endpoints | No | Not assessed. The accountable role uses its own devices; none of this is evidenced for this assessment. |
| UEM-11.1 | Data loss prevention on endpoints | No | Not assessed. The accountable role uses its own devices; none of this is evidenced for this assessment. |
| UEM-12.1 | Remote locate on mobile endpoints | Not applicable | No managed mobile endpoints. |
| UEM-13.1 | Remote wipe of company data | No | Not assessed. The accountable role uses its own devices; none of this is evidenced for this assessment. |
| UEM-14.1 | Security of third-party endpoints | Not applicable | No third party has endpoint access to company data. |

## 21 Submission state {#submission status=not_yet}
> In plain words: nothing has been sent to the Cloud Security Alliance.

21.1 Not submitted to the CSA STAR Registry. Greypillar may submit. After that, the registry entry will be linked here and this page will say Level 1, self-assessed, never a certification or a listing by the CSA of Greypillar's controls.
21.2 No audit or certification is held or claimed. Paid assurance starts on its triggers: insurance before the first pilot, a penetration test with hosted service, SOC 2 or ISO when the first enterprise asks.
