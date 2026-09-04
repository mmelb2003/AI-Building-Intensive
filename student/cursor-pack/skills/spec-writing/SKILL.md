---
name: spec-writing
description: >-
  Load when the user asks to write a spec, plan a delivery slice,
  document what shipped, split a too-big spec, or update spec status.
  Phrases: "write a spec", "plan this slice", "is this spec done".
  Do not load for a PRD, strategy doc, commit message, or a bugfix
  that does not change the contract.
---

# Spec writing

A spec is a **delivery slice**: the smallest unit of work that produces
user-visible (or agent-visible) value and can be marked done with a
checkable list. It sits between strategy and code.

> Strategy answers *why* and *what*.
> Specs answer *what this slice ships* and *how we know it is done*.
> Code is the third layer.

The spec is a **durable contract** for the next agent, not a throwaway
prompt. When code and spec disagree, one of them is wrong on purpose:
amend the spec first (change log), then make the code follow. Never
silently patch either side to hide the drift.

This skill is project-agnostic. Discover the repo's existing `specs/`
conventions before writing. A project overlay wins on extra sections
and status names. One file per slice — not a spec / plan / tasks trio.

---

## When this skill applies

Follow it when the user asks to propose a slice, document what just
shipped, split a chunk that grew too big, or audit code against a spec.

Skip a new spec when the change is a rename, a lint, a behavior-preserving
refactor, or a bugfix that does not change the contract — update the
existing spec's change log instead.

The test: would another agent reading only `specs/NNN-name.md` ship this
slice end-to-end and check it off? If yes, it is a spec.

For the when-to-write table, size calibration, and AI-paced pre-speccing,
read [`references/when-and-size.md`](references/when-and-size.md).

---

## What the model should do

1. **Discover the project overlay.** Look for `specs/_template.md`,
   `specs/README.md`, and a project `.cursor/skills/spec-writing/`.
   If a project template exists, that is the section contract — fill
   it; do not replace it with this skill's template. If the project
   skill renames a status (`pending-founder` for `blocked`) or requires
   extra sections (compliance, push tags), obey those. Find the
   strategy doc (`PRD.md`, `STRATEGY.md`, `mvp-spec.md`, or whatever
   the index already cites). Use the project's real paths and check
   commands, not Next.js / `src/` / `npm` defaults.
2. **Decide whether a new spec is warranted.** If not, update the
   existing change log and stop.
3. **Write done criteria first.** They pull the rest of the spec into
   focus. Then fill every section of the template. If a section does
   not apply, write `n/a — <one-line reason>` — never delete the heading.
4. **Create or update the files.** New project: copy
   [`assets/_template.md`](assets/_template.md) to `specs/_template.md`
   and [`assets/readme-seed.md`](assets/readme-seed.md) to
   `specs/README.md`. New slice: copy the project template (or this
   one) to `specs/NNN-kebab-name.md`, add the index row, set `planned`
   or `building`.
5. **On ship or audit:** walk done criteria against the code, confirm
   the named surfaces exist, run the test plan. Drift is either a code
   change or a dated spec amendment — say which, then do that.

Numbering, status tokens, and `_*.md` companions:
[`references/status-and-files.md`](references/status-and-files.md).

How to write stories, EARS done criteria, constraints, and open questions:
[`references/authoring.md`](references/authoring.md).

---

## Gotchas

- The highest-ROI section is **Constraints (must NOT)**. Agents "improve"
  the slice (new database, extra route, extra library) unless this list
  is concrete. "None" is almost always wrong.
- An open question with no owner is an invitation to guess. Blocking
  items (public API shape, migration, permission, payment, legal copy)
  stop the build.
- Do not invent GitHub Spec Kit's `spec.md` / `plan.md` / `tasks.md`
  split, a constitution file, or a push-tag field the project does not
  already use. Standing rules live in `.cursor/rules/` (or `AGENTS.md`).
- Do not invent HIPAA / counsel / HelpTopic / `src/` sections on a
  project that does not have them. Use **Domain & quality guardrails**
  and write `n/a` when nothing applies.
- Do not edit the strategy/PRD to record delivery state. That is what
  the spec index is for.
- Do not reuse a sequence number, even for a cancelled spec.
- A spec past ~200 lines or ~10 focused work-days is two specs. Split
  it (horizontal or temporal) and leave the original `cancelled` with
  pointers.
- "Spec-then-spec-then-spec" while waiting on a real-world signal is
  planning overhead. A *cohesive* batch that locks a shared contract
  ahead of an imminent build is the opposite — do that.
- Cite the project rule file and section, not a principle ("log
  carefully").
- After any status change, update `specs/README.md` in the same turn.

---

## On-demand resources

- Size, when-to-write, pre-speccing: [`references/when-and-size.md`](references/when-and-size.md).
- Status taxonomy, numbering, special files, overlays: [`references/status-and-files.md`](references/status-and-files.md).
- Stories, done criteria, EARS, constraints, open questions: [`references/authoring.md`](references/authoring.md).
- New slice file: copy [`assets/_template.md`](assets/_template.md).
- New `specs/` folder: also copy [`assets/readme-seed.md`](assets/readme-seed.md).

---

## What this skill is not for

- Not for writing or rewriting a PRD / strategy doc.
- Not for commit messages, PR descriptions, or session handoffs
  (use the `session-handoff` skill to wrap a session).
- Not for a one-line bugfix or refactor that does not change the contract.
