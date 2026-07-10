# PUBLISH.md — adding a note to this repo

> **THE HARD RULE:** external PDFs only — never the engine, never live ideas,
> never holdings. The governing law is the private research repo's boundary
> document. Any doubt, any scan hit: stop, nothing gets pushed.

## To add a note

1. Copy (never move) the note's **external PDF** from the private repo into the
   right folder, named `<name>_<YYYY-MM>.pdf`:
   - `reports/stocks/` · `reports/etfs/` · `reports/funds/` · `reports/macro/`
2. Add one line to the README index under the matching heading:
   `**<Company>** — <Month Year> — *<the note's one-line question>* → <path>`
3. Sanity-check: it is the *external* render, it carries the public disclaimer,
   and the scan (key shapes, engine paths, internal markers — full list in the
   private boundary doc) is clean.
4. ```
   git add -A
   git commit -m "Add <name> note"
   git push
   ```

## The one line to paste to Claude

> Publish the new external note for <TICKER> to the public repo — run the
> boundary checklist first.

Notes: the `.gitignore` is default-deny (only PDFs under `reports/` plus the
index files can be committed). One-way flow — nothing here feeds back into the
private system.
