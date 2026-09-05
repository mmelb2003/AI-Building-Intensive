# Student pack — bootstrap

This zip is a **crate**, not your app. Do not open this folder as the project you will build in.

## You

1. Create a **new empty folder**. In Cursor: **File → New Window → Open** that folder.
2. On GitHub: green **Code** button → **Download ZIP**.
3. Drag the zip (or the unzipped folder) into that empty project.
4. Set the agent to **Composer 2.5**. Paste:

> Read `README.md` inside the zip (or unzipped pack) in this folder. Follow it exactly. This folder is my app.

Keep a copy of the pack in Downloads. You will copy `specs/` and `handoff/` from it after the first screen works.

## Agent — do exactly this

There is a student pack in this workspace (`.zip` or unzipped folder). This folder is the app.

**Do not invent a product. Do not add features, APIs, OpenAI, Neon, specs, or a handoff. Do not git clone.**

1. Unzip if needed. Find `student/`.
2. Copy only:
   - `student/DESIGN.md` → `DESIGN.md`
   - `student/themes/harbor.css` → `themes/harbor.css`
   - `student/cursor-pack/rules/` → `.cursor/rules/`
   - `student/cursor-pack/skills/spec-writing/` → `.cursor/skills/spec-writing/`
   - `student/cursor-pack/skills/session-handoff/` → `.cursor/skills/session-handoff/`
   - `student/.env.example` → `.env`
   - `student/prd/PRD-Template.md` → `PRD.md`
3. Scaffold the Next.js shell in a subfolder so you do not fight existing files, then move it up:

   `npx create-next-app@latest _next --ts --tailwind --eslint --app --no-src-dir --import-alias "@/*" --use-npm --yes`

   Move `_next/` contents into this folder without overwriting `DESIGN.md`, `PRD.md`, `.env`, `.cursor/`, or `themes/`. Delete `_next`.
4. `npx shadcn@latest init -d`
5. `npx shadcn@latest add button card input label -y`
6. Paste tokens from `themes/harbor.css` into `app/globals.css` `:root`. Keep imports, `@theme`, and the base layer.
7. **Delete** the zip and the extracted pack from this project. Do not leave `student/` here.
8. List what you created. **Stop.**

Look is Harbor. To rebrand later, change hex values in `DESIGN.md` and `app/globals.css` `:root`. Do not add a second design file.
