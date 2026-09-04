# Handoff

Session state for the next agent (or you tomorrow). Copy the template into your app as `HANDOFF.md` **after** the first screen works — same timing as `specs/`.

| File | What it is |
|------|------------|
| `HANDOFF-Template.md` | Blank handoff. Copy into **your app** as `HANDOFF.md` and fill it. |
| `HANDOFF-Example-Loop.md` | Worked example for Loop — see what “good” looks like. |

## How to use

1. After something is on screen, copy `HANDOFF-Template.md` into your app root as `HANDOFF.md`.
2. Fill sections 1–3 from `PRD.md` / `DESIGN.md` / the workshop rules (those rarely change).
3. At the end of each work session, tell Cursor:

> Wrap up this session. Update `HANDOFF.md` so the next agent can pick up cleanly.

That loads the **session-handoff** skill (copy it from `cursor-pack/skills/session-handoff/` into `.cursor/skills/` if it is not there yet).

4. Next session, open a **fresh** chat and paste:

> Read `HANDOFF.md` first. Follow the reading order in § 3. Then do the Next session pickup — do not rebuild anything already shipped.

## What gets updated every wrap

**State (rewrite each time):** snapshot date, next-session pickup, § 4 current state, § 5 what’s next, § 8 open external actions, § 13 change log.

**Contracts (rarely touch):** § 1–3, 6, 11, 12 — and only if the product or rails actually changed.

The handoff is **last** in the source-of-truth order. If it disagrees with `workshop.mdc`, `PRD.md`, or a spec, fix the handoff — do not “win” from this file.
