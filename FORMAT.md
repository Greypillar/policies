# How a document is written here

One Markdown file per document. The website reads these files into its reading system (GP-SITE `components/read/model.ts`, type `ReadingDoc`), so the page, its Markdown twin and this file say the same thing. The format is small on purpose.

## Front matter (YAML)

```yaml
---
slug: privacy                # stable id; also the file name
path: /legal/privacy         # the site address
group: Policies              # Agreements | Policies | Security | Data
audience: Everyone           # Everyone | Customers | Partners | Makers | Security teams
kind: Legal                  # the word above the title
legal: true                  # legal text: closer measure, smaller head
title: Privacy notice
summary: One or two sentences: what this document is for.
banner: ""                   # only when the text is a draft or not in force
record:                      # shown as the document's record, in this order
  Version: "1.0"
  State: In force            # In force | Draft | In progress
  Effective: 11 November 2026
  Updated: 11 November 2026
  Reviewed: Written by Greypillar. Not yet reviewed by outside counsel.
  Governing text: English
changes:
  - {version: "1.0", date: "11 November 2026", text: "First version."}
sources:                     # optional; cited in text as [^1]
  - {n: 1, text: "Common Paper Cloud Service Agreement, version 3.0", href: "https://commonpaper.com/standards/cloud-service-agreement/3.0/"}
---
```

## Body

```markdown
# Part title                                  ← optional; starts a part
> lead: One sentence that opens the part.     ← optional

## 1 Who we are {#who status=live}            ← a section: number, title, id, status
> In plain words: Greypillar LLC decides how your data is used.   ← the margin note
1.1 Greypillar LLC, a Delaware limited liability company, is the controller.   ← a numbered clause
A plain paragraph.                            ← p
- a list item                                 ← list

| Name | Purpose | Data | Location |          ← table; an optional caption line above it:
|---|---|---|---|                                Table: Subprocessors in use
| Vercel Inc. | Hosting | ... | United States |
```

- Section attributes in `{...}`: `#id` (required), `status=` one of `live` (holds today), `early_access`, `planned`, `not_yet`, `open` (not written), and `decides` when a person decides there (the one ember mark).
- A section that changes when the site opens is written twice, one after the other, with the same number and id: the text that holds now carries `until=opening`, the text that holds from the opening carries `opens=opening`. The site shows one of the two, from the opening gate (GP-SITE `registry/opening.yaml`, recorded only by `pnpm opening:open` after every check passes).
- A clause is a line that starts with a number like `1.1 ` or `12.3 `.
- Inline: `**strong**`, `_emphasis_`, `[text](href)`, `[^n]` for a source, `{claim:id}` for a registry claim (the site resolves it to the claim's current text; in a policy, never type a fact a claim holds; agreements: see Rules).
- No HTML. No images. One blank line between blocks, including after a `> In plain words:` note (without it, GitHub shows the next clause inside the quote).

## Rules

- A legal or security text here carries no "what is not known" list. Open questions about a document are kept privately (founder, 2026-11-14), because they name infrastructure and undecided points.

- Facts that the registry holds (entity, status, prices, retention, location, reply time) appear as `{claim:id}` in policies, so the site and the text never disagree. In an agreement, every operative promise is written out in full, in the agreement's own defined terms, so the commit history shows the words a customer signs; `{claim:id}` stays only for non-operative facts there (the entity's name and address, the contact address, status lines).
- Plain words in the margin help the reader; the clause governs. Every legal document says so once.
- Never "certified", "compliant", "secure" as a state; name the control and its evidence.
- Every document has a version, an effective date and a change line. A material change is announced 30 days before it takes effect.
