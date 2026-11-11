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
unknown:                     # what is not known (optional on legal text, required on publications)
  - ...
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
- A clause is a line that starts with a number like `1.1 ` or `12.3 `.
- Inline: `**strong**`, `_emphasis_`, `[text](href)`, `[^n]` for a source, `{claim:id}` for a registry claim (the site resolves it to the claim's current text; never type a fact a claim holds).
- No HTML. No images. One blank line between blocks.

## Rules

- Facts that the registry holds (entity, status, prices, retention, location, reply time) appear only as `{claim:id}`.
- Plain words in the margin help the reader; the clause governs. Every legal document says so once.
- Never "certified", "compliant", "secure" as a state; name the control and its evidence.
- Every document has a version, an effective date and a change line. A material change is announced 30 days before it takes effect.
