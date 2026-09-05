# Student pack — bootstrap

This zip is a **crate**, not your app. Do not open this folder as the project you will build in.

## You

1. Create a **new empty folder**. In Cursor: **File → New Window → Open** that folder.
2. On GitHub: green **Code** button → **Download ZIP**.
3. Drag the zip (or the unzipped folder) into that empty project.
4. Set the agent to **Composer 2.5**. Paste:

> Read `README.md` inside the zip (or unzipped pack) in this folder. Follow it exactly. This folder is my app.

After setup: fill `PRD.md` sections 1–4, then use the prompt already in that file.

## Agent — do exactly this

There is a student pack in this workspace (`.zip` or unzipped folder). This folder is the app.

**Do not invent a product. Do not add features, APIs, OpenAI, or Neon. Do not write spec 001. Do not git clone.**

1. Unzip if needed. Find `student/`.
2. Copy only:
   - `student/DESIGN.md` → `DESIGN.md`
   - `student/themes/harbor.css` → `themes/harbor.css`
   - `student/cursor-pack/rules/` → `.cursor/rules/`
   - `student/cursor-pack/skills/spec-writing/` → `.cursor/skills/spec-writing/`
   - `student/cursor-pack/skills/session-handoff/` → `.cursor/skills/session-handoff/`
   - `student/.env.example` → `.env`
   - `student/prd/PRD-Template.md` → `PRD.md`
   - `student/specs/_template.md` → `specs/_template.md`
   - `student/specs/README-seed.md` → `specs/README.md`
   - `student/handoff/HANDOFF-Template.md` → `HANDOFF.md`
3. Scaffold the Next.js shell in a subfolder so you do not fight existing files, then move it up:

   `npx create-next-app@latest _next --ts --tailwind --eslint --app --no-src-dir --import-alias "@/*" --use-npm --yes`

   Move `_next/` contents into this folder without overwriting `DESIGN.md`, `PRD.md`, `HANDOFF.md`, `.env`, `.cursor/`, `themes/`, or `specs/`. Delete `_next`.
4. If `package.json` name is `_next` or `next-tmp`, set it to the folder name.
5. `npx shadcn@latest init -d`
6. `npx shadcn@latest add button card input label -y`
7. Paste tokens from `themes/harbor.css` into `app/globals.css` `:root`. Keep imports, `@theme`, and the base layer.
8. Leave `AGENTS.md` and `CLAUDE.md` if Next created them. Do not delete them — `next dev` puts them back.
9. **Delete** the zip and the extracted pack from this project. Do not leave `student/` here.
10. List what you created. **Stop.**

Look is Harbor. To rebrand later, change hex values in `DESIGN.md` and `app/globals.css` `:root`. Do not add a second design file.

Do not copy Loop examples (`PRD-Example-Loop.md`, `Spec-Example-Loop.md`, `HANDOFF-Example-Loop.md`) unless the student is building Loop.
