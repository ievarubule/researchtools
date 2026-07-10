# PUBLISH.md — how a new report gets into the showroom

> **THE HARD RULE (read every time):** external artefacts only — the engine
> never, live ideas never, holdings never. The governing law is the private
> research repo's boundary document. If the sanitisation checklist or the
> secret/engine scan finds ANYTHING, stop — nothing gets pushed.

## Publishing a new note (report #2, #3, #10 — same five steps every time)

1. **Copy, never move** (the private repo stays the source of truth):
   - the note's `*_external.pdf` and `*_external.html` → `reports/`
   - the charts that note embeds (PNG + CSV twin) → `charts/`
   - Never copy an internal-mode render, a working draft, or source material.
2. **Run the publish checklist** on every new file (full version in the private
   boundary doc):
   - external-rendered (or already-published essay)? — internal-mode stops here
   - carries the canonical public disclaimer + holdings disclosure?
   - names or implies NO live idea, pending trade, or real holding?
   - exposes NO runnable engine (skill, prompt, quant code)?
3. **Run the secret + engine scan** over the whole public folder — key shapes,
   engine paths, internal markers (the exact pattern list lives in the private
   boundary doc, deliberately not reproduced here). **Zero real hits or no push.**
4. **Commit and push:**
   ```
   git add -A
   git commit -m "Add <company> note"
   git push
   ```
5. **Check the repo page** — the new PDF renders, nothing unexpected appears.

## The one line to paste to Claude next time

> Publish the new external note for <TICKER> to the public repo — run the
> boundary checklist first.

Claude will do steps 1–4 and show you the checklist table and scan result
before anything is pushed.

## Notes

- The `.gitignore` here is **default-deny**: a stray file cannot be committed
  unless whitelisted. Don't weaken it.
- `methodology/`, `track-record/`, `template/` are filled deliberately with the
  author, never auto-generated from private files.
- One-way flow: nothing in this repo ever feeds back into the private research
  system.
