# Source: /ai-act/gp

[← The EU AI Act](/ai-act)

For VC, PE and private credit general partners · Last reviewed June 2026

# The EU AI Act, for GPs

What a fund manager actually has to do — for internal tools, for portfolio-company and borrower DD, and for the agents now running your data room.

Share article →

## Where you actually sit

As a GP you are almost always a *deployer*, not a provider. Sourcing, screening, IC drafting and monitoring sit in **minimal or limited risk** under the Act. The real exposure is two steps removed from your laptop — and it splits cleanly along strategy.

**VC and PE — risk travels with the deal.** Equity-backed companies that build AI which **scores or ranks people** (CV screening, employee assessment, fraud/credit decisions) sit in the high-risk tier. The obligations don't disappear at close — they follow the cap table.[Annex III](https://ai-act-service-desk.ec.europa.eu/en/ai-act/annex-3) is the reference. It does not matter where your fund is domiciled: any portfolio company selling into the EU pulls you into scope.

**Private credit — you may be the high-risk deployer.** AI underwriting models that score individuals or SMEs are a textbook [Annex III](https://ai-act-service-desk.ec.europa.eu/en/ai-act/annex-3) high-risk case. If a borrower runs that model, it's their obligation. If the **fund itself runs it** — direct lending, NAV, ABL with an in-house scoring layer — the fund is operating as a high-risk deployer in its own right: different governance stack, conformity assessment, logging, human oversight.

**Internal agents — same tier, wider surface.** Claude Code, OpenAI Codex, n8n / LangGraph workflows reading the data room end-to-end and drafting memos don't change your tier, but they widen the confidentiality surface and multiply the places a human-in-the-loop checkpoint needs to sit.

It does not matter where your fund is domiciled: any portfolio company or borrower selling into the EU, or any LP receiving your output in the EU, pulls you into scope.

## Where you can get burned

- **Portfolio-company DD that doesn't ask the AI Act question.** A clean SaaS company can ship a CV-screener as a feature update post-close and flip into the high-risk tier overnight. You won't have priced this.
- **Agents drifting into ranking people.** A screening workflow that started as "summarise this founder's deck" becomes "score these 200 founders on coachability." Once it ranks identifiable individuals, the tier changes.
- **Confidential portfolio data in personal LLM accounts.** Confidential Information Memorandum (CIM) pasted into a personal ChatGPT account vs the same task on an enterprise tenancy with zero-retention is the same workflow, very different exposure — and very different posture in front of an LP.
- **No AI-literacy paper trail.** The Feb 2025 duty is the easiest box to tick and the easiest one for an LP to ask about. Don't be caught without sign-off sheets.
- **Private-credit underwriting models built in-house.** If the fund itself runs an AI scoring model on borrowers — including SME borrowers — that's the fund operating as a high-risk deployer, not minimal-risk. The model is still commercially viable — the change is that the fund must accept the full high-risk deployer obligations (conformity assessment, logging, human oversight) rather than treating it as minimal-risk.

## Monday morning

- —**Inventory every AI tool** the team touches — browser ChatGPT, M365 Copilot, Claude, Cursor, Codex, autonomous agents. You can't classify what you can't see.
- —**Run AI-literacy training** (60 minutes, sign-off, refreshed annually). In force since Feb 2025.
- —**Add an AI Act block to your DD questionnaire** for every new investment or new borrower. Which tier, conformity assessment if high-risk, GPAI provider underneath, training-data provenance, EU deployment footprint.
- —**Govern your agents explicitly.** For each agentic workflow: scope, data access, human checkpoints, kill switch. One page per agent.
- —**Vendor contracts:** zero-retention, EU data residency where possible, sub-processors disclosed, right to audit.
- —**Name a single owner** — usually the COO or General Counsel — for the inventory, the policy, and the regulator relationship.

[← The EU AI Act](/ai-act)

Read as[LPs across fund commitments, co-investments and secondaries](/ai-act/lp)·[family-office principals and COOs](/ai-act/family-office)·[CIOs and portfolio managers](/ai-act/cio)·[individuals managing their own money](/ai-act/hnwi)·[independent advisors and ad-hoc wealth services](/ai-act/advisor)

Sources[Reg (EU) 2024/1689 (EUR-Lex)](https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng)·[Art. 4 — AI literacy](https://ai-act-service-desk.ec.europa.eu/en/ai-act/article-4)·[Art. 5 — Prohibited practices](https://ai-act-service-desk.ec.europa.eu/en/ai-act/article-5)·[Art. 6 + Annex III — High-risk](https://ai-act-service-desk.ec.europa.eu/en/ai-act/annex-3)·[Art. 99 — Penalties](https://ai-act-service-desk.ec.europa.eu/en/ai-act/article-99)

Related reading

[Data leakage in AI workflows — for gps — vc, pe & private credit →](/ai-act/articles/data-leakage/gp)

The six leak vectors, the AI Act and GDPR hooks for each, and a precautionary checklist tailored to your lane. Or read the [overview](/ai-act/articles/data-leakage).

Share article →

Found this useful? Come say hello on [LinkedIn](https://www.linkedin.com/in/ieva-rubule/).
