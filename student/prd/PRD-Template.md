# PRD — [Your Product Name]

**Author:** [name]  ·  **Date:** [YYYY-MM-DD]  ·  **Version:** 0.1

> **How to use this in the workshop**
> - Fill in **sections 1–4** (required). Sections **5–8** are optional but make the agent far more accurate.
> - Keep it to about **one page**. Use bullets and tables, not paragraphs — agents parse structure better than prose.
> - **Be specific and measurable.** Replace vague words ("nice", "intuitive", "fast") with numbers and observable behavior.
> - **Every requirement gets an acceptance criterion** the agent (or you) can actually check.
> - Mark anything you're guessing with **`[ASSUMPTION]`** — don't invent facts or numbers.
> - Save this file in your project as `PRD.md`, then tell Cursor:
>   *"Read `PRD.md` and `DESIGN.md`. Follow the workshop rule. Use local JSON in `data/` for now — no database or API keys. Ask me any clarifying questions first, then build the smallest version that tests the riskiest assumption in section 3."*
>
> *Sections map to the **Lean Product Process**: target customer → underserved needs → value → MVP feature set.*

---

## 1. Product Summary
*What is it, who is it for, and what does it help them do?*

- **One-liner:** For _[target customer]_ who _[need]_, **[product]** is a _[category]_ that _[key benefit]_.
- **TL;DR (2–4 sentences):** What we're building, for whom, and what counts as success.

## 2. Target Customer  *(Lean Product Process: Target Customer)*
*Describe the person. Separate the **buyer / relationship owner** from the **user** if they differ.*

- **User:**
- **Buyer / decision-maker (if different):**
- **Top 3–5 defining attributes** (demographic, psychographic, behavioral, needs):
  1.
  2.
  3.

## 3. Customer Problems & the Bet  *(Lean Product Process: Underserved Needs → Value)*
*List the top problems, ideally as a real quote in the customer's own words.*

1. "…"
2. "…"
3. "…"

- **Riskiest assumption** (if this is wrong, the idea fails):
  > …
- **The bet (falsifiable):** We believe _[building this]_ will cause _[outcome]_ for _[user]_. **We'll know we're right if _[observable signal / number]_.**

## 4. Product Requirements / Functionality  *(Lean Product Process: MVP Feature Set)*

**Key user stories** — *As a [user], I want [action] so that [outcome].*
- As a …, I want … so that …
- As a …, I want … so that …

**Must-haves for v1** — number them, set a priority, and give each a checkable acceptance criterion:

| ID | Requirement | Priority | Acceptance criterion (observable / measurable) |
|----|-------------|----------|------------------------------------------------|
| R1 |  | P0 | e.g., "A new user completes signup in < 60s with no console errors." |
| R2 |  | P0 |  |
| R3 |  | P1 |  |

*(P0 = must ship for v1 · P1 = should · P2 = nice-to-have.)*

**Build order** (agents do best in sequence): 1) local JSON in `data/` →  2) core action →  3) UI →  4) extras. Neon, APIs, and OpenAI come in later class sessions — do not add them now.

**Explicitly NOT in v1 (non-goals):**
- …
- …

**Do NOT change / keep working** (fill in only when iterating on an existing build):
- …

## 5. Data Model *(optional)*
*What objects/records must the app store, with key fields and how they relate? These names are the JSON now and the Neon table later — keep them stable.*

- **[Object]** — fields: … · start in `data/[object].json` · relates to: …
- **[Object]** — fields: … · start in `data/[object].json` · relates to: …

## 6. Guidance on User Experience *(optional)*
- **Main user flow** (4–7 steps, first visit → core value): 1 → 2 → 3 …
- **Error / empty states:** *e.g., "show an inline message with a retry button; never a blank screen."*
- **Visual aesthetic:** *Follow the design system in `DESIGN.md`* (pick one from `design-systems/` — Harbor, Studio, Console, Garden, Signal).

## 7. Guidance on Tech Stack / Components *(optional)*
*Pick the product. The workshop rule already locks the stack, secrets, and scope. Add only don'ts that are about **this** product.*

- **Course default:** Next.js + React + Tailwind + shadcn/ui, deploy on Vercel. Start on local JSON in `data/`. Neon and OpenAI come later.
- **My preferences / must-use:**
- **Must-avoid** (product-specific): *e.g., "no modals for the main action," "no paid third-party APIs."*

## 8. Other Info & Open Questions *(optional)*
- **Constraints / deadlines:**
- **Products I admire (as references):**
- **Open questions to resolve:** *(mark guesses with `[ASSUMPTION]`)*

---
<sub>**AI Building Intensive — Part 1: Rapid Prototyping with AI** · PRD template<br/>
Created by **Melanie Brewer** · melaniebbrewer@gmail.com</sub>
