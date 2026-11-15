---
slug: ai-addendum
path: /legal/ai-addendum
group: Agreements
audience: Customers
kind: Legal
legal: true
title: AI addendum
summary: The terms for the AI in Greypillar. Your inputs and outputs are yours, nothing trains a model unless you sign a specific grant, generated work proposes and a person commits it, and agents say what they are. It is the Common Paper AI Addendum, version 1.0, with Greypillar's own terms.
banner: "Draft. Not offered to anyone yet."
record:
  Version: "0.1"
  State: Draft
  Effective: Not set
  Updated: 14 November 2026
  Reviewed: Written by Greypillar. Not yet reviewed by outside counsel.
  Governing text: English
  Standard terms: Common Paper AI Addendum, version 1.0
changes:
  - {version: "0.1", date: "14 November 2026", text: "First published draft."}
sources:
  - {n: 1, text: "Common Paper AI Addendum Standard Terms, version 1.0 (CC BY 4.0)", href: "https://commonpaper.com/standards/ai-addendum/1.0/"}
  - {n: 2, text: "Regulation (EU) 2024/1689 (AI Act), Article 50, transparency obligations", href: "https://eur-lex.europa.eu/eli/reg/2024/1689/oj"}
---

# How this addendum is built

> lead: A cover page sets the variables. Common Paper's standard terms carry the rest. Greypillar adds the rules its agents work by.

## 1 What this addendum is {#what status=planned}

> In plain words: This adds the terms for the AI in Greypillar to your customer or pilot agreement. The notes in the margin help you read it. If a note and a clause differ, the clause governs.

1.1 This Cover Page incorporates the AI Addendum Standard Terms available at https://commonpaper.com/standards/ai-addendum/1.0/ ("AI Addendum Standard Terms") with the Variables set out below (together with the Greypillar Terms, the "AI Addendum").[^1]

1.2 This AI Addendum amends and is incorporated into the following "Agreement": the Greypillar customer agreement or pilot agreement between {claim:entity.legal_name} ("Provider" or "Greypillar") and Customer that refers to it. Undefined capitalized words have the meanings or descriptions given in the Agreement. If there is any inconsistency between this AI Addendum and the Agreement, the AI Addendum will control for the provision of AI Services. For Personal Data, the Data Processing Agreement controls over this AI Addendum.

1.3 The Greypillar Terms in sections 3 to 10 are part of this Cover Page and each names the section of the AI Addendum Standard Terms it changes, if any.

1.4 The notes headed "In plain words" are reading aids, not part of the AI Addendum. English governs; translations carry the same meaning.

## 2 Variables {#variables status=planned}

> In plain words: No training on your data. No product improvement built from your content for anyone but you. No indemnity for output, but the agreement's indemnity for the service still covers the AI in it. The acceptable use policy applies.

Table: Variables (Common Paper AI Addendum cover page, version 1.0)

| Variable | Value |
|---|---|
| Training Data | None |
| Training Purposes | None |
| Training Restrictions | Not applicable while Training Data is None. A Contribution Grant under section 5 states its own restrictions |
| Improvement Restrictions | (1) Neither Input nor Output may identify Customer. (2) Improvements based on Customer's Input or Output will be solely for Customer's benefit. (3) Greypillar may improve the AI System for other customers only from Usage Data as the Agreement defines it, which contains no Input or Output |
| Covered Claims | None for Output. Where the Agreement has Provider Covered Claims, they apply to the AI System and Models as part of the Cloud Service or Product |
| AI Acceptable Use Policy | Use of the AI Services is subject to the Acceptable use policy available at /legal/acceptable-use |

# Greypillar terms

> lead: The rules Greypillar's agents follow, written so you can hold Greypillar to them.

## 3 No training on your content {#training status=planned}

> In plain words: We do not train models on your content. That covers what you send and what Greypillar makes for you.

3.1 This section adds to AI Addendum Standard Terms Sections 1.3 and 1.4.

3.2 Greypillar does not train models on Customer Content. Greypillar will not use Input, Output, Customer Content or Feedback that contains Customer Content to Train any Model, and will not allow its Subprocessors to do so.

3.3 Greypillar routes requests to third-party Models only through providers whose terms, as Greypillar has accepted them, do not permit them to Train on Input or Output and keep no Input or Output after processing, except as each provider's zero-retention terms listed at /trust/subprocessors state, or through Customer's own provider account. OpenRouter states one such exception: content flagged as possible child sexual abuse material may be kept for review. OpenRouter also screens content in flight. The list at /trust/subprocessors, or the Order Form for customer work, names the providers and their countries before any use. Where a provider changes its terms so that this is no longer true, Greypillar stops using it for Customer's Input and replaces it under the Agreement's upkeep terms.

3.4 Section 1.4 of the AI Addendum Standard Terms applies only as limited by the Improvement Restrictions. Greypillar will not use Customer's Input or Output to build or improve any rule, pack, capability or other material offered to anyone other than Customer.

## 4 Who owns what {#ownership status=planned}

> In plain words: Your inputs and the outputs are yours. Greypillar keeps no right to use them for anyone else.

4.1 AI Addendum Standard Terms Section 2.1 applies. Output is part of the Delivered Materials under the Agreement, and the Agreement's licence of Greypillar Components in Delivered Materials applies to it.

## 5 Contributing data, if you ever choose to {#contribution status=planned decides}

> In plain words: You may choose to give data to improve Greypillar. We ask each time, say exactly what and why, say what you get, and say what cannot be undone. Nothing is contributed by default, by silence, or by a tick buried in another form.

5.1 Customer may choose to contribute data to improve Greypillar. Greypillar asks for each contribution specifically, says what Customer gains, and says what cannot be undone.

5.2 A contribution of Input, Output, Customer Content or Usage Data that identifies Customer to Train a Model, or to build material offered to others, happens only under a separate written "Contribution Grant". A Contribution Grant is valid only if: (a) it is signed or accepted, for that contribution, by a person authorised by Customer, separately from any Order Form or other acceptance; (b) it names the specific data or classes of data, the purpose, the Models or materials it may be used for, and who will have access; (c) it states what Customer receives for it; (d) it states the Training Restrictions that apply, such as de-identification or aggregation; and (e) it contains the warning in section 5.3, shown before acceptance.

5.3 The warning reads: "Once this data has been used to train a model, it cannot reliably be removed from that model. Withdrawing this grant stops any future use, but it cannot undo training that has already happened."

5.4 Customer may withdraw a Contribution Grant at any time, by notice, for future use. Greypillar then stops using the data for new Training or new materials, and deletes the contributed copy it holds, except what is already part of a trained Model or a released material.

5.5 Declining or withdrawing a Contribution Grant changes nothing in the price or the service Customer receives.

## 6 Generated work proposes, a person commits {#proposes status=planned decides}

> In plain words: What the AI generates is a proposal. It becomes an action or a final result only when a person with the authority to decide accepts it, or when it falls inside limits you set in advance.

6.1 This section adds to AI Addendum Standard Terms Section 1.1.

6.2 Output is a proposal until a person accepts it, or until it acts within a Standing Approval Customer has given under the Agreement. Greypillar will not configure the AI Services to send, pay, commit, delete or file anything that cannot be undone on Customer's behalf outside those limits.

6.3 In work Greypillar runs, a person at Greypillar reviews each result before it is delivered, unless the Order Form states otherwise for a named kind of result.

## 7 Agents say what they are {#agents status=planned}

> In plain words: Greypillar's agents tell people they are AI, and say who is responsible. No setting changes that.

7.1 This section adds to AI Addendum Standard Terms Section 1.2(c).

7.2 Each Greypillar agent that writes to a person says that it is an AI agent and says who is responsible for it. When an agent communicates with a person on Customer's behalf, it says that Customer is responsible, or names the role Customer designates for that work. When it communicates on Greypillar's behalf, it says that Greypillar is responsible, and that the accountable role is named in the Order Form.

7.3 Customer may set an agent's style, limits and subject matter. No setting allows an agent to claim to be a human, to deny being an AI when asked, to borrow the name of a real person, or to deceive the people Customer serves. Where Regulation (EU) 2024/1689 applies, Greypillar designs the AI Services so that people are told they are interacting with an AI system, as its Article 50 requires.[^2]

## 8 How far to rely on output {#reliance status=planned}

> In plain words: AI can be wrong, and the standard terms say so. Where we run the work, we answer for the result within the scope. Where the law reserves a decision for a licensed professional, AI output does not replace them.

8.1 AI Addendum Standard Terms Section 3 applies, subject to the Agreement's terms on work Greypillar runs, under which Greypillar answers for the result within the written scope.

8.2 Output does not replace an act that Applicable Laws reserve for a licensed or registered professional, and Greypillar does not represent that any Output makes Customer compliant with any law, regulation or standard.

8.3 Where an Output states something as fact, the Service shows what it rests on, where Customer is permitted to see the source, and keeps what was read, what was inferred and what is not known separate, as far as the Service's functions allow.

## 9 Your own AI provider {#own-provider status=planned}

> In plain words: You can use your own AI provider account. That provider works under your agreement with it, and Greypillar adds nothing to its price.

9.1 Customer may use its own AI provider account, and Greypillar adds no markup to it. Where Customer connects its own provider account, the provider's terms with Customer govern that provider's processing, including any training or retention, and Greypillar is not responsible for that provider's acts. Greypillar sends that provider only what the task needs.

## 10 No indemnity for output {#indemnity status=planned}

> In plain words: Some providers promise to defend you if their AI's output infringes someone's rights. Greypillar does not offer that for output. The agreement's promise to defend you if the service itself infringes still covers the AI in it. A person checks work Greypillar runs before it is sent.

10.1 The Variables set no Covered Claims for Output. Greypillar offers no indemnity for Output. This does not reduce any indemnity the Agreement gives for the Cloud Service or Product, which covers the AI System and Models as part of it.

# Signature

## 11 Acceptance {#acceptance status=planned}

> In plain words: Accepting the customer or pilot agreement accepts this addendum too.

11.1 By signing or accepting the Agreement that refers to it, or this Cover Page, each party agrees to enter into this AI Addendum.

## 12 Source and licence {#licence status=live}

> In plain words: The standard terms are Common Paper's, free to use under CC BY 4.0. Common Paper has not reviewed or endorsed this addendum.

12.1 The AI Addendum Standard Terms are the Common Paper AI Addendum Standard Terms Version 1.0, © Common Paper, Inc., available at https://commonpaper.com/standards/ai-addendum/1.0/ and licensed under CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/). They are incorporated by reference without modification. This Cover Page is adapted from the Common Paper AI Addendum cover page, version 1.0. Greypillar changed it by filling in its variables, extending its use to the Common Paper Pilot Agreement, and adding the Greypillar Terms. Common Paper is not a party to this AI Addendum and has not reviewed or endorsed it.

Common Paper AI Addendum (Version v1.0) free to use under CC BY 4.0.
