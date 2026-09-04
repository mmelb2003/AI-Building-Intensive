# Pick a look for your app

Everything for looks lives in **this folder**.

1. Open `index.html` in a browser and click tabs until you like one.
2. Copy that look’s `.md` into **your app** as `DESIGN.md`.
3. After shadcn init, paste tokens from the matching `themes/*.css` into `app/globals.css` `:root`.

**Inside your app, `DESIGN.md` is the only source of truth for the look.** Do not restate Harbor / Studio / etc. in `PRD.md` or specs.

| Guide | Theme tokens | Name | Feel | Best for |
|------|--------------|------|------|----------|
| `01-harbor.md` | `themes/harbor.css` | **Harbor** | Clean blue SaaS, lots of space | Tools, dashboards, work apps |
| `02-studio.md` | `themes/studio.css` | **Studio** | Warm paper, serif headlines | Stories, education, local services |
| `03-console.md` | `themes/console.css` | **Console** | Dark screen, cyan accent | Dev tools, data, “serious product” |
| `04-garden.md` | `themes/garden.css` | **Garden** | Soft sage, rounded, friendly | Health, community, consumer apps |
| `05-signal.md` | `themes/signal.css` | **Signal** | White, black, one orange, sharp edges | Archives, research, lists, catalogs |

If you cannot decide, use **Harbor**.

## Want to change the look later?

Edit hex values in `app/globals.css` `:root` (for example `--primary`). Save. The UI should update without rewriting components.
