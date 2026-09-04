# Spec NNN — [Capability name in sentence case]

| Field | Value |
|---|---|
| **Status** | `planned` |
| **Owner** | [person or agent] |
| **Started** | YYYY-MM-DD |
| **Done** | — |
| **Strategy ref** | `[strategy-doc] § [X]` or `n/a — no strategy doc` |

> [One sentence. What this slice delivers.]

---

## 1. What ships when this is done

[One short paragraph. What can the user or the next agent do now that
they could not before? Name any artifact (route, report, integration)
in the words the user will see.]

## 2. User stories

2–4 stories. Primary persona plus one secondary where the need diverges.

- **As a [persona]**, when I [trigger], I need [job] so I can [observable outcome].
- **As a [secondary persona]**, when I [trigger], I need [job] so I can [observable outcome].

## 3. Surfaces

Concrete paths and URLs this spec adds or materially touches. Use the
project's real tree — do not invent `src/` or a framework.

- User-facing: `[/route or screen]`
- Code: `[path]`
- APIs / actions: `[method + path or exported name]`
- Env vars: `[NAME]` (server-only unless the project marks it public)

## 4. Done criteria

Independently verifiable. 5–12 boxes. Write these first. Event, state,
and failure boxes use EARS (WHEN / WHILE / IF … THE [system] SHALL).
Include at least one unwanted-behavior box.

- [ ] [Most important check — command, URL state, or response shape]
- [ ] [WHEN / IF … THE [system] SHALL …]
- [ ] [Unwanted behavior / empty / outage / malformed input]
- [ ] [Project check command the repo already runs]

## 5. Constraints (must NOT)

What this slice must not touch, add, or change.

- [Do not add …]
- [Do not change … — locked by spec NNN]
- [Do not touch files outside …]
- [Cite `.cursor/rules/[file].mdc` § "[section]" where a standing rule applies]

## 6. Out of scope (for this spec)

Adjacent capabilities this slice will not ship. Point at where they live.

- [Thing] — see spec `NNN-name.md`
- [Thing] — future spec, unassigned
- [Thing] — will not build

## 7. Dependencies

Mark **Blocking** vs **Nice-to-have**.

- **Blocking:** spec `NNN-name.md` (`shipped` / `building` / `planned`)
- **Blocking:** `[env var or external decision]`
- **Nice-to-have:** spec `NNN-name.md` — improves this slice, not required

## 8. Open questions

| Question | Owner | Blocking? |
|---|---|---|
| [undecided thing] | [named person or role] | yes / no |
| n/a — no open questions | — | — |

## 9. Architecture notes

Load-bearing decisions only. Persistence shape, integration contract,
what this deletes, security posture. Link `_data-shapes.md` or a rule
file instead of restating them.

- [Note, or `n/a — no new architectural decisions`]

## 10. Domain & quality guardrails

Standing project rules that apply **to this slice**. Cite file + surface.
Default if none:

`n/a — no project domain-rule file applies to this slice.`

- Security / privacy / compliance: [rule file § section — where it applies]
- Copy: [rule file § section]
- Quality bar: [a11y / performance / i18n only if this slice owns it]

## 11. Test plan

How § 4 is proven. Use the project's real commands.

- [typecheck / lint / test / build — whatever this repo runs]
- Manual: load `[URL or entrypoint]` at [viewports the project cares about]
- [Any accessibility or visual check the project already uses]

## 12. Change log

| Date | Change |
|---|---|
| YYYY-MM-DD | Spec created. |
