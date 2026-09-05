# PRD

Two files to copy into your app project.

| File | What it is |
|------|------------|
| `PRD-Template.md` | The one-page template. Fill in sections 1–4 (required); 5–8 are optional but make the agent far more accurate. |
| `PRD-Example-Loop.md` | A worked example ("Loop," a feedback board). Read it to see what "good" looks like, or use it as your backup project if you don't have your own idea. |

## How to use (2 minutes)

1. Copy `PRD-Template.md` into **your app project** and rename it `PRD.md`.
2. Fill in at least sections 1–4. Keep it to about one page — bullets and tables, not paragraphs.
3. Tell Cursor:

> Read `PRD.md` and `DESIGN.md`. Follow the workshop rule. Seed from local JSON in `data/`; put new items in localStorage. No database or API keys yet. Do not write a JSON file on the server. Ask me any clarifying questions first, then build the smallest working version of the P0 must-haves in section 4, following the build order.

If you don't have your own idea, copy `PRD-Example-Loop.md` instead and run the same prompt. The look is `DESIGN.md` (Harbor unless you changed the tokens).

After the first screen works, start a spec (see `specs/README.md`). Do not record what shipped by editing this PRD.
