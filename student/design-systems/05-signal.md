# Signal

Bare and exact. Near-white, plain black type, one orange, 1px hairlines, no rounded corners. Feels like a research archive or catalog, not a startup landing page.

**Use this when:** collections, research, lists, libraries, wikis, anything that should feel honest and un-designed.

## Apply (once)

1. Copy this file into your app as `DESIGN.md`.
2. After shadcn init, paste the token values from `themes/signal.css` into the `:root { ... }` block in `app/globals.css` (replace the default token values; keep the rest of the file). `--radius` is `0` — keep corners sharp.
3. Tell Cursor: *Follow `DESIGN.md`. Use theme tokens only (`bg-primary`, `text-muted-foreground`). Do not hardcode colors. No rounded corners.*

## Tweak (optional)

Change a hex in `app/globals.css` `:root` — e.g. `--primary` — and the whole app updates. Do not invent new colors inside components.

## Colors
- Background: `#FAFAFA`
- Surface / cards: `#FFFFFF`
- Text: `#000000`
- Muted text: `#666666`
- Faint text: `#999999`
- Border: `#DDDDDD`
- Brand / links: `#FF6600`
- Brand hover: `#E85A00`
- Brand on color: `#FFFFFF`
- Success: `#2D6A4F`
- Danger: `#8B1A1A`

## Type
- Font: Inter, Helvetica Neue, Helvetica, Arial, sans-serif
- One family only — no serif, no display font
- Page title: 32px, weight 500
- Section title: 18px, weight 500
- Body: 14px, weight 400, line-height 1.45
- Meta / counts: 13px, `#666666`

## Shape and space
- Radius: **0px** everywhere (buttons, cards, inputs)
- No shadows, no gradients, no blur
- 1px `#DDDDDD` borders define every block
- Dense: 16px page padding, 16–24px between sections
- Max content width: 1040px
- Grid of blocks, not floating cards

## Components
- **Nav:** text links, orange for current page, hairline underneath
- **Primary button:** orange rectangle, white text, no radius
- **Secondary button:** white, 1px border, black text
- **Cards / blocks:** white, 1px border, no shadow, flush in a grid
- **Links:** orange, underline on hover only
- **Lists:** compact, meta text in muted gray

## Do
- Let the grid and type do the work
- Use orange only for links, actions, and the mark
- Keep titles modest — not giant marketing type

## Don’t
- Rounded corners
- Drop shadows or glass
- Blue SaaS chrome
- Hero images with overlays
- Extra accent colors
