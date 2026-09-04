# Studio

Warm editorial. Cream paper, terracotta ink, serif headlines. Feels like a small studio or magazine, not a tech company.

**Use this when:** education, local services, storytelling, portfolios, community guides.

## Apply (once)

1. Copy this file into your app as `DESIGN.md`.
2. After shadcn init, paste the token values from `themes/studio.css` into the `:root { ... }` block in `app/globals.css` (replace the default token values; keep the rest of the file).
3. Tell Cursor: *Follow `DESIGN.md`. Use theme tokens only (`bg-primary`, `text-muted-foreground`). Do not hardcode colors.*

## Tweak (optional)

Change a hex in `app/globals.css` `:root` — e.g. `--primary` — and the whole app updates. Do not invent new colors inside components. Optional: load Source Serif 4 for headlines via `next/font`.

## Colors
- Background: `#F7F1E8`
- Surface / cards: `#FFFDF8`
- Text: `#2A2118`
- Muted text: `#7A6A58`
- Border: `#E4D6C3`
- Brand: `#C45C26`
- Brand hover: `#A44B1E`
- Brand on color: `#FFFDF8`
- Success: `#3F6B4A`
- Danger: `#9B2C2C`

## Type
- Headlines: Source Serif 4 or Georgia, serif
- Body: Inter or system-ui, sans-serif
- Page title: 34–40px serif, weight 600
- Section title: 24px serif
- Body: 17px sans, line-height 1.6
- Small / meta: 13px, `#7A6A58`

## Shape and space
- Radius: 6px (slight, not pill-shaped)
- Almost no shadows
- Page padding: 28px
- Space between sections: 40px
- Max content width: 720px for reading, 960px for mixed layouts

## Components
- **Nav:** simple text links, no heavy bar, brand color for the active link
- **Primary button:** terracotta, cream text
- **Secondary button:** cream, terracotta border
- **Cards:** cream surface, 1px warm border, no shadow
- **Quotes / callouts:** left terracotta rule, slightly larger serif

## Do
- Let headlines be a little literary
- Keep body text easy to read
- Use brand color sparingly (links, buttons, small marks)

## Don’t
- Cool blue SaaS chrome
- Dark mode
- Huge rounded “app” buttons
- Stock-photo hero with overlay gradient
