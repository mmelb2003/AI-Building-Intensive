# Specs

The PRD is the product. A **spec** is one slice of the build — what ships
in this pass, and how you know it is done.

Do not start here. Build the smallest working version from `PRD.md` first.
Create `specs/` in your app after something is on screen.

| File | What it is |
|------|------------|
| `_template.md` | The blank spec. Copy this into **your app** as `specs/_template.md`. |
| `README-seed.md` | The spec index. Copy this into **your app** as `specs/README.md`. |
| `Spec-Example-Loop.md` | A filled spec for Loop (submit + list). Read it to see what "good" looks like. |
| `CHANGELOG.md` | What changed in these pack files. Do not copy this into your app. |

The agent skill that writes and updates specs lives in
`cursor-pack/skills/spec-writing/`. Copy that folder into your app as
`.cursor/skills/spec-writing/` (see `cursor-pack/README.md`).

## How to use (2 minutes)

1. After the first screen works, create a folder named `specs/` in **your app project**.
2. Copy `_template.md` into that folder. Keep the filename.
3. Copy `README-seed.md` into that folder and **rename it** `README.md`.
4. Tell Cursor:

> Copy `.cursor/skills/spec-writing/` from the student cursor-pack if it is not already there. Read `PRD.md` and `DESIGN.md`. Write spec 001 for the slice that is already on screen. Follow the spec-writing skill. Use `specs/_template.md`. Seed from local JSON in `data/`; put new items in localStorage. No database or API keys yet.

Using Loop and want a model? Read `Spec-Example-Loop.md`. Do not paste it in as your spec unless you are actually building Loop and this is the slice you shipped.

## What the agent will do

Each spec is one capability (`001-feedback-submit-list`, `002-theme-dashboard`).
The index in `specs/README.md` is the build log — planned, building, shipped.
Do not edit `PRD.md` to record what shipped. That is what the spec index is for.
