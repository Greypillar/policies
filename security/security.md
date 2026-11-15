---
slug: security
path: /security
group: Security
audience: Security teams
kind: Security
legal: false
title: Security overview
summary: Which security controls protect greypillar.ai and the Start intake today, which are planned, and which do not exist yet. Each control is named with its evidence. No certification is held.
banner: ""
record:
  Version: "1.0"
  State: In force
  Effective: On the opening of greypillar.ai
  Updated: 14 November 2026
  Reviewed: Written by Greypillar. Not yet reviewed by outside counsel or an independent assessor.
  Governing text: English
changes:
  - {version: "1.0", date: "14 November 2026", text: "First published version, in force from the opening of greypillar.ai."}
sources:
  - {n: 1, text: "Response headers of https://greypillar.ai/ observed on 14 November 2026 (HSTS, content security policy, frame refusal, Cloudflare in front of Vercel)", href: "https://greypillar.ai/"}
  - {n: 2, text: "Cloudflare, Access service tokens", href: "https://developers.cloudflare.com/cloudflare-one/identity/service-tokens/"}
  - {n: 3, text: "RFC 9116, A File Format to Aid in Security Vulnerability Disclosure (security.txt)", href: "https://www.rfc-editor.org/rfc/rfc9116"}
  - {n: 4, text: "Personal Data Protection Act B.E. 2562 (2019), unofficial English translation (KMUTT copy), section 37(4)", href: "https://cc.kmutt.ac.th/Files/Act%20Eng/personal-data-protection-act-2019-en.pdf"}
  - {n: 5, text: "Supabase security page (mechanisms read: shared responsibility stated per party, limits stated by plan)", href: "https://supabase.com/security"}
  - {n: 6, text: "Hetzner, Data protection at Hetzner (DPA concluded in the account, data stays in the chosen location)", href: "https://docs.hetzner.com/general/company-and-policy/data-protection-at-hetzner"}
---

## 1 What this is {#scope status=live}

> In plain words: what protects the website and Start today, stated as it is. Where something does not exist, this page says so.

1.1 This overview describes the security controls for greypillar.ai and the Start intake. {claim:status.public_service} There is no customer system to describe yet.

1.2 Each section has a status. Live means the control runs today. Planned means it is decided and not yet running. Not yet means it does not exist.

1.3 This page makes no promise beyond what it states, and it does not limit any liability that the law does not allow to be limited, including under section 373 of the Thai Civil and Commercial Code.

## 2 Hosting and network {#hosting status=live}

> In plain words: Cloudflare sits in front of the website, Vercel serves it, and mail runs on Google Workspace.

2.1 Vercel serves the website. Cloudflare provides DNS and sits in front of the site as a proxy[^1].

2.2 Mail for greypillar.ai runs on Google Workspace. The domain publishes an SPF record and a DMARC record. The DMARC policy is "none" today, which reports spoofed mail but does not reject it.

## 3 Encryption in transit {#in-transit status=live}

> In plain words: every connection to the site is encrypted.

3.1 The site is served only over HTTPS. Plain HTTP requests are redirected to HTTPS. The site sends a Strict-Transport-Security header with a two-year lifetime[^1].

3.2 The site sends a content security policy that limits where scripts, styles and connections may come from, and refuses to be framed by other sites[^1].

3.3 Mail between Google and other mail servers is encrypted when the other server supports it.

## 4 Access {#access status=planned}

> In plain words: one role holds administrative access today. The controls below are decided and being confirmed one by one.

4.1 Administrative access to Greypillar's accounts and servers is held only by the people at Greypillar who need it. Agents act only within limits those people set.

4.2 Agents get the least access their task needs. On the intake, an agent reads only the one request it is preparing. It reads it read-only, never the whole table, and cannot change or send anything.

4.3 Secrets are kept in a secrets manager and injected when a service starts. They are not stored in code repositories.

## 5 Signing in {#sign-in status=live}

> In plain words: the four accounts the site depends on use passkeys or two-factor sign-in, as Greypillar confirmed on 12 November 2026.

5.1 Google Workspace, GitHub, Vercel and Cloudflare each use passkeys or two-factor sign-in. Greypillar confirmed this on 12 November 2026. This is Greypillar's own statement, and no independent party has checked it.

5.2 Greypillar does not claim passkeys or two-factor sign-in on any other account.

## 6 Development {#development status=live}

> In plain words: every change to the website runs automated checks, and dependency updates are proposed weekly.

6.1 The website's code lives in a private GitHub repository. Every pull request, and every change to its main branch, runs automated checks: type checks, linting, a check of the public claims, unit tests, a production build and a browser test suite.

6.2 Dependabot proposes updates to dependencies and to the build workflow every week. A person decides each update. The web framework is pinned and changes only by a person's decision.

6.3 Changes are reviewed by the accountable lead and by AI agents. There is no second human reviewer yet.

## 7 How the Start intake will be built {#intake status=planned until=opening}

> In plain words: Start is not open yet. When it opens, our intake service has no open port to the internet, and files are never opened where they are stored.

7.1 Start is not open yet, and nothing in this section runs today. When it opens, Start requests will be stored on a server Hetzner runs for Greypillar in Helsinki, Finland. Hetzner keeps a cloud server's data in the location chosen for it[^6]. The website's server function will reach it only through an encrypted Cloudflare tunnel.

7.2 The intake will have no open port to the internet. Only the website's own server function will reach it, through an encrypted Cloudflare tunnel that requires a secret token[^2].

7.3 A file will be stored exactly as received. It will never be opened, parsed or previewed on that server.

7.4 A copy of each request will go to {claim:channel.email}, and a person will reply from there.

7.5 No agent will read Start requests at first, and no request will go to an AI model. When that changes, the [privacy notice](/legal/privacy) and the [subprocessors](/trust/subprocessors) list will announce it at least 30 days ahead. Agents will then read only the one request they are preparing, read-only, and never the table.

## 7 How the Start intake is built {#intake opens=opening status=live}

> In plain words: our intake service has no open port to the internet, and files are never opened where they are stored.

7.1 Start requests are stored on a server Hetzner runs for Greypillar in Helsinki, Finland. Hetzner keeps a cloud server's data in the location chosen for it[^6]. The website's server function reaches it only through an encrypted Cloudflare tunnel.

7.2 The intake has no open port to the internet. Only the website's own server function reaches it, through an encrypted Cloudflare tunnel that requires a secret token[^2].

7.3 A file is stored exactly as received. It is never opened, parsed or previewed on that server.

7.4 A copy of each request goes to {claim:channel.email}, and a person replies from there.

7.5 No agent reads Start requests yet, and no request goes to an AI model. When that changes, the [privacy notice](/legal/privacy) and the [subprocessors](/trust/subprocessors) list announce it at least 30 days ahead. Agents will then read only the one request they are preparing, read-only, and never the table.

## 8 Encryption at rest {#at-rest status=not_yet}

> In plain words: we have not confirmed disk encryption on our own server, so we do not claim it.

8.1 Disk encryption on Greypillar's intake server is not confirmed. Until it is, Greypillar does not claim it.

8.2 Vercel, Cloudflare, Google, PostHog and OpenRouter each describe their own encryption at rest in their own documentation. Greypillar has not audited it.

## 9 Incidents {#incidents status=live}

> In plain words: if something goes wrong with personal information, we contain it, tell the regulator within 72 hours where required, and tell you if you are at risk. The plan has not been tested yet.

9.1 When we learn of a security incident, we contain it first, then find what was affected and who.

9.2 If personal information is breached and this is likely to put people at risk, we tell the Office of the Personal Data Protection Committee without delay, and within 72 hours of becoming aware of it where feasible[^4]. Where the GDPR applies, we tell the relevant supervisory authority on the same timeline.

9.3 If the risk to you is high, we tell you directly and without delay, with what happened and what you can do.

9.4 We publish a dated note in the changes feed on [Trust](/trust) once doing so no longer puts anyone at further risk.

9.5 This plan is short and has not been tested in an exercise.

9.6 In June 2026 a server used neither by the website nor by the Start intake was isolated after a compromise whose cause was not established. It stays isolated.

## 10 Backups and continuity {#backups status=not_yet}

> In plain words: Start material is not backed up today.

10.1 Start material is not backed up today. Before it is, the [retention schedule](/legal/retention) will state how long backups are kept.

## 11 Certification and assessment {#certifications status=not_yet}

> In plain words: no certificate, no audit report and no penetration test yet. We say which controls exist instead.

11.1 {claim:assurance.certifications}

11.2 No independent audit or penetration test has been carried out. A draft self-assessment against the Cloud Security Alliance's questionnaire (the CAIQ, for CSA STAR Level 1) is published as [STAR self-assessment](/trust/star), labelled self-assessed. It is not submitted to the STAR Registry.

## 12 Who is responsible for what {#shared status=planned}

> In plain words: when the service runs, where it runs decides who looks after each layer. Nothing runs yet.

12.1 Greypillar's system is planned to run in four places. This table sets out who will be responsible for each layer in each place. No service runs in any of them yet.

Table: Shared responsibility by place (planned)

| Layer | Greypillar's cloud | Your cloud | One machine | Offline |
|---|---|---|---|---|
| Physical hardware and data centre | Greypillar's hosting provider | Your cloud provider | You | You |
| Network and firewall | Greypillar | You, with Greypillar's published settings | You | You. No connection by design |
| Operating system and patches | Greypillar | You, or Greypillar if you grant access | You | You |
| Greypillar software and its updates | Greypillar | Greypillar publishes signed updates. You apply them | Greypillar publishes signed updates. You apply them | Greypillar delivers signed updates, online or carried in. You apply them |
| Keys and who can sign in | Greypillar runs sign-in. You decide who has access | You | You | You |
| AI model provider | Greypillar's providers, or your own account | Your choice | Your choice, including models on the machine | Models on site only |
| Backups | Greypillar | You | You | You |
| Monitoring and incident response | Greypillar | Shared. Greypillar for its software, you for your environment | You, with Greypillar's support | You, with Greypillar's support |
| Your data and what agents may do with it | You decide. Greypillar enforces your rules | You decide. The software enforces your rules | You decide. The software enforces your rules | You decide. The software enforces your rules |

## 13 Reporting a security problem {#report status=live}

> In plain words: write to security@greypillar.ai. The disclosure policy protects good-faith research.

13.1 Report a vulnerability to security@greypillar.ai. The [vulnerability disclosure policy](/legal/vulnerability-disclosure) sets out scope, safe harbour and what to expect.

13.2 The site publishes a security.txt file at /.well-known/security.txt that points to this address and to the policy[^3].

## 14 Changes {#changes status=live until=opening}

> In plain words: this page changes as controls change. Every change is dated.

14.1 We update this overview when a control starts, stops or changes. Every change is dated and public in the changes feed on [Trust](/trust).

## 14 Changes {#changes opens=opening status=live}

> In plain words: this page changes as controls change. Every change is dated.

14.1 We update this overview when a control starts, stops or changes. Every change is dated and public in the changes feed on [Trust](/trust) and in the history of the public policies repository on GitHub.
