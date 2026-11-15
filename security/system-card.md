---
slug: system-card
path: /trust/system-card
group: Security
audience: Security teams
kind: System card
title: System card for Greypillar's agents
summary: What the agents planned for the first step may and may not do, how they are routed, what is known to go wrong, and what has and has not been tested.
banner: "{claim:status.public_service} No agent handles a visitor's words today. This card describes the design for step 1. Nothing here has been evaluated."
record:
  Version: "1.1"
  State: Draft
  Effective: Not set
  Updated: 15 November 2026
  Reviewed: Written by Greypillar. Not independently assessed.
  Governing text: English
changes:
  - {version: "1.1", date: "15 November 2026", text: "Website analytics do not run for visitors in Europe (4.7)."}
  - {version: "1.0", date: "14 November 2026", text: "First published draft."}
sources:
  - {n: 1, text: "OpenRouter, the model routing service chosen for step 1", href: "https://openrouter.ai"}
---

# What the agents do
> lead: In the first step, agents turn a visitor's own words into a draft brief. A person checks it before anything is sent, and the agents can do nothing else.

## 1 What this card covers {#covers status=live}
> In plain words: it covers the agents that will read what a visitor writes. They do not exist yet.

1.1 {claim:status.public_service} No agent reads a visitor's words today. The Start page runs without AI.
1.2 This card covers the agents planned for step 1: the ones that read a visitor's words and at most one file, and prepare a provisional brief. It does not cover the product, which does not exist.
1.3 Greypillar also uses AI tools to write its own code and documents. Those are not covered here.
1.4 {claim:responsibility.agent_disclosure}
1.5 This card is a draft. It describes a design, not behaviour anyone has observed. It changes when the design changes, with a new version and date above.

## 2 What the agents may and may not do at step 1 {#scope status=planned decides}
> In plain words: they read, draft and hand over. A person sends. They cannot act anywhere else.

2.1 The visitor says what they want, or adds one file, and gives a name and a work email. They press Send. Agents prepare a provisional brief from those words and that file. A person checks it and replies.
2.2 Nothing is sent to the visitor, or anyone, until that person has checked the brief. The person who checks is the one responsible for it.

Table: What the agents may and may not do

| May | May not |
|---|---|
| Read what the visitor wrote and the one file they added | Take any action in an outside system |
| Prepare a provisional brief from those: what the visitor wants, what it may be worth, what must become known, what stays as it is, the first proof, and what is uncertain | Send a message, an email or a file to anyone |
| Read the one request they are preparing, read-only, and never the table | Change or delete any record |
| Leave a value as not known yet until a source shows it | Open or run anything inside a file on the intake server |
| Say they are agents when asked, and say who is responsible | Claim to be a person, or deny being an agent |
| | Invent a value no source shows |
| | Make an offer, a price, a promise or a commitment |
| | Build a profile of a person |
| | Use what a visitor sent to train a model |

2.3 Agents disclose that they are agents and say who is responsible for what they prepare. Hiding it is not a setting that exists. Each brief carries a line that says it was prepared by Greypillar's agents, that a person checked it before it reached you, and who is responsible.
2.4 A visitor can ask for what they sent to be deleted. They can also ask to hear when a workspace can open; that is a separate choice and is off unless they make it.
2.5 A file added through Start can be up to 4 MB at step 1. A larger file would need a direct upload, which does not exist yet.

## 3 The gate rule, as designed {#gate status=planned decides}
> In plain words: nothing changes in a customer's affairs except through one door. The agents at step 1 have no door at all.

3.1 Step 1 has no gate, because the agents change nothing. The gate rule is how the product will govern anything that does. It is a specification with tests, not a running system.
3.2 What is in force changes only through an accepted proposal, or through a rule already in force applied to a fact a boundary recorded. A consequence never goes beyond the rule that was accepted. Free text is no fact.
3.3 A note never changes what is in force. A note can start narrowing, a recheck or attention, nothing else.
3.4 Accepted is not done. An effect counts as done only when its evidence shows it.
3.5 A stop is never held beyond the current prepare bound. A stop that was requested stays apart from a stop a receiver confirmed, and each receiver not yet covered is named. A change that would widen anything fails closed.
3.6 The specification's tests run against a reference model with a defect planted in each, to show the test would catch it. This tests the specification. It does not test any agent. See [the gate rule](/docs/gate-rule) and [commitments](/commitments).

## 4 Model routing and data handling {#routing status=planned}
> In plain words: one route to the models, to providers that say they do not keep or train on what they are sent.

4.1 Briefs are prepared through OpenRouter, a service that routes a request to a model provider.[^1] Greypillar restricts it to providers that do not train on inputs and keep no data.
4.2 Which provider answers a given request is not fixed. That varies, and Greypillar cannot verify a provider's claim. OpenRouter and the providers it uses are named in the Order Form or in the [subprocessor list](/trust/subprocessors) before any is used. A change to that list is published 30 days before it takes effect.
4.3 What a visitor sends is stored on a server Greypillar rents, as plain database records and a file store, with a copy to {claim:channel.email}. {claim:location.data_hosting}
4.4 The intake has no open port to the internet. Only the website's own server function reaches it, through an encrypted Cloudflare tunnel that requires a secret token. Files are stored as received and are never opened on that server; reading a file happens in a sandbox on a separate server.
4.5 The agents read only the one request they are preparing, read-only, and never the table. They write nothing back to the intake.
4.6 {claim:data_use.no_training_default} A visitor's words are kept so a workspace can start from them, and deleted on request or after the period in the privacy notice.
4.7 Website analytics are cookieless and aggregate, and do not run at all for visitors in the EU, the EEA, the UK or Switzerland. Session replay runs only for visitors who agree, with inputs masked, and Start is never recorded. Replays are kept 30 days. A Global Privacy Control or Do Not Track signal counts as a no to replay.
4.8 The agents are not built. The intake that stores requests is deployed when greypillar.ai opens. No agent reads from it until the agents exist.

## 5 Known limits and failure modes {#limits status=planned}
> In plain words: these agents can be wrong, can be talked into odd output, and can miss things in a file. That is why a person reads every brief.

5.1 **They can be wrong.** A brief may misread the request, leave out something important, or state something the visitor did not say. The brief is provisional for that reason.
5.2 **Hostile text.** A visitor's words or file may contain instructions meant to steer the agent. The agents have no outside action to be steered into, and a person reads the brief. A steered brief could still mislead that person. Prompt injection has not been tested.
5.3 **Files.** A file may be unreadable, very long, in another language or not what it claims. The agent may skip or misread part of it and may not say so.
5.4 **Thai and other languages.** Output quality outside English has not been tested.
5.5 **About Greypillar.** An agent may describe what Greypillar offers wrongly. Claims on the website come from a registry with expiry dates, but an agent's own sentence is not checked against it automatically.
5.6 **Sensitive content.** A visitor may send personal or confidential material. The agents are not designed to recognise it. The retention and deletion rule applies to everything sent.
5.7 **Outage.** If the model route fails, a person writes the reply without a draft. {claim:channel.reply_time} That reply time is a goal of the design, not a record of anything.
5.8 **Provider behaviour.** A model provider can change what it does, retain data against its stated terms or be compromised. Greypillar would learn of it from the provider. No contract exists yet.
5.9 **No guarantee of consistency.** The same words may produce different briefs.

## 6 Evaluations {#evals status=not_yet}
> In plain words: no evaluation has been run. We would rather say so than imply one.

6.1 No evaluation of the agents has been run. There is no test set, no accuracy measurement, no prompt-injection or red-team test, no bias or fairness test, no test in Thai, and no outside review.
6.2 The website's automated tests cover the website's code and a small number of its response headers. They do not cover any agent.
6.3 The specification's tests of the gate rule cover the rule. They do not show that an agent behaves.
6.4 Until evaluations exist, nothing in this card should be read as a measured property.

## 7 How to report a problem {#report status=live}
> In plain words: write to us, and a person replies.

7.1 To report an agent's mistake, a worry about how it behaved, or a concern about this card, write to {claim:channel.email}. A person reads it.
7.2 To report a security problem, write to security@greypillar.ai, as the [vulnerability disclosure policy](/legal/vulnerability-disclosure) sets out.
7.3 Greypillar's incident plan is short and has not yet been exercised (see the [security overview](/security), section 9), so we cannot promise a fix time. We will say what we know.
