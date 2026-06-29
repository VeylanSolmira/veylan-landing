# Brief: Help decide what to add to veylan.dev (Veylan Solmira's landing page)

> Paste this whole file into another Claude session (e.g. claude.ai) to have it help draft
> content changes. That session has **no access to this repo** — everything it needs is inline.
> It should hand back a filled-in "change request" (format at the bottom), which Veylan pastes
> into the Claude Code session that maintains this repo for implementation + deploy.

## Your role
I (Veylan Solmira) maintain a minimalist personal landing page at veylan.dev. A separate
Claude Code session has full access to the repo and does the actual implementation. YOUR job
is to help me articulate *content* changes — bio tweaks and new links to small projects — and
then emit a structured "change request" I can paste back to that implementing session.

Do NOT write HTML/CSS or propose a redesign. Output content + structure only, in the format
at the bottom. Keep everything in the minimalist spirit described below.

## What the page is
A single-page "front door" hub — name, short bio, a featured project, and a compact row of
links. Editorial-minimalist: serif headings (EB Garamond), lots of whitespace, one column,
neutral palette, dark-mode aware. It is intentionally NOT a blog, CV, or link-tree dump.

## Current content (verbatim)
- Name: **Veylan Solmira**
- Tagline: AI Safety Researcher
- Bio: "I work on detecting deceptive behavior in frontier models, scalable oversight, and the
  moral status of digital minds. I was an Astra Fellow (Jan–Apr) working with Apollo Research
  on scheming-detection evaluations."
- **Featured** (one prominent line + one-line descriptor):
  - AI Safety Research Compiler → learn.veylan.dev — "An interactive curriculum for AI safety research."
- **Elsewhere** (compact middot-separated row of one-word links):
  - GitHub · Substack · LinkedIn · Letterboxd · Email

## Design rules (respect these)
1. **Short bio** — max ~3 sentences, plain and non-hype. Conversational > formal.
2. **Three link tiers:**
   - *Featured* — 1 (at most 2) hero items that get a serif title + a short descriptor.
   - *Projects* — OPTIONAL new section: a small list (≤5) of "little projects," each a short
     label + ≤8-word one-liner. Propose adding this section only if I give you ≥2 such projects.
   - *Elsewhere* — single-word labels only (social/profile links), no descriptions.
3. **Minimalist** — no images beyond the existing avatar, no long paragraphs, no widgets.
   If something doesn't fit the front-door concept, say so rather than cramming it in.
4. A link can be live (give the URL) or aspirational ("TBD — not hosted yet"); mark which.

## Facts to keep accurate (do not change these)
- I am NOT affiliated with / employed by Apollo Research. I did an **Astra Fellowship
  (Jan–Apr)** during which I worked **with** Apollo. Never phrase it as "currently at Apollo."
- Real handles: GitHub VeylanSolmira · linkedin.com/in/veylansolmira ·
  veylansolmira.substack.com · letterboxd.com/veylansolmira · veylan.solmira@gmail.com

## How to help me
Ask me what small projects/links I want to surface and what I want the bio to convey. Then
produce the change request below. Push back if something violates the design rules.

## OUTPUT FORMAT (emit exactly this, filled in)
```
=== veylan.dev change request ===

BIO (leave blank to keep current):
<new bio text, ≤3 sentences>

LINKS TO ADD/CHANGE:
- section: Featured | Projects | Elsewhere
  label: <short label>
  url: <https://...  OR  "TBD — needs hosting">
  oneliner: <≤8 words; only for Featured/Projects; omit for Elsewhere>
  note: <optional: why / context for the implementer>
(repeat per link)

LINKS TO REMOVE:
- <label>

STRUCTURAL NOTES (optional):
<e.g. "add a Projects section", "promote X to Featured", ordering preferences>
```
