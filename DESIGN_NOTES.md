# Design notes — veylan.dev landing page

A living scratchpad for the landing page's design rationale: what the "consensus"
looks like among comparable personal sites, where this design deliberately differs,
and options to revisit later. Edit freely.

## Reference cohort

Surveyed 9 prominent AI / AI-safety researcher personal homepages:

- [Andrej Karpathy](https://karpathy.ai)
- [Chris Olah](https://colah.github.io)
- [Lilian Weng](https://lilianweng.github.io)
- [Simon Willison](https://simonwillison.net)
- [Chip Huyen](https://huyenchip.com)
- [Neel Nanda](https://www.neelnanda.io)
- [Jacob Steinhardt](https://jsteinhardt.stat.berkeley.edu)
- [Paul Christiano](https://paulfchristiano.com)
- [Dario Amodei](https://darioamodei.com)

## The consensus (what nearly everyone does)

- **Single-column, text-first layout** — no sidebars, no grids. (9/9)
- **Sans-serif typography** — system or web-safe sans throughout. (9/9)
- **Neutral palette** — black/dark text on white/light; one accent color (usually blue)
  reserved for links. No gradients, decoration, or animation. (9/9)
- **Very short bio** — 2–3 conversational sentences, not a formal CV summary. (8/9)
- **Two content models:** *hub* (name + bio + curated links: Karpathy, Christiano, Amodei)
  vs *blog/feed* (reverse-chron writing list: Weng, Nanda, Olah).
- **Link presentation, three modes:** icon-only row (Karpathy, Nanda) · inline links woven
  into the bio (Christiano, Amodei) · compact text list (Huyen).
- **Avatar is optional** — 5/9 are text-only; small circular photo on 2/9; larger centered
  headshot on 2/9. When present, minimal framing (no borders/shadows).

### Table-stakes vs differentiators

| Table-stakes | Differentiators (rarer, add character) |
|---|---|
| Single column | Serif headings (vs the universal sans) |
| Neutral palette, minimal | Small circular avatar (only 2/9) |
| ≤3-sentence bio | Conversational bio tone |
| Scannable links | Compact text links over icon rows / cards |

## Where this design deliberately differs

This page is a **hub** (not a blog/feed), and breaks from the cohort on purpose to look
distinctive while staying "polished academic":

1. **Serif headings — EB Garamond.** The cohort is 100% sans; an editorial serif for the
   name/headings is the single biggest differentiator. Body stays system-sans for clarity.
   The bio is also set in serif (larger) for an editorial, essay-like feel.
2. **Small circular avatar.** Currently an EB Garamond italic "V" **monogram** (SVG), which
   reads as intentional/editorial and needs no photo. Swappable to a real headshot anytime
   (see comment in `index.html`).
3. **Compact text links, not a card grid.** The original draft used bordered link "cards";
   replaced with a hairline-ruled *Featured* line (the Compiler) + a middot-separated
   *Elsewhere* row — closer to Huyen/Christiano, less heavy.

Everything else follows the consensus: single column (~38rem), warm-neutral palette, one
restrained navy accent, ≤3-sentence bio, dark-mode via `prefers-color-scheme`.

## Options to explore later

- **Other serif faces:** Fraunces (more modern/personality) or Newsreader (longform/journal)
  — swap the `@font-face` + `--serif` var to test.
- **Monospace/terminal direction** — a more "builder/hacker" identity (rejected for now).
- **Add a "Selected work" section** — short reverse-chron list of 3–5 projects/writings with
  one-line descriptions (moves toward the blog/feed model).
- **Add a "Now / updates" line** — signals the page is alive/maintained.
- **Icon-only link row** — if the text row ever feels wordy.
- **Real photo vs monogram** — drop in `avatar.jpg` and uncomment the `<img>` to A/B it.
- **Accent color** — could shift from navy to a warmer editorial ink (oxblood/terracotta).
