# Agreements

The agreements Greypillar LLC will offer its customers. **State: draft, 14 November 2026. Not offered to anyone yet.** Each is written by Greypillar and has not been reviewed by outside counsel. Greypillar accepts the set before the first payment. Every clause has had an adversarial review, and this version carries its fixes.

## How the set fits together

Two ways in, one set of shared documents.

```text
 A PILOT (first)                         ONGOING WORK
 pilot-agreement.md                      customer-agreement.md  (Key Terms + Greypillar terms)
   = its own Order Form                    + order-form.md      (one per order)
 ─────────────────── both attach ───────────────────
 dpa.md               personal data, transfers, subprocessors (by reference to /trust/subprocessors)
 ai-addendum.md       training, contribution, agents, how far to rely on output
 billing-and-refunds.md   currency, taxes, credits, every refund case
 ../policies/acceptable-use.md   what no one may do, including Greypillar's own agents
```

- A pilot is signed as the **pilot agreement**, whose order form carries the written scope, the stated result and date, and the fee. If the customer continues, the **customer agreement** and an **order form** become the definitive agreement, and the pilot fee is credited in full.
- The **DPA** and the **AI addendum** attach to either. For personal data the DPA controls; for AI services the AI addendum controls.
- **Billing and refunds** and **acceptable use** are part of both.
- Order of precedence inside the customer agreement: DPA (personal data), AI addendum (AI services), Key Terms (the customer agreement, including the Greypillar terms), the order form (which changes a Key Term only where it names the section), billing and acceptable use, then the Common Paper standard terms. The customer agreement's section 1.3 states it. The pilot agreement's section 1.3 sets the same order for a pilot.

## Standard terms used

Each agreement incorporates Common Paper's standard terms by reference, **unmodified**, and changes them only through its cover page, as the standard terms are designed to be used. Greypillar's own terms sit on the cover page as named changes ("Greypillar terms"), each naming the section it changes. Versions were read at source on 12 November 2026.

| Document | Path | Standard terms | Version | Source |
|---|---|---|---|---|
| Customer agreement | /legal/terms | Cloud Service Agreement | 3.0 | https://commonpaper.com/standards/cloud-service-agreement/3.0 |
| Order form | /legal/order-form | Cloud Service Agreement cover page (Order Form) | 3.0 | https://commonpaper.com/standards/cloud-service-agreement/3.0/cover-page-docx |
| Pilot agreement | /legal/pilot | Pilot Agreement | 1.1 | https://commonpaper.com/standards/pilot-agreement/1.1 |
| Data processing agreement | /legal/dpa | Data Processing Agreement | 1.1 | https://commonpaper.com/standards/data-processing-agreement/1.1/ |
| AI addendum | /legal/ai-addendum | AI Addendum | 1.0 | https://commonpaper.com/standards/ai-addendum/1.0/ |
| Billing and refunds | /legal/billing | None (Greypillar's own text) | — | — |
| Acceptable use | /legal/acceptable-use | None (Greypillar's own text) | — | — |

Notes on versions:
- Common Paper's standalone "Order Form" document is written for the Cloud Service Agreement **v2**. For v3.0 the order form is part of the CSA cover page, so `order-form.md` follows that cover page.
- The AI Addendum is drafted to attach to a CSA or Software License Agreement. Greypillar also attaches it to the Pilot Agreement and says so on its cover page.
- The EU transfer clauses are the 2021 SCCs (Decision 2021/914), Modules 2 and 3; the UK uses the ICO Addendum B1.0; Swiss transfers follow the DPA standard terms §3.4. The Thai basis (PDPA s.29 standard contractual clauses) is open until the PDPC notification is read at source.

## Attribution (CC BY 4.0)

Common Paper's agreements are free to use and modify under the Creative Commons Attribution 4.0 International licence (https://creativecommons.org/licenses/by/4.0/). Each Greypillar agreement built on them:

1. names the Common Paper standard terms, their version and their versioned URL, and that they are © Common Paper, Inc. and licensed under CC BY 4.0;
2. says that the standard terms are incorporated without modification, and that its cover page is adapted from Common Paper's cover page, naming what Greypillar changed;
3. says that Common Paper is not a party and has not reviewed or endorsed it (the licence grants no endorsement);
4. keeps Common Paper's own footer line, for example "Common Paper Cloud Service Agreement (Version 3.0) free to use under CC BY 4.0."

Greypillar's own text in this repository is licensed under CC BY 4.0 as the repository README states.

## Decided terms these drafts carry

- Governing law Delaware
- SIAC arbitration seated in Singapore, English, one arbitrator, with court carve-outs for urgent relief and small money claims up to US$25,000
- Liability cap of 12 months' fees, never covering fraud, gross negligence, wilful misconduct, death or injury, or what the law forbids limiting (Thai CCC s.373)
- **For customers in the EU and the UK, liability for breach of the EU standard contractual clauses or the UK Addendum is uncapped**: the DPA standard terms §8.3 say so, and the DPA's section 13.2 repeats it
- **Insurance first: Greypillar processes no customer personal data, in any market, until its insurance is in place, so the insurance is in place before the first pilot** (DPA section 13.3)
- Every DPA security measure marked "Not yet", and every planned measure the processing relies on, is in place before the first customer personal data is processed (DPA Annex II, 18.2)
- Pilot of 30 days, fee credited in full; if the stated result is not delivered by the stated date, judged against the written scope, Greypillar refunds the fee it received plus any tax it collected and can recover, if the customer claims within 30 days after the stated date; a customer that had to withhold tax reclaims that part from its tax authority, with Greypillar's documents
- Disputed charges and refusals reviewed by an independent reviewer both sides agree, paid by Greypillar
- No trial auto-charge
- Money the customer adds itself never expires while the agreement runs; when it ends, the unused amount is refunded automatically within 30 days, and if that cannot be done the customer can ask for it for 24 months
- Any price increase lets the customer leave without charge
- Renewals off unless the customer turns them on
- Lapse ends future supply only, and the customer keeps what was delivered
- Greypillar's own parts inside delivered work are licensed for the customer's and its affiliates' own operations, not for resale
- No training on customer content by default; contribution only by a specific signed grant with an irreversibility warning, and no personal data in it unless anonymised first
- Three responsibility tiers: software, work Greypillar runs, acts the law reserves
- Agents say they are AI and say who is responsible; no person is named in the texts, the order form names the accountable role
- Upkeep in the service price within the agreed period, scope and conditions
- Subprocessors published 30 days before use, with an objection right and exit; for customer work they are approved in the order form
- Customer content stored in Helsinki, Finland by default; Greypillar reaches it only from Thailand; a new place of access is announced 30 days ahead, like a subprocessor
- No one may pass a technical barrier a source has put in place, use material known or suspected to come from a breach, or knowingly breach a source's terms of use, with no exception
- Material changes announced 30 days ahead

Every promise that binds Greypillar is written in full in the agreement itself, so it can change only with a new version. The site's claim registry holds the same promises in short form for the website, and the two must say the same thing. Only facts that are not promises appear as `{claim:id}`: `entity.legal_name`, `entity.address`, `channel.email`, `status.public_service` and `status.customers`.

## Not yet

Each arrives with its trigger. None is part of any agreement until it exists and is signed.

| Document | Trigger |
|---|---|
| Software License (self-hosted and offline; evergreen subscription with perpetual fallback) | The first self-hosted customer |
| Service level agreement (Common Paper SLA v2.0 as the base) | Hosted service |
| Enterprise security addendum | The first enterprise deal |
| Partner terms (Common Paper Partnership Agreement v1.1) | The first partner |
| Marketplace maker terms | The maker kit |
| Professional services terms beyond the order form (Common Paper PSA) | GP-run work too large for an order form's scope rows |
| Thai-language versions | Native review; English governs until then |
