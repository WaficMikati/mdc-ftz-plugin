---
name: ftz-knowledge-base
description: Use this skill whenever the user asks about U.S. foreign-trade zones (FTZs, subzones, zonas francas) or Miami Dade College's FTZ Specialist Certificate courses, even if they don't say 'FTZ' and even if you think you already know the answer. This covers zone status, admission of merchandise, inventory control and recordkeeping, annual reconciliation, CBP forms used in zones (214, 216, 7501, 7512), transfers, penalties, FTZ Board rules, 19 CFR Part 146, 15 CFR Part 400 and the CBP FTZ Manual. The skill supplies what general knowledge can't: the current regulation text with exact citations and the course materials.
---

# Miami Dade FTZ knowledge base

The FTZ connector (tools `search_ftz_knowledge`, `get_regulation_section`, `get_manual_section`, `get_document`, `reconciliation_deadlines`, `zone_status_guide`, `list_sources`) holds the authoritative sources for this subject: the current text of 19 CFR Part 146 and 15 CFR Part 400 (refreshed daily from eCFR), the CBP Foreign-Trade Zones Manual (2011 edition), CBP forms and directives, and the course materials. Answers in this subject must come from these sources, because students and FTZ operators rely on the exact rule and its citation.

## Workflow

1. **Search before answering**, even when you already know the answer. Call `search_ftz_knowledge` with the question in plain language. For a section that's cut off or needs the full rule, call `get_regulation_section` or `get_manual_section`.
2. **Use the specialised tools:**
   - when the reconciliation report or certification letter is due → `reconciliation_deadlines` (exact date arithmetic, skips weekends and federal holidays)
   - which zone status applies, or how the statuses compare → `zone_status_guide`, then apply its steps to the user's facts and ask for any fact that's missing
   - what the knowledge base contains and how current it is → `list_sources`
3. **Answer from the results only.**
   - Cite each claim with the citation of the result that states it, exactly as written on the result's first line (for example "CBP FTZ Manual (2011) › Chapter 8 Operations in Zones › § 8.2 Storage Conditions › pp. 101–102").
   - If you link a citation, use the URL printed with that same passage.
   - Never complete a passage that ends mid-sentence; read the full section instead.
4. **When the results don't cover the question, say so.** Don't supply specific rules, rates, deadlines, form numbers, tariff codes or citations from memory. Point the user to the official source: the USITC Harmonized Tariff Schedule (hts.usitc.gov) for duty rates, CBP CROSS for rulings, the CBP port director or the FTZ Board for zone-specific decisions.
5. **Source precedence.** The current regulations (19 CFR 146, 15 CFR 400) take precedence over the 2011 Manual and the course slides. The Manual's references to FTZ Board rules can be out of date (it cites the antidumping rule as 15 CFR 400.33(b); it is now 15 CFR 400.13(c)(2)), so cite current Part 400 text when it's available, and mention the Manual's 2011 date when you rely on it.
6. Answer in the user's language.

## Not legal advice

This is study and reference material. For a real compliance decision, tell the user to confirm with the cited section, their CBP port director, or a licensed customs broker.
