# Cursor pack

One file that keeps the agent on the rails. Copy it into your app — same idea as `DESIGN.md`.

You do not need to understand “rules” yet. Just put the file in the right place.

## How to use (2 minutes)

1. In your app project, create a folder named `.cursor/rules/` (the dot at the front matters).
2. Copy `rules/workshop.mdc` into that folder. Keep the filename `workshop.mdc`.
3. Then tell Cursor:

> Read `DESIGN.md`. Follow the workshop rule. Build the smallest version of this app.

If creating the folder feels fiddly, paste this instead:

> Create `.cursor/rules/` and copy `workshop.mdc` from the student cursor-pack into it. Then follow that rule and `DESIGN.md`.

## What’s in the file (for later)

The agent will always: use the course stack (Next.js + Vercel), follow `DESIGN.md`, start from local JSON in `data/` (no database or API keys yet), call third-party APIs and keep secrets on the server (never from the browser), and build only what your PRD asks for.
