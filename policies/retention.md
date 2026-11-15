---
slug: retention
path: /legal/retention
group: Policies
audience: Everyone
kind: Legal
legal: true
title: Retention and deletion
summary: How long Greypillar keeps each kind of record, what happens at the end, and how to ask for deletion sooner. Each section has its plain meaning in the margin. If the two differ, the clause governs.
banner: ""
record:
  Version: "1.0"
  State: In force
  Effective: On the opening of greypillar.ai
  Updated: 14 November 2026
  Reviewed: Written by Greypillar. Not yet reviewed by outside counsel.
  Governing text: English
changes:
  - {version: "1.0", date: "14 November 2026", text: "First published version, in force from the opening of greypillar.ai."}
sources:
  - {n: 1, text: "Personal Data Protection Act B.E. 2562 (2019), unofficial English translation (KMUTT copy), sections 33, 34 and 37(3)", href: "https://cc.kmutt.ac.th/Files/Act%20Eng/personal-data-protection-act-2019-en.pdf"}
  - {n: 2, text: "PostHog, Replay recording retention", href: "https://posthog.com/docs/session-replay/recording-retention"}
  - {n: 3, text: "Vercel, Runtime logs: retention by plan", href: "https://vercel.com/docs/logs/runtime"}
  - {n: 4, text: "OpenRouter, Data collection", href: "https://openrouter.ai/docs/guides/privacy/data-collection"}
  - {n: 5, text: "OpenRouter, Zero Data Retention", href: "https://openrouter.ai/docs/features/zdr"}
---

## 1 The rule {#rule status=live}

> In plain words: we keep each record only as long as its purpose needs, then delete it.

1.1 Greypillar keeps personal information only as long as the purpose it was collected for needs it, then deletes it or makes it anonymous. The [privacy notice](/legal/privacy) states each purpose.

1.2 "Delete" means removed from our systems so that it cannot be read back, and a request is sent to any provider holding a copy for us to do the same.

1.3 "Last contact" means the date of the last message we received from you.

## 2 How long each record is kept {#schedule status=live}

> In plain words: this table is the schedule for what we hold today. Section 3 adds Start and analytics, when they open.

2.1 We keep each kind of record we hold today for the period in this table.

Table: Retention schedule

| Record | Where | Kept | At the end |
|---|---|---|---|
| Email to {claim:channel.email} that is not a Start request | Google Workspace | 12 months after last contact | Deleted by hand. See 2.3 |
| Hosting and network logs | Vercel and Cloudflare | The provider's standard period. The runtime logs Vercel shows us are kept for 1 day on Vercel's Pro plan[^3] | Deleted by the provider |
| Security reports and their correspondence | Google Workspace | 24 months after the report is closed | Deleted by hand. See 2.3 |
| The light level and other settings in your browser | Your browser only | Until you clear them | You control them. See [Cookies](/legal/cookies) |

2.2 We do not export or copy hosting and network logs into our own systems. We cannot delete the providers' own logs sooner than their standard period. Where a provider keeps a record longer than the period above, its period is the one that applies to that copy.

2.3 Google Workspace does not delete mail for us on these periods. A person at Greypillar deletes mail and security reports by hand when their period ends. An automatic routine is planned.

## 3 When Start opens and analytics is switched on {#schedule-opening status=planned until=opening}

> In plain words: Start is not open and analytics is not switched on yet. When they are, their records follow this table.

3.1 Start is not open yet and analytics is not switched on, so none of these records exist today. From the day each opens, we keep its records for the period in this table.

Table: Retention schedule for Start and analytics

| Record | Where | Kept | At the end |
|---|---|---|---|
| What you send through Start: words, file, name and work email | Greypillar's intake server, in Helsinki | {claim:data_use.retention_start} | Deleted |
| The copy of a Start request in our mailbox | Google Workspace | The same period as the server copy | Deleted by hand on the same day |
| Our replies to a Start request | Google Workspace | 12 months after last contact | Deleted by hand. See 2.3 |
| "Tell me when my workspace can open": your name, email and that you asked | Greypillar's intake server, in Helsinki | Until you take back your consent, or until we have sent that message. You can take back this consent without deleting your Start request | Deleted. The request stays, if you have one, until its own period ends |
| The bot check result and its IP address | Cloudflare | The provider's standard period. We do not keep it ourselves | Deleted by the provider |
| Session replays and heatmaps, only with your yes | PostHog EU cloud, Frankfurt | 30 days[^2] | Deleted by PostHog |
| Aggregate analytics events | PostHog EU cloud, Frankfurt | 12 months | Deleted by PostHog |

3.2 Agents do not prepare briefs when Start opens, so there is no brief to keep. If they begin, this section will say where briefs are kept and for how long, at least 30 days before. Requests sent to an AI model would not be kept after processing, with one exception: OpenRouter states that content flagged as possible child sexual abuse material may be kept for review. OpenRouter keeps token counts and timing, not the text[^4][^5]. We cannot delete what a provider keeps under that exception.

## 3 Start and analytics {#schedule-opening opens=opening status=live}

> In plain words: Start requests are kept for your workspace, then deleted. Analytics follows its own periods.

3.1 We keep the records of Start and of analytics for the period in this table.

Table: Retention schedule for Start and analytics

| Record | Where | Kept | At the end |
|---|---|---|---|
| What you send through Start: words, file, name and work email | Greypillar's intake server, in Helsinki | {claim:data_use.retention_start} | Deleted |
| The copy of a Start request in our mailbox | Google Workspace | The same period as the server copy | Deleted by hand on the same day |
| Our replies to a Start request | Google Workspace | 12 months after last contact | Deleted by hand. See 2.3 |
| "Tell me when my workspace can open": your name, email and that you asked | Greypillar's intake server, in Helsinki | Until you take back your consent, or until we have sent that message. You can take back this consent without deleting your Start request | Deleted. The request stays, if you have one, until its own period ends |
| The bot check result and its IP address | Cloudflare | The provider's standard period. We do not keep it ourselves | Deleted by the provider |
| Session replays and heatmaps, only with your yes | PostHog EU cloud, Frankfurt | 30 days[^2] | Deleted by PostHog |
| Aggregate analytics events | PostHog EU cloud, Frankfurt | 12 months | Deleted by PostHog |

3.2 Agents do not prepare briefs yet, so there is no brief to keep. If they begin, this section will say where briefs are kept and for how long, at least 30 days before. Requests sent to an AI model would not be kept after processing, with one exception: OpenRouter states that content flagged as possible child sexual abuse material may be kept for review. OpenRouter keeps token counts and timing, not the text[^4][^5]. We cannot delete what a provider keeps under that exception.

## 4 Deleting sooner {#sooner status=live}

> In plain words: ask, and we delete within 30 days, everywhere we hold it.

4.1 You can ask us to delete your information at any time by writing to {claim:channel.email}. We delete it from every place in sections 2 and 3 within 30 days and tell you when it is done. What a provider keeps under its own rules, such as network logs, we cannot delete sooner. Sections 2 and 3 say which records those are.

4.2 If we cannot find a record from what you give us, for example a session replay, we tell you and say what would help us find it.

## 5 Backups {#backups status=planned}

> In plain words: no backup holds Start material today. If that changes, the period will be stated here first.

5.1 No backup holds Start material today.

5.2 Before any backup holds it, we will state here how long backups are kept. A deleted record will then leave the backups when they expire, and will not be restored into use.

## 6 When we must keep something longer {#holds status=live}

> In plain words: the law or a legal claim can require us to keep a record. If so, we tell you, and we use it for nothing else.

6.1 We may keep a record beyond its period only where the law requires it, or where it is needed to establish, exercise or defend a legal claim[^1]. The PDPA (s.33 and s.37(3)) and the GDPR (Art. 17(3)) allow this.

6.2 While a record is kept for that reason, we use it only for that reason and restrict all other use. We delete it when the reason ends.

6.3 If this stops us deleting something you asked us to delete, we tell you why, unless the law forbids it.

## 7 Changes {#changes status=live until=opening}

> In plain words: a shorter period applies at once. A longer one is announced 30 days ahead.

7.1 A change that shortens a period applies when it is published. A change that lengthens a period is announced at least 30 days before it takes effect, and applies only to records collected after that.

7.2 Every change is dated and public in the changes feed on [Trust](/trust).

## 7 Changes {#changes opens=opening status=live}

> In plain words: a shorter period applies at once. A longer one is announced 30 days ahead.

7.1 A change that shortens a period applies when it is published. A change that lengthens a period is announced at least 30 days before it takes effect, and applies only to records collected after that.

7.2 Every change is dated and public in the changes feed on [Trust](/trust) and in the history of github.com/Greypillar/policies.

## 8 Language {#language status=live}

> In plain words: the English text governs.

8.1 {claim:language.governing}

8.2 No translation of this document is published yet.
