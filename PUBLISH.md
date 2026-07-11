# PUBLISH.md — adding to this repo

> **THE HARD RULE:** share the useful, never the engine. Reports: external PDFs
> only. Toolkit: author-curated items only — regulatory helpers, evals of shared
> skills, tips. Valuation / DD / base-rate / screening / fund-analysis skills:
> **never.** Live ideas and holdings: **never.** The governing law is the
> private repo's boundary document. Any doubt, any scan hit: stop.

## Shelf 1 — adding a research note (`reports/`)

1. Copy (never move) the note's **external PDF** into the right folder, named
   `<name>_<YYYY-MM>.pdf`: `stocks/` · `etfs/` · `funds/` · `macro/`.
2. Add one line to the README index under the matching heading.
3. Sanity-check: external render, public disclaimer visible, scan clean.
4. `git add -A && git commit -m "Add <name> note" && git push`

## Shelf 2 — adding a toolkit item (`toolkit/`)

1. **The author picks it.** Nothing lands here by default; each item is an
   explicit decision recorded against the boundary doc's toolkit rule.
2. **Make it self-contained.** Strip every reference to the private system —
   its folders, other skills, internal paths. If it can't stand alone without
   dragging engine context, it wasn't shareable.
3. **Date it.** Regulatory or fast-moving content carries "Last reviewed:
   <month year>" at the top.
4. **Attach the proof.** A shared skill ships with its worked example (real
   input → real output) — the eval is the credibility, not overhead.
5. Scan, then `git commit -m "Add toolkit: <item>" && git push`, and add its
   line to the README under **Use**.

## The one line to paste to Claude

> Publish <the new external note for TICKER / toolkit item NAME> to the public
> repo — run the boundary checklist first.

Notes: `.gitignore` is default-deny — only report PDFs and whitelisted toolkit
paths can be committed. One-way flow: nothing here feeds back into the private
system. Toolkit is MIT-licensed; reports are all rights reserved (see README).
