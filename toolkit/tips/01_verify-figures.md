# How to make AI verify figures instead of inventing them

*A practitioner's note from building an AI-assisted investment-research process.
Last reviewed: July 2026. Works with any capable AI assistant; nothing here is
tool-specific. Not investment advice.*

The single biggest risk in AI-assisted research is not laziness — it is
**confidence**. An AI will give you a wrong revenue figure in the same fluent
sentence as a right one. These are the five rules I use so that numbers in my
notes can be trusted, in rising order of effort:

## 1. Filings first, aggregators second — and say so

Give the AI the primary source (the annual report, the results announcement)
and instruct it to cite the page for every material figure. Data screens and
aggregators are allowed for assembly, but the standing rule is: **when an
aggregator and a filing disagree, the filing wins.** No source page, no claim.

## 2. Label every figure — Disclosed / Inferred / Estimated

Three labels, applied to every material number:

- **[Disclosed]** — taken directly from a filing, as reported.
- **[Inferred]** — derived from disclosed figures (a margin, a growth rate).
  The arithmetic is yours; the inputs are filed.
- **[Estimated]** — an estimate, and it says so.

The labels force the AI (and you) to know which kind of number each one is —
and they make the finished note auditable by any reader.

## 3. Make "N/A" an acceptable answer

Tell the AI explicitly: *if a figure cannot be traced to a source, write N/A —
do not approximate it.* Without this instruction, models fill gaps with
plausible-looking numbers, which is the worst failure mode in financial work:
wrong but not obviously wrong.

## 4. Derive ratios; never quote them

Margins, returns, and growth rates get computed from the filed numerator and
denominator — never copied from a screener, where definitions differ silently
(is that operating margin before or after one-offs? whose "net debt"?). If the
AI shows the derivation, a reviewer can check it in seconds.

## 5. Spot-check the headline numbers against the document itself

Before anything ships, take the two or three figures the whole argument rests
on and find them **on the page** of the actual filing — not in the AI's
summary of it. In my process this is a separate, fresh pass, done as if
checking a stranger's work. It has caught real discrepancies; that is the
point.

---

**The mindset that ties it together:** treat the AI as a brilliant junior
analyst with no fear of being wrong. Everything it produces is a draft until a
source page confirms it. The discipline is cheap — a few standing instructions
and one verification pass — and it is the difference between research you can
publish and text that merely sounds like research.

*From the process behind [ievarubule.ai](https://ievarubule.ai) — where every
published note labels its figures and ships its chart data.*
