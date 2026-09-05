# Handoff

Bootstrap already copied `HANDOFF-Template.md` into the app as `HANDOFF.md`.
Do not copy this folder into the app. Do not fill the handoff until something is on screen.

| File | What it is |
|------|------------|
| `HANDOFF-Template.md` | Blank handoff (already `HANDOFF.md` in the app). |
| `HANDOFF-Example-Loop.md` | Worked example. Read it; do not copy it unless you are building Loop. |

End of a work session:

> Wrap up this session. Update `HANDOFF.md` so the next agent can pick up cleanly.

Next session, open a **fresh** chat and paste:

> Read `HANDOFF.md` first. Follow the reading order in § 3. Then do the Next session pickup — do not rebuild anything already shipped.

The handoff is **last** in the source-of-truth order. If it disagrees with `workshop.mdc`, `PRD.md`, or a spec, fix the handoff.
