# PRD

Bootstrap already copied `PRD-Template.md` into the app as `PRD.md`. Fill sections 1–4 there. Do not copy this folder into the app.

| File | What it is |
|------|------------|
| `PRD-Template.md` | The one-page template (already `PRD.md` in the app). |
| `PRD-Example-Loop.md` | Worked example. Read it, or use it as `PRD.md` if you are building Loop. |

**Optional — second opinion before you build.** Open a **new chat**, switch to **Opus** (or another high-reasoning model), and say:

> Review this PRD before we build.

Read **Fix these 3.** Keep, change, or ignore them. Switch that model off. Apply accepted edits with **Grok**, then build with **Composer 2.5**.

Then tell Cursor:

> Read `PRD.md` and `DESIGN.md`. Follow the workshop rule. Seed from local JSON in `data/`; put new items in localStorage. No database or API keys yet. Do not write a JSON file on the server. Ask me any clarifying questions first, then build the smallest working version of the P0 must-haves in section 4, following the build order.

After the first screen works, write spec 001 (see `specs/README.md`). Do not record what shipped by editing the PRD.
