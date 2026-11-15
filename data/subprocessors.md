---
slug: subprocessors
path: /trust/subprocessors
group: Data
audience: Everyone
kind: Data
legal: true
title: Subprocessors
summary: The companies that handle personal information for Greypillar, what each does, what it handles, where, and on what terms. Each section has its plain meaning in the margin. If the two differ, the clause governs.
banner: ""
record:
  Version: "1.1"
  State: In force
  Effective: On the opening of greypillar.ai
  Updated: 15 November 2026
  Reviewed: Written by Greypillar. Not yet reviewed by outside counsel.
  Governing text: English
changes:
  - {version: "1.1", date: "15 November 2026", text: "PostHog runs only outside the EU, the EEA, the UK and Switzerland."}
  - {version: "1.0", date: "14 November 2026", text: "First published version, in force from the opening of greypillar.ai."}
sources:
  - {n: 1, text: "Vercel Data Processing Addendum (Vercel Inc., Delaware, 440 N Barranca Ave #4133, Covina, CA, SCCs Modules 1–3 and the UK IDTA)", href: "https://vercel.com/legal/dpa"}
  - {n: 2, text: "Vercel, Is Vercel certified under DPF?", href: "https://vercel.com/kb/guide/is-vercel-certified-under-dpf"}
  - {n: 3, text: "Cloudflare Customer Data Processing Addendum (Cloudflare, Inc., 101 Townsend Street, San Francisco, SCCs, UK Addendum, DPF)", href: "https://www.cloudflare.com/cloudflare-customer-dpa/"}
  - {n: 4, text: "Google Cloud Data Processing Addendum, covering Google Workspace (SCCs)", href: "https://cloud.google.com/terms/data-processing-addendum/"}
  - {n: 5, text: "Google Cloud, Alternative Transfer Solution (Google LLC certified to the EU-U.S. Data Privacy Framework)", href: "https://cloud.google.com/terms/alternative-transfer-solution"}
  - {n: 6, text: "Hetzner Online GmbH, legal notice (Industriestr. 25, 91710 Gunzenhausen, Germany)", href: "https://www.hetzner.com/legal/imprint/"}
  - {n: 7, text: "Hetzner, Data protection at Hetzner (data stays in the chosen location)", href: "https://docs.hetzner.com/general/company-and-policy/data-protection-at-hetzner"}
  - {n: 8, text: "PostHog Data Processing Agreement (PostHog, Inc., 2261 Market St., #4008, San Francisco, SCCs Module 2, DPF participation, clause 10.3). Read from the page's source in PostHog's public website repository", href: "https://posthog.com/dpa"}
  - {n: 9, text: "PostHog, GDPR compliance (EU cloud hosted in Frankfurt)", href: "https://posthog.com/docs/privacy/gdpr-compliance"}
  - {n: 10, text: "OpenRouter Terms of Service (OpenRouter, Inc., 169 Madison Avenue, New York)", href: "https://openrouter.ai/terms"}
  - {n: 11, text: "OpenRouter Privacy Policy (standard contractual clauses for transfers, no training on inputs or outputs by OpenRouter)", href: "https://openrouter.ai/privacy"}
  - {n: 12, text: "OpenRouter, Zero Data Retention", href: "https://openrouter.ai/docs/features/zdr"}
  - {n: 13, text: "Stripe Privacy Center (mechanism read: service-provider list kept apart from the policy)", href: "https://stripe.com/privacy-center/legal"}
---

## 1 What this list is {#scope status=live until=opening}

> In plain words: every company that handles personal information for us is named here, with what it handles and where.

1.1 This list names every company that handles personal information on Greypillar's behalf today (section 2), and those announced for when Start opens and analytics is switched on (section 3). Each acts only on Greypillar's instructions, under data protection terms. A company announced for later handles nothing until Greypillar has accepted its terms.

1.2 {claim:status.public_service} {claim:status.customers} No customer data is processed yet. Greypillar will not process customer personal data, in any market, until its insurance is in place. When the first customer agreement is signed, this list also becomes the list of subprocessors under that agreement.

## 1 What this list is {#scope opens=opening status=live}

> In plain words: every company that handles personal information for us is named here, with what it handles and where.

1.1 This list names every company that handles personal information on Greypillar's behalf: for the website and email (section 2), and for Start and analytics (section 3). Each acts only on Greypillar's instructions, under data protection terms. A company announced for later handles nothing until Greypillar has accepted its terms.

1.2 {claim:status.public_service} {claim:status.customers} No customer data is processed yet. Greypillar will not process customer personal data, in any market, until its insurance is in place. When the first customer agreement is signed, this list also becomes the list of subprocessors under that agreement.

## 2 Current subprocessors {#current status=live}

> In plain words: three companies today: hosting, the network, and email.

2.1 Greypillar uses these subprocessors today.

Table: Subprocessors in use

| Name | What they do | Data | Where |
|---|---|---|---|
| Vercel Inc. | Serves the website and runs its server function. When Start opens, that function passes Start requests to Greypillar's intake server | Network and request records (IP address, browser type, address requested). When Start opens, Start requests in transit | Global edge network. The server function runs in the United States. Company in the United States[^1] |
| Cloudflare, Inc. | DNS and the network in front of the website. When Start opens, also the encrypted tunnel to Greypillar's intake server and the bot check (Turnstile) on the Start form | Network and request records. All traffic to the site, and, when Start opens, Start requests in transit, and the IP address and browser signals the bot check reads | Global network. Company in the United States[^3] |
| Google (Google Workspace) | Email for greypillar.ai and, when Start opens, the copy of each Start request | Email you send us and, when Start opens, copies of Start requests | Google's data centres. Google LLC is a company in the United States[^4] |

## 3 Announced: when Start opens and analytics is switched on {#announced status=planned until=opening}

> In plain words: three more companies, published here before they handle anything. Hetzner stores Start requests in Helsinki, PostHog holds analytics in Frankfurt, OpenRouter would route requests to AI models later.

3.1 These subprocessors handle nothing today. The notice date is the day these texts are first published at github.com/Greypillar/policies. Hetzner and PostHog start no sooner than 30 days after that day. OpenRouter starts only as 3.2 says.

Table: Subprocessors announced

| Name | What they will do | Data | Where |
|---|---|---|---|
| Hetzner Online GmbH | Hosts Greypillar's intake server, which stores Start requests | Start requests: words, files, name and work email | Helsinki, Finland. Company in Germany[^6][^7] |
| PostHog, Inc. | Website analytics, outside the EU, the EEA, the UK and Switzerland only: it counts pages without cookies. Session replay and heatmaps only for visitors who say yes | Page events. Recordings of page use, with text fields masked, for visitors who say yes | EU cloud in Frankfurt, Germany. Company in the United States[^8][^9] |
| OpenRouter, Inc. | Would route agents' requests to AI models, only after agents begin to prepare briefs, which Start does not do when it opens | The text of a Start request and text read from its file, while a brief is prepared. OpenRouter keeps token counts and timing, not the text | Company in the United States. The model providers and their countries are not yet named. They are named here, or in the Order Form for customer work, before any use[^10][^12] |

3.2 OpenRouter passes each request to one AI model provider. Before any use, Greypillar names the providers and their countries on this list or in the Order Form. It will then set its account to route only to those providers, and only to those with zero data retention, which OpenRouter defines as no routine storage after processing. OpenRouter states one exception, content flagged as possible child sexual abuse material, which may be kept for review. OpenRouter also screens content in flight[^12].

## 3 For Start and analytics {#announced opens=opening status=live}

> In plain words: Hetzner stores Start requests in Helsinki and PostHog holds analytics in Frankfurt. OpenRouter is announced for later and handles nothing yet.

3.1 These two subprocessors handle Start requests and analytics.

Table: Subprocessors for Start and analytics

| Name | What they do | Data | Where |
|---|---|---|---|
| Hetzner Online GmbH | Hosts Greypillar's intake server, which stores Start requests | Start requests: words, files, name and work email | Helsinki, Finland. Company in Germany[^6][^7] |
| PostHog, Inc. | Website analytics, outside the EU, the EEA, the UK and Switzerland only: it counts pages without cookies. Session replay and heatmaps only for visitors who say yes | Page events. Recordings of page use, with text fields masked, for visitors who say yes | EU cloud in Frankfurt, Germany. Company in the United States[^8][^9] |

3.2 OpenRouter, Inc. is announced and handles nothing yet. It would route agents' requests to AI models, only after agents begin to prepare briefs, which Start does not do. The notice date is the day these texts are first published at github.com/Greypillar/policies, and OpenRouter does not start less than 30 days after the day its use is announced here. Before any use, Greypillar names the model providers and their countries on this list or in the Order Form. It will then set its account to route only to those providers, and only to those with zero data retention, which OpenRouter defines as no routine storage after processing. OpenRouter states one exception, content flagged as possible child sexual abuse material, which may be kept for review. OpenRouter also screens content in flight[^12].

## 4 Terms and transfer basis {#terms status=live}

> In plain words: each company is bound by data protection terms. For data from Europe, each US company uses the EU's standard clauses, and most also the Data Privacy Framework.

4.1 This table states the published terms each provider offers and the basis each states for transfers of personal information from the EU, the UK or Switzerland. For a provider not yet in use, Greypillar accepts its terms before it handles anything.

Table: Terms and transfer basis

| Name | Data protection terms | Transfer basis stated by the provider |
|---|---|---|
| Vercel Inc. | Vercel Data Processing Addendum | EU standard contractual clauses (Modules 1 to 3) and the UK addendum[^1]. Vercel states it is certified under the EU-U.S. Data Privacy Framework[^2] |
| Cloudflare, Inc. | Cloudflare Customer Data Processing Addendum | EU standard contractual clauses (Modules 2 and 3), the UK addendum and the Data Privacy Framework[^3] |
| Google (the company named in Greypillar's Workspace terms) | Cloud Data Processing Addendum, which covers Google Workspace | EU standard contractual clauses[^4]. Google LLC is certified under the EU-U.S. Data Privacy Framework[^5] |
| Hetzner Online GmbH | Hetzner's data processing agreement | No transfer out of the EU. The data stays in the EU location chosen[^7]. For information from Thailand, see 4.2 |
| PostHog, Inc. | PostHog Data Processing Agreement | EU standard contractual clauses (Module 2), and participation in the EU-U.S. Data Privacy Framework, its UK extension and the Swiss-U.S. framework[^8] |
| OpenRouter, Inc. | OpenRouter's data processing agreement, referred to in its privacy policy | EU standard contractual clauses[^11] |

4.2 For transfers out of Thailand, Greypillar relies on these same terms as safeguards, as set out in the [privacy notice](/legal/privacy). Storing a Start request in Finland is a transfer out of Thailand, and Hetzner's terms do not carry transfer clauses. For that transfer Greypillar relies on section 28(3) of the PDPA, because it is needed to take the steps the sender asks for.

4.3 Each AI model provider that sees a request is named on this list, or in the Order Form for customer work, with its country, before its first use. OpenRouter's own terms do not name them.

## 5 Not on this list {#not-listed status=live}

> In plain words: some companies we use never touch your personal information. They are named here so the list is complete.

5.1 GitHub, Inc. hosts the code of the website, and hosts github.com/Greypillar/policies, the public repository for these documents. It holds no personal information of visitors or of people who use Start.

5.2 Professional advisers and authorities may receive personal information in the cases set out in the [privacy notice](/legal/privacy). They are not subprocessors.

## 6 Changes to this list {#changes status=live until=opening}

> In plain words: a new company is announced here 30 days before it handles your information.

6.1 Greypillar publishes a new subprocessor on this list at least 30 days before it handles personal information. The entry gives its name, what it does, what it handles and where. The day the entry is first published at github.com/Greypillar/policies is the notice date.

6.2 There is no exception to the 30 days for an emergency. A change needed to keep the service running or secure waits for the notice period like any other.

6.3 You can follow changes in the changes feed on [Trust](/trust), which offers an Atom feed. Email notice will start with the first customer agreement.

6.4 Greypillar works from Thailand. Customer data and Start requests are read only from Thailand; a new place for them is announced here at least 30 days ahead, like a new subprocessor.

## 6 Changes to this list {#changes opens=opening status=live}

> In plain words: a new company is announced here 30 days before it handles your information.

6.1 Greypillar publishes a new subprocessor on this list at least 30 days before it handles personal information. The entry gives its name, what it does, what it handles and where. The day the entry is first published at github.com/Greypillar/policies is the notice date.

6.2 There is no exception to the 30 days for an emergency. A change needed to keep the service running or secure waits for the notice period like any other.

6.3 You can follow changes in the changes feed on [Trust](/trust), which offers an Atom feed, and in the history of github.com/Greypillar/policies. Email notice will start with the first customer agreement.

6.4 Greypillar works from Thailand. Customer data and Start requests are read only from Thailand; a new place for them is announced here at least 30 days ahead, like a new subprocessor.

## 7 Objecting to a new subprocessor {#objection status=planned}

> In plain words: once customer agreements exist, a customer can object to a new subprocessor and leave without charge.

7.1 There are no customer agreements yet. When there are, a customer may object to a new subprocessor during the 30-day notice. If Greypillar cannot meet the objection, the customer may end the affected service without charge and gets back what it prepaid for the period after the service ends.

7.2 Until then, anyone may write to {claim:channel.email} with an objection or a question about this list.
