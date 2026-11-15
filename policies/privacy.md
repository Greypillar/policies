---
slug: privacy
path: /legal/privacy
group: Policies
audience: Everyone
kind: Legal
legal: true
title: Privacy notice
summary: How Greypillar handles personal information when you visit greypillar.ai, send a request through Start, or write to us. Each section has its plain meaning in the margin. If the two differ, the clause governs.
banner: ""
record:
  Version: "1.1"
  State: In force
  Effective: On the opening of greypillar.ai
  Updated: 15 November 2026
  Reviewed: Written by Greypillar. Not yet reviewed by outside counsel.
  Governing text: English
changes:
  - {version: "1.1", date: "15 November 2026", text: "No analytics for visitors in the EU, the EEA, the UK and Switzerland (6.2, the tables in 3 and 4); when a representative there is appointed (1.5)."}
  - {version: "1.0", date: "14 November 2026", text: "First published version, in force from the opening of greypillar.ai."}
sources:
  - {n: 1, text: "Personal Data Protection Act B.E. 2562 (2019), unofficial English translation (KMUTT copy)", href: "https://cc.kmutt.ac.th/Files/Act%20Eng/personal-data-protection-act-2019-en.pdf"}
  - {n: 2, text: "GDPR Article 27, representatives of controllers not established in the Union", href: "https://gdpr-info.eu/art-27-gdpr/"}
  - {n: 3, text: "PostHog, Controlling data collection: cookieless tracking", href: "https://posthog.com/docs/privacy/data-collection"}
  - {n: 4, text: "OpenRouter, Zero Data Retention", href: "https://openrouter.ai/docs/features/zdr"}
  - {n: 5, text: "OpenRouter, Data collection", href: "https://openrouter.ai/docs/guides/privacy/data-collection"}
  - {n: 6, text: "California Privacy Protection Agency, CCPA monetary thresholds", href: "https://cppa.ca.gov/regulations/cpi_adjustment.html"}
  - {n: 7, text: "GitHub General Privacy Statement (mechanisms read: per-purpose bases, 30-day notice of material change)", href: "https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement"}
  - {n: 8, text: "Anthropic Privacy Policy (mechanism read: legal bases as a purpose table)", href: "https://www.anthropic.com/legal/privacy"}
---

## 1 Who we are {#who status=live}

> In plain words: Greypillar LLC decides how your information is used. We work from Thailand.

1.1 This notice is from {claim:entity.legal_name} ("Greypillar", "we"). Greypillar is the controller of the personal information described here, under the Thai Personal Data Protection Act and, where it applies, the GDPR.

1.2 {claim:entity.address}

1.3 For anything in this notice, write to {claim:channel.email}. For security problems, write to security@greypillar.ai. The [vulnerability disclosure policy](/legal/vulnerability-disclosure) sets out what to expect.

1.4 Greypillar is run from Thailand. We treat the Thai Personal Data Protection Act B.E. 2562 (the PDPA) as applying in full to everything we do with personal information, wherever you are[^1].

1.5 Greypillar has not appointed a representative in the EU or the UK yet[^2]. It runs no analytics for visitors in the EU, the EEA, the UK or Switzerland and does not market there. It will appoint one before either changes, or before its first customer there. It has not appointed a data protection officer.

1.6 {claim:status.public_service} {claim:status.customers}

## 2 What this notice covers {#scope status=live}

> In plain words: this covers the website, the Start page and email to us. Customer contracts will come with their own data terms.

2.1 This notice covers personal information we handle when you visit greypillar.ai or one of its subdomains, send a request through [Start](/start), or write to us by email.

2.2 It does not cover information a customer gives us to process on its behalf under a contract. That will be governed by a data processing agreement, which is not yet published. Greypillar processes no customer personal data today. It will not do so, in any market, until its insurance is in place.

2.3 It does not cover other companies' websites, even where we link to them.

## 3 What we collect {#collect status=live until=opening}

> In plain words: little from visitors, and only what you choose to send through Start or email.

3.1 We collect the information in this table and nothing else. Rows marked "when" start only when that part of the site opens. Today the site has no analytics and Start is not open.

Table: What we collect

| From | What | How |
|---|---|---|
| Every visitor | IP address, browser and device type, the address requested, time, and response. These are network and server records | Created by our hosting and network providers when your browser asks for a page |
| Every visitor, when analytics is switched on | The country your network address is in, so the site knows whether to ask before it counts anything | Worked out when your browser asks for a page |
| Visitors outside the EU, the EEA, the UK and Switzerland, when analytics is switched on | Pages viewed, the site that sent you, how far you scrolled, where you left, the route from the home page to Start and Send. Nothing is stored in your browser | Measured by PostHog, in its EU cloud. See section 6 |
| Visitors who say yes to recording, when analytics is switched on | A recording of how the page was used: pointer movement, clicks, scrolling and the page's structure. What you type is masked and not recorded. Start is never recorded | Recorded by PostHog, only after you agree |
| Every visitor | The light level you chose. It stays in your browser and is never sent to us | Saved in your browser's local storage. See [Cookies](/legal/cookies) |
| People who use Start, when it opens | What you write, one file if you add one (with its name, type and size, and a checksum of its contents), your name and your work email | You send it when you press Send |
| People who use Start, when it opens | The result of a bot check, your IP address and signals from your browser, which Cloudflare reads | Cloudflare Turnstile runs on the Start page and when you press Send |
| People who ask to hear when their workspace can open, when Start opens | Your name and email, and that you asked | You tick a separate box |
| People who write to us | Your email address, your name if you give it, and what you write | You send it |

3.2 We do not ask for sensitive information, such as health, religion, criminal records or biometric data. Please do not include it in Start or in email. If it arrives, we delete it unless you ask us to keep it for your request.

3.3 We do not buy personal information, and we do not collect it from data brokers.

## 3 What we collect {#collect opens=opening status=live}

> In plain words: little from visitors, and only what you choose to send through Start or email.

3.1 We collect the information in this table and nothing else.

Table: What we collect

| From | What | How |
|---|---|---|
| Every visitor | IP address, browser and device type, the address requested, time, and response. These are network and server records | Created by our hosting and network providers when your browser asks for a page |
| Every visitor | The country your network address is in, so the site knows whether to ask before it counts anything | Worked out when your browser asks for a page |
| Visitors outside the EU, the EEA, the UK and Switzerland | Pages viewed, the site that sent you, how far you scrolled, where you left, the route from the home page to Start and Send. Nothing is stored in your browser. PostHog is set to discard the IP address | Measured by PostHog, in its EU cloud. See section 6 |
| Visitors who say yes to recording | A recording of how the page was used: pointer movement, clicks, scrolling and the page's structure. What you type is masked and not recorded. Start is never recorded | Recorded by PostHog, only after you agree |
| Every visitor | The light level you chose. It stays in your browser and is never sent to us | Saved in your browser's local storage. See [Cookies](/legal/cookies) |
| People who use Start | What you write, one file if you add one (with its name, type and size, and a checksum of its contents), your name and your work email | You send it when you press Send |
| People who use Start | The result of a bot check, your IP address and signals from your browser, which Cloudflare reads | Cloudflare Turnstile runs on the Start page and when you press Send |
| People who ask to hear when their workspace can open | Your name and email, and that you asked | You tick a separate box |
| People who write to us | Your email address, your name if you give it, and what you write | You send it |

3.2 We do not ask for sensitive information, such as health, religion, criminal records or biometric data. Please do not include it in Start or in email. If it arrives, we delete it unless you ask us to keep it for your request.

3.3 We do not buy personal information, and we do not collect it from data brokers.

## 4 Why we use it, and the legal ground {#why status=live}

> In plain words: each use has one reason and one legal ground. Where the ground is your consent, you can take it back.

4.1 We use personal information only for the purposes in this table, each on the ground shown.

Table: Purposes and legal grounds

| Purpose | Information | GDPR ground | PDPA ground |
|---|---|---|---|
| Serve the website, keep it running and protect it from abuse | Network and server records | Legitimate interests, Art. 6(1)(f). Our interest is a site that works and resists abuse | Legitimate interests, s.24(5) |
| Understand, in aggregate, how the site is used by visitors outside the EU, the EEA, the UK and Switzerland | Analytics without cookies | Legitimate interests, Art. 6(1)(f). Our interest is a site people can use | Legitimate interests, s.24(5) |
| Improve the website from recordings | Session replay and heatmaps | Consent, Art. 6(1)(a) | Consent, s.19 |
| Keep Start free of bots and abuse | The bot check result, IP address and browser signals | Legitimate interests, Art. 6(1)(f). Our interest is a form that works and resists abuse | Legitimate interests, s.24(5) |
| Answer a Start request | What you send through Start | Legitimate interests, Art. 6(1)(f), where you write for your employer or organisation. Our interest is answering the people who write to us. Steps you ask for before a contract, Art. 6(1)(b), where you write for yourself | s.24(5), or s.24(3) where you write for yourself |
| Keep a Start request so your workspace can begin from it | What you send through Start | Legitimate interests, Art. 6(1)(f), or steps you ask for before a contract, Art. 6(1)(b), as above. Our interest is letting your workspace begin from what you sent | s.24(5) or s.24(3), as above |
| Tell you when your workspace can open | Name and email | Consent, Art. 6(1)(a) | Consent, s.19 |
| Answer your email | What you write | Legitimate interests, Art. 6(1)(f), or steps you ask for, Art. 6(1)(b) | s.24(5) or s.24(3) |
| Meet a legal duty, such as tax records or a lawful order | What the duty requires | Legal obligation, Art. 6(1)(c) | Legal obligation, s.24(6) |
| Establish, exercise or defend a legal claim | What the claim concerns | Legitimate interests, Art. 6(1)(f) | Legitimate interests, s.24(5) |

4.2 Where the ground is legitimate interests, you may object, and section 11 says how.

4.3 We use information for a new purpose only if it fits the purpose it was collected for, or after we tell you and, where the law requires, ask you.

4.4 You do not have to send us anything. To answer a Start request we need your name and work email. Without them we cannot reply. Nothing else on the site needs information from you.

## 5 What will happen when you use Start {#start status=planned decides until=opening}

> In plain words: Start is not open yet. When it opens, your request is kept on our own server in Helsinki and a person reads it and replies.

5.1 Start is not open yet. This section applies from the day it opens. When you press Send, your request passes through our hosting and network providers to Greypillar's intake server, which Hetzner hosts for us in Helsinki. {claim:location.data_hosting}

5.2 A copy of your request is sent to our mailbox, {claim:channel.email}, on Google Workspace.

5.3 The intake service has no open port to the internet. Only the website's server function reaches it, through an encrypted Cloudflare tunnel that requires a secret token. The [security overview](/security) describes this.

5.4 You can add one file of up to 4 MB. It is stored as you sent it. It is never opened on the server that stores it.

5.5 A person at Greypillar reads what you send and replies. {claim:channel.reply_time}

5.6 Agents do not prepare briefs when Start opens. We plan that they will, and that a person will check each brief before anything reaches you. We will announce this here, at least 30 days ahead, with the model providers that would see your text, the countries they work in and what they keep. When it starts, requests to models would go through OpenRouter, set to route only to providers that neither train on them nor keep them after processing. OpenRouter calls this zero data retention[^4]. It states one exception, content flagged as possible child sexual abuse material, which may be kept for review. OpenRouter keeps records such as the number of tokens and the time taken, not the text[^5].

5.7 No agent sends anything to you alone.

5.8 {claim:data_use.retention_start} [Retention](/legal/retention) sets out the details.

5.9 {claim:data_use.no_training_default} This will hold for everything you send through Start.

## 5 What happens when you use Start {#start opens=opening status=live decides}

> In plain words: your request is kept on our own server in Helsinki. A person reads it and replies.

5.1 When you press Send, your request passes through our hosting and network providers to Greypillar's intake server, which Hetzner hosts for us in Helsinki. {claim:location.data_hosting}

5.2 A copy of your request is sent to our mailbox, {claim:channel.email}, on Google Workspace.

5.3 The intake service has no open port to the internet. Only the website's server function reaches it, through an encrypted Cloudflare tunnel that requires a secret token. The [security overview](/security) describes this.

5.4 You can add one file of up to 4 MB. It is stored as you sent it. It is never opened on the server that stores it.

5.5 A person at Greypillar reads what you send and replies. {claim:channel.reply_time}

5.6 Agents do not prepare briefs yet. We plan that they will, and that a person will check each brief before anything reaches you. We will announce this here, at least 30 days ahead, with the model providers that would see your text, the countries they work in and what they keep.

5.7 No agent sends anything to you alone.

5.8 {claim:data_use.retention_start} [Retention](/legal/retention) sets out the details.

## 6 Analytics and session replay, when switched on {#analytics status=planned until=opening}

> In plain words: analytics is not switched on yet. When it is, it will not run at all for visitors in Europe; elsewhere we record a visit only if you say yes, and we never record Start.

6.1 Analytics is not switched on yet. Today nothing is counted or recorded. When it is, we will use PostHog, in its EU cloud in Frankfurt, Germany, to understand how the site is used. PostHog will keep its identifier only in the page's memory. It stores nothing in your browser, and every full page load starts a new identifier, so we count pages and steps, not people[^3].

6.2 If your network address is in the EU, the EEA, the UK or Switzerland, or we cannot tell where you are, we will run no analytics at all: PostHog does not load, nothing is counted or recorded, and the site does not ask.

6.3 Everywhere else, we will count pages without cookies and without asking, because nothing is stored on your device. We record a visit only if you say yes.

6.4 We do not identify you in analytics. We do not link analytics to your name or email, including when you use Start.

6.5 Session replay and heatmaps run only if you say yes through the line on the site that asks. The line names PostHog, says that recordings are kept in the EU for 30 days, and links to the [Cookies](/legal/cookies) page. A recording stores nothing in your browser beyond your answer. A new page load starts a new recording.

6.6 Recordings mask every text field. What you type is not recorded. The Start form is blocked from recording, and the Start page is never recorded, whatever you chose.

6.7 You can take back your yes at any time on the [Cookies](/legal/cookies) page, which is linked at the foot of every page. Recording stops at once. Recordings already made are deleted when their keeping period ends, or sooner if you ask and we can find them.

6.8 Your answer, yes or no, lasts 6 months. After that the site asks again.

6.9 If your browser sends a Global Privacy Control or Do Not Track signal, we treat it as a no to session replay. Nothing is recorded and the site does not ask.

6.10 We use recordings only to improve the website. We do not use them to decide anything about you.

## 6 Analytics and session replay {#analytics opens=opening status=live}

> In plain words: analytics does not run at all for visitors in Europe. Elsewhere we record a visit only if you say yes, and never on Start.

6.1 We use PostHog, in its EU cloud in Frankfurt, Germany, to understand how the site is used. PostHog is set to discard the IP address before an event is stored. It keeps its identifier only in the page's memory. It stores nothing in your browser, and every full page load starts a new identifier, so we count pages and steps, not people[^3].

6.2 If your network address is in the EU, the EEA, the UK or Switzerland, or we cannot tell where you are, we run no analytics at all: PostHog does not load, nothing is counted or recorded, and the site does not ask.

6.3 Everywhere else, we count pages without cookies and without asking, because nothing is stored on your device. We record a visit only if you say yes.

6.4 We do not identify you in analytics. We do not link analytics to your name or email, including when you use Start.

6.5 Session replay and heatmaps run only if you say yes through the line on the site that asks. The line names PostHog, says that recordings are kept in the EU for 30 days, and links to the [Cookies](/legal/cookies) page. A recording stores nothing in your browser beyond your answer. A new page load starts a new recording.

6.6 Recordings mask every text field. What you type is not recorded. The Start form is blocked from recording, and the Start page is never recorded, whatever you chose.

6.7 You can take back your yes at any time on the [Cookies](/legal/cookies) page, which is linked at the foot of every page. Recording stops at once. Recordings already made are deleted when their keeping period ends, or sooner if you ask and we can find them.

6.8 Your answer, yes or no, lasts 6 months. After that the site asks again.

6.9 If your browser sends a Global Privacy Control or Do Not Track signal, we treat it as a no to session replay. Nothing is recorded and the site does not ask.

6.10 We use recordings only to improve the website. We do not use them to decide anything about you.

## 7 What we never do {#never status=live}

> In plain words: we do not sell your information or build a profile of you.

7.1 We do not sell personal information. We do not share it for advertising.

7.2 We do not build profiles of visitors, track you across other websites, or use advertising networks.

7.3 We make no decision about you by automated means alone that has legal or similarly significant effects. Where an agent prepares anything that affects you, a person decides.

## 8 Who else handles it {#others status=live}

> In plain words: a few companies help us run the site. The list names each one, what it handles and where, and which start only when Start and analytics open.

8.1 Companies that handle personal information for us are listed, with what each does, what it handles and where, in [Subprocessors](/trust/subprocessors). Each acts on our instructions under data protection terms. A company announced for later handles nothing until Greypillar has accepted its data protection terms.

8.2 We may also share information with professional advisers bound to confidentiality, or with an authority when the law requires it. When the law allows, we tell you first.

8.3 If Greypillar or its business is transferred to another company, personal information may pass with it. That company must keep the commitments in this notice, and we will tell you before it happens.

## 9 Transfers across borders {#transfers status=live until=opening}

> In plain words: your information passes through companies in the United States, and email is held by Google. Start and analytics add places in the EU when they open. We read Start requests only from Thailand.

9.1 Today, pages pass through the networks of Vercel and Cloudflare, which run worldwide, and the website's server function, which runs in the United States. Email is held by Google. When Start opens, its requests will be stored in Finland (section 5). When analytics is switched on, it will be stored in Germany (section 6).

9.2 Greypillar is run from Thailand. We read Start requests and customer data only from Thailand. If we ever do so from another place, we announce it here at least 30 days ahead.

9.3 For information from the EU, the UK or Switzerland, each provider in the United States uses data protection terms that include the European Commission's standard contractual clauses. Some also take part in the EU-U.S. Data Privacy Framework. [Subprocessors](/trust/subprocessors) states the basis for each. You can ask us for a copy of the safeguards that apply to your information by writing to {claim:channel.email}.

9.4 For transfers out of Thailand, we rely on the safeguards the PDPA allows under section 29 and the rules of the Personal Data Protection Committee, chiefly the providers' data protection terms. Storing a Start request in Finland is a transfer out of Thailand. We rely there on section 28(3), because the transfer is needed to take the steps you ask for[^1].

## 9 Transfers across borders {#transfers opens=opening status=live}

> In plain words: Start requests are stored in the EU and your information passes through companies in the United States. We read Start requests only from Thailand.

9.1 Start requests are stored in Finland. Analytics is stored in Germany. On the way, information passes through the networks of Vercel and Cloudflare, which run worldwide, and the website's server function, which runs in the United States. Email is held by Google.

9.2 Greypillar is run from Thailand. We read Start requests and customer data only from Thailand. If we ever do so from another place, we announce it here at least 30 days ahead.

9.3 For information from the EU, the UK or Switzerland, each provider in the United States uses data protection terms that include the European Commission's standard contractual clauses. Some also take part in the EU-U.S. Data Privacy Framework. [Subprocessors](/trust/subprocessors) states the basis for each. You can ask us for a copy of the safeguards that apply to your information by writing to {claim:channel.email}.

9.4 For transfers out of Thailand, we rely on the safeguards the PDPA allows under section 29 and the rules of the Personal Data Protection Committee, chiefly the providers' data protection terms. Storing a Start request in Finland is a transfer out of Thailand. We rely there on section 28(3), because the transfer is needed to take the steps you ask for[^1].

## 10 How long we keep it {#retention status=live until=opening}

> In plain words: each kind of record has its own period. Start requests, once Start opens, follow section 5.

10.1 What you send through Start, once it opens, is kept as section 5 sets out.

10.2 Each kind of record, its period and what happens at the end are set out in [Retention](/legal/retention).

10.3 We may keep information longer only where the law requires it, or where it is needed to establish, exercise or defend a legal claim. If that stops us deleting something you asked us to delete, we tell you why.

## 10 How long we keep it {#retention opens=opening status=live}

> In plain words: Start requests are kept for your workspace, then deleted. Each kind of record has its own period.

10.1 {claim:data_use.retention_start}

10.2 Each kind of record, its period and what happens at the end are set out in [Retention](/legal/retention).

10.3 We may keep information longer only where the law requires it, or where it is needed to establish, exercise or defend a legal claim. If that stops us deleting something you asked us to delete, we tell you why.

## 11 Your rights {#rights status=live}

> In plain words: you can see, copy, correct, move, limit or delete your information, object to its use, and take back consent. Write to us.

11.1 You can ask us to do any of the following.

- give you access to your personal information and a copy of it (PDPA s.30, GDPR Art. 15)
- send it to you, or to another organisation, in a common machine-readable form (PDPA s.31, GDPR Art. 20)
- correct it or complete it (PDPA s.35 and s.36, GDPR Art. 16)
- delete it (PDPA s.33, GDPR Art. 17)
- restrict its use (PDPA s.34, GDPR Art. 18)
- stop using it, where we rely on legitimate interests (PDPA s.32, GDPR Art. 21)

11.2 Where we rely on your consent, you can take it back at any time, as easily as you gave it. Taking it back does not make earlier use unlawful (PDPA s.19).

11.3 Write to {claim:channel.email}. We may ask you to confirm it is you, usually by writing from the email address we hold. Someone may ask on your behalf if they show that you authorised them.

11.4 We answer within 30 days. If we cannot do what you ask, we say why, and we record the refusal and its reason as the PDPA requires. Using your rights costs nothing.

11.5 You can complain to the Personal Data Protection Committee in Thailand (PDPA s.73). If you are in the EU, you can complain to the data protection authority where you live or work. If you are in the UK, you can complain to the Information Commissioner's Office. We would like the chance to put it right first, but you do not need to come to us before you complain.

## 12 United States state privacy laws {#us-states status=live}

> In plain words: most US state privacy laws do not reach a company of our size. You have the rights in section 11 anyway.

12.1 Most US state privacy laws apply only to businesses above thresholds that Greypillar does not meet today. For example, the California Consumer Privacy Act applies to a business with more than $26,625,000 in annual gross revenue, or to one that buys, sells or shares the personal information of 100,000 or more consumers or households, or earns half or more of its annual revenue from selling or sharing it[^6]. Greypillar meets none of these.

12.2 We give everyone the rights in section 11, wherever they live.

12.3 We do not sell or share personal information as those laws define selling and sharing. We do not use it for targeted advertising, and we do not use it for profiling that leads to decisions with legal or similarly significant effects.

## 13 How we protect it {#security status=live}

> In plain words: the security overview says which controls exist today and which do not.

13.1 We protect personal information with the controls described in the [security overview](/security). That page says which controls run today and which are planned.

13.2 If a breach of personal information is likely to put you at risk, we tell the Office of the Personal Data Protection Committee without delay, and within 72 hours of becoming aware of it where feasible. Where the risk to you is high, we also tell you without delay (PDPA s.37(4)). Where the GDPR applies, we follow its rules on notice (Art. 33 and 34).

## 14 Children {#children status=live}

> In plain words: Greypillar is for organisations and working adults.

14.1 The site and Start are meant for organisations and working adults. We do not knowingly collect personal information from children. If you believe a child has sent us information, write to {claim:channel.email} and we delete it.

## 15 When an agent writes to you {#agents status=planned}

> In plain words: if an AI agent wrote a message, the message says so and says who is responsible.

15.1 {claim:responsibility.agent_disclosure} The [AI disclosure](/legal/ai-disclosure) sets out the rule.

## 16 Changes to this notice {#changes status=live until=opening}

> In plain words: every change is dated and public. A material change is announced 30 days before it takes effect.

16.1 Each version of this notice has a number and an effective date. Every change is public in the changes feed on [Trust](/trust).

16.2 We announce a material change at least 30 days before it takes effect. A material change is one that widens what we collect, adds a purpose, adds a recipient of a new kind, adds a place from which we read your information, or reduces your rights.

16.3 A change never applies to information we already hold in a way that needs your consent, unless you give it.

## 16 Changes to this notice {#changes opens=opening status=live}

> In plain words: every change is dated and public. A material change is announced 30 days before it takes effect.

16.1 Each version of this notice has a number and an effective date. Every change is public in the changes feed on [Trust](/trust) and in the history of github.com/Greypillar/policies.

16.2 We announce a material change at least 30 days before it takes effect. A material change is one that widens what we collect, adds a purpose, adds a recipient of a new kind, adds a place from which we read your information, or reduces your rights.

16.3 A change never applies to information we already hold in a way that needs your consent, unless you give it.

## 17 Language {#language status=live}

> In plain words: the English text governs.

17.1 {claim:language.governing}

17.2 No translation of this notice is published yet.
