---
slug: cookies
path: /legal/cookies
group: Policies
audience: Everyone
kind: Legal
legal: true
title: Cookies and browser storage
summary: What greypillar.ai stores in your browser, why, for how long, and how to remove it. Without your yes, the site sets no cookies. Each section has its plain meaning in the margin. If the two differ, the clause governs.
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
  - {n: 1, text: "PostHog, Controlling data collection: cookieless tracking and what each mode stores", href: "https://posthog.com/docs/privacy/data-collection"}
  - {n: 2, text: "PostHog, JavaScript persistence options", href: "https://posthog.com/docs/libraries/js/persistence"}
  - {n: 3, text: "PostHog, Replay recording retention", href: "https://posthog.com/docs/session-replay/recording-retention"}
  - {n: 4, text: "Cloudflare, Turnstile Privacy Addendum", href: "https://www.cloudflare.com/turnstile-privacy-policy/"}
---

## 1 What this covers {#scope status=live}

> In plain words: this lists everything the site keeps in your browser.

1.1 This notice covers cookies, local storage and session storage that greypillar.ai and its subdomains use in your browser. The [privacy notice](/legal/privacy) covers everything else we do with personal information.

1.2 A cookie is a small file a site keeps in your browser and sends back with each request. Local storage and session storage are places in your browser where a page can keep a small setting. Session storage is cleared when you close the tab. Local storage stays until you clear it.

## 2 What is stored, and why {#stored status=live until=opening}

> In plain words: today, only the settings you choose. Section 4 adds what your answer about recording stores, once analytics is switched on.

2.1 Today the site stores only what is in this table.

Table: What the site stores in your browser

| Name | Kind | Set by | Purpose | Kept | Needs your yes |
|---|---|---|---|---|---|
| gp-site-light | Local storage | Greypillar | Remembers the light level you chose, so the next visit opens in it. Never sent to us | Until you clear it | No. It is set only when you choose a level |
| gp-docs-surface | Local storage | Greypillar | On documentation pages, remembers which of the tabs you last chose. Never sent to us | Until you clear it | No. It is set only when you choose a tab |

2.2 Nothing in this table is used for advertising, and no other company reads it through our site.

2.3 The Start page, when it opens, loads a bot check from Cloudflare (Turnstile). Cloudflare runs it. Our own storage is only what is in the table above. Turnstile runs in a frame served from Cloudflare's own address, so anything it keeps belongs to Cloudflare, not to this site. Cloudflare may set its own security cookies there to tell people from automated programs; they are needed for that check and for nothing else[^4].

## 2 What is stored, and why {#stored opens=opening status=live}

> In plain words: the settings you choose, and your answer about recording once you give it.

2.1 The site stores only what is in this table and in section 4.

Table: What the site stores in your browser

| Name | Kind | Set by | Purpose | Kept | Needs your yes |
|---|---|---|---|---|---|
| gp-site-light | Local storage | Greypillar | Remembers the light level you chose, so the next visit opens in it. Never sent to us | Until you clear it | No. It is set only when you choose a level |
| gp-docs-surface | Local storage | Greypillar | On documentation pages, remembers which of the tabs you last chose. Never sent to us | Until you clear it | No. It is set only when you choose a tab |

2.2 Nothing in this table is used for advertising, and no other company reads it through our site.

2.3 The Start page loads a bot check from Cloudflare (Turnstile). Cloudflare runs it. Our own storage is only what is in the table above. Turnstile runs in a frame served from Cloudflare's own address, so anything it keeps belongs to Cloudflare, not to this site. Cloudflare may set its own security cookies there to tell people from automated programs; they are needed for that check and for nothing else[^4].

## 3 Analytics, when switched on {#analytics status=planned until=opening}

> In plain words: analytics is not switched on yet. When it is, visitors in Europe are asked first. Elsewhere we count pages without storing anything in your browser.

3.1 Analytics is not switched on yet. When it is, PostHog will measure how the site is used while keeping its identifier only in the page's memory. It stores nothing in cookies, local storage or session storage, and every full page load starts a new identifier, so it counts pages and steps, not people[^1].

3.2 This layer does not record your screen and does not identify you.

3.3 If your network address is in the EU, the EEA, the UK or Switzerland, PostHog will load only after you say yes through the line the site shows. Before you answer, and if you say no, nothing is counted or recorded. If we cannot tell where you are, the site asks.

3.4 Everywhere else, we will count pages without asking. This relies on legitimate interests, because nothing is stored on your device.

## 3 Analytics {#analytics opens=opening status=live}

> In plain words: visitors in Europe are asked first. Elsewhere we count pages without storing anything in your browser.

3.1 PostHog measures how the site is used while keeping its identifier only in the page's memory. It stores nothing in cookies, local storage or session storage, and every full page load starts a new identifier, so it counts pages and steps, not people[^1]. PostHog is set to discard the IP address before an event is stored.

3.2 This layer does not record your screen and does not identify you.

3.3 If your network address is in the EU, the EEA, the UK or Switzerland, PostHog loads only after you say yes through the line the site shows. Before you answer, and if you say no, nothing is counted or recorded. If we cannot tell where you are, the site asks.

3.4 Everywhere else, we count pages without asking. This relies on legitimate interests, because nothing is stored on your device.

## 4 Session replay, only with your yes, when switched on {#replay status=planned until=opening}

> In plain words: when analytics is switched on, we record visits only if you agree, we never record what you type, and you can change your mind.

4.1 Once analytics is switched on, session replay and heatmaps run only after you say yes through the line on the site that asks. The line names PostHog, says that recordings are kept in the EU for 30 days, and links to this page. Before you answer, and if you say no, nothing is recorded.

4.2 A recording shows pointer movement, clicks, scrolling and the page's structure. Every text field is masked, so what you type is not recorded. The Start form is blocked from recording, and the Start page is never recorded.

4.3 We keep recordings for 30 days, then PostHog deletes them[^3].

4.4 You can take back your yes at any time on this page. A control here changes your answer to no, and recording stops at once. In the EU, the EEA, the UK and Switzerland, counting stops too. This page is linked at the foot of every page. A new page load starts a new recording, so nothing follows you from page to page.

4.5 Your answer, yes or no, lasts 6 months. After that the site asks again.

4.6 If your browser sends a Global Privacy Control or Do Not Track signal, we treat it as a no to session replay. Nothing is recorded and the site does not ask. In the EU, the EEA, the UK and Switzerland that also means PostHog does not load.

4.7 PostHog stores nothing in your browser, so recording adds only this entry.

Table: What recording stores in your browser

| Name | Kind | Set by | Purpose | Kept | Needs your yes |
|---|---|---|---|---|---|
| gp-site-recording | Local storage | Greypillar | Remembers your answer about recording and the day you gave it, so the site does not ask again for 6 months. Never sent to us | 6 months, then the site asks again, or until you clear it | No. It stores only your answer and its date |

## 4 Session replay, only with your yes {#replay opens=opening status=live}

> In plain words: we record visits only if you agree, we never record what you type, and you can change your mind.

4.1 Session replay and heatmaps run only after you say yes through the line on the site that asks. The line names PostHog, says that recordings are kept in the EU for 30 days, and links to this page. Before you answer, and if you say no, nothing is recorded.

4.2 A recording shows pointer movement, clicks, scrolling and the page's structure. Every text field is masked, so what you type is not recorded. The Start form is blocked from recording, and the Start page is never recorded.

4.3 We keep recordings for 30 days, then PostHog deletes them[^3].

4.4 You can take back your yes at any time on this page. A control here changes your answer to no, and recording stops at once. In the EU, the EEA, the UK and Switzerland, counting stops too. This page is linked at the foot of every page. A new page load starts a new recording, so nothing follows you from page to page.

4.5 Your answer, yes or no, lasts 6 months. After that the site asks again.

4.6 If your browser sends a Global Privacy Control or Do Not Track signal, we treat it as a no to session replay. Nothing is recorded and the site does not ask. In the EU, the EEA, the UK and Switzerland that also means PostHog does not load.

4.7 PostHog stores nothing in your browser, so recording adds only this entry.

Table: What recording stores in your browser

| Name | Kind | Set by | Purpose | Kept | Needs your yes |
|---|---|---|---|---|---|
| gp-site-recording | Local storage | Greypillar | Remembers your answer about recording and the day you gave it, so the site does not ask again for 6 months. Never sent to us | 6 months, then the site asks again, or until you clear it | No. It stores only your answer and its date |

## 5 Removing what is stored {#remove status=live}

> In plain words: your browser can clear all of it. The site then opens with its defaults.

5.1 You can remove everything in sections 2 and 4 through your browser's settings for site data. The site then opens in its default light level and, once analytics is switched on, asks again about recording.

5.2 Blocking storage does not stop the site from working.

## 6 Changes {#changes status=live until=opening}

> In plain words: we update this table before anything new is stored.

6.1 We update this notice before the site stores anything new in your browser. Every change is dated and public in the changes feed on [Trust](/trust).

## 6 Changes {#changes opens=opening status=live}

> In plain words: we update this table before anything new is stored.

6.1 We update this notice before the site stores anything new in your browser. Every change is dated and public in the changes feed on [Trust](/trust) and in the history of github.com/Greypillar/policies.

## 7 Language {#language status=live}

> In plain words: the English text governs.

7.1 {claim:language.governing}

7.2 No translation of this notice is published yet.
