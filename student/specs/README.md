# Specs

The PRD is the product. A **spec** is one slice of the build — what ships
in this pass, and how you know it is done.

Bootstrap already put `_template.md` and `README.md` (from `README-seed.md`)
in the app as `specs/`. Do not copy this folder again. Do not write spec 001
until a screen is on and the student asks.

| File | What it is |
|------|------------|
| `_template.md` | The blank spec (already in the app). |
| `README-seed.md` | The spec index (already `specs/README.md` in the app). |
| `Spec-Example-Loop.md` | Filled spec for Loop. Read it; do not paste it in unless you shipped that slice. |

Once something is on screen, tell Cursor:

> Write spec 001 for the slice that is already on screen. Follow the spec-writing skill. Use `specs/_template.md`. Seed from local JSON in `data/`; put new items in localStorage. No database or API keys yet.

**Optional — second opinion before the next build.** Open a **new chat**, switch to **Opus** (or another high-reasoning model), and say:

> Review this spec before we build.

Each spec is one capability (`001-feedback-submit-list`, `002-theme-dashboard`).
The index in `specs/README.md` is the build log. Do not edit `PRD.md` to record what shipped.
