# Cursor pack

Files that keep the agent on the rails. Copy them into your app — same
idea as `DESIGN.md`.

You do not need to understand “rules” or “skills” yet. Just put the
files in the right place.

## How to use (2 minutes)

1. In your app project, create `.cursor/rules/` and `.cursor/skills/`
   (the dot at the front matters).
2. Copy **both** files from `rules/` into `.cursor/rules/`. Keep the
   filenames `workshop.mdc` and `folders.mdc`.
3. Copy **each** folder from `skills/` into `.cursor/skills/`
   (`spec-writing/` and `session-handoff/`). Keep the folder names.
4. Then tell Cursor:

> Read `DESIGN.md`. Follow the workshop rules. Build the smallest version of this app.

If creating the folders feels fiddly, paste this instead:

> Create `.cursor/rules/` and `.cursor/skills/`. Copy every file from the student cursor-pack `rules/` folder into `.cursor/rules/`. Copy every folder from `skills/` into `.cursor/skills/`. Then follow those rules and `DESIGN.md`.

## What’s in the files (for later)

| File | The agent will always |
|------|------------------------|
| `rules/workshop.mdc` | Use the course stack (Next.js + Vercel), follow `DESIGN.md`, apply theme tokens in `app/globals.css`, use semantic colors (no hardcoded hex), seed from local JSON in `data/` and put new items in localStorage (no database or API keys yet), call third-party APIs and keep secrets on the server (never from the browser), hardcode OpenAI as `gpt-4o-mini` with only `OPENAI_API_KEY` in `.env`, and build only what your PRD asks for. |
| `rules/folders.mdc` | Put every new file in the default project map (`app/`, `components/`, `lib/`, `data/`, plus `PRD.md` / `DESIGN.md` / `HANDOFF.md` / `specs/` at the root). No `src/`. No empty folders. |
| `skills/spec-writing/` | After the first screen is up: write one spec per slice, keep `specs/README.md` current, and treat the spec as the contract — not a throwaway prompt. |
| `skills/session-handoff/` | End of a work block: update `HANDOFF.md` so a fresh chat can pick up without rebuilding what already shipped. |
