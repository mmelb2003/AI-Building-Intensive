# Student pack

Everything you need to set up your project and start building.

| File | What it is |
|------|------------|
| `design-systems/` | Looks + preview — open `index.html`, then copy **one** `.md` into your app as `DESIGN.md` (+ tokens into `globals.css`) |
| `cursor-pack/` | Workshop rules + skills — copy `rules/` and `skills/` so the agent stays on the rails |
| `.env.example` | Env template — copy into your app as `.env`; paste your OpenAI key when you add AI (model stays hardcoded) |
| `prd/` | The PRD template + a worked example ("Loop") — copy one into your app as `PRD.md` |
| `specs/` | Spec template, index seed, and a Loop example — copy these into your app **after** the first screen works |
| `handoff/` | Handoff template + Loop example — copy into your app as `HANDOFF.md` **after** the first screen works |

**Look contract:** After you copy a look, **`DESIGN.md` in your app** is the only place that defines the visual system. `PRD.md` and specs just say “follow `DESIGN.md`.”

## Pick a look (2 minutes)

1. Open `design-systems/index.html` in Chrome.
2. Click the tabs until you like one.
3. Copy that `.md` from `design-systems/` into **your app project** and rename it `DESIGN.md`. That file is now your look.
4. Copy everything in `cursor-pack/rules/` into **your app project** as `.cursor/rules/`, and every folder in `cursor-pack/skills/` into `.cursor/skills/` (see `cursor-pack/README.md`).
5. Copy `.env.example` into **your app project** as `.env`. Leave the key blank until you add an AI feature — then paste your OpenAI API key. Do not commit `.env`.
6. Copy `prd/PRD-Template.md` into **your app project** as `PRD.md` and fill in sections 1–4 (see `prd/README.md`). No idea yet? Use `prd/PRD-Example-Loop.md` instead.
7. Tell Cursor: *Read `PRD.md` and `DESIGN.md`. Follow the workshop rules. After shadcn init, apply the theme tokens for this `DESIGN.md` into `app/globals.css`. Seed from local JSON in `data/`; put new items in localStorage. No database or API keys yet.*

If you cannot decide, use **Harbor** (`design-systems/01-harbor.md` + `themes/harbor.css`).

Later, to rebrand: change a hex in `app/globals.css` `:root` (see `design-systems/README.md`).

## After the first screen works

Do not create `specs/` or `HANDOFF.md` on day one. Once something is on screen:

1. Copy `specs/_template.md` and `specs/README-seed.md` into **your app** as `specs/_template.md` and `specs/README.md` (see `specs/README.md`).
2. Copy `handoff/HANDOFF-Template.md` into **your app** as `HANDOFF.md` (see `handoff/README.md`).
3. Tell Cursor: *Write spec 001 for the slice that is already on screen. Follow the spec-writing skill. Use `specs/_template.md`.*

## End of a work session

Tell Cursor:

> Wrap up this session. Update `HANDOFF.md` so the next agent can pick up cleanly.

Next time, open a **fresh** chat and paste:

> Read `HANDOFF.md` first. Follow the reading order in § 3. Then do the Next session pickup — do not rebuild anything already shipped.
