# Garden

Soft, friendly, calm. Sage and cream, rounded corners, gentle cards. Feels like a consumer app people would actually enjoy opening.

**Use this when:** health, wellness, community, family, volunteering, anything human and low-stress.

## Apply (once)

1. Copy this file into your app as `DESIGN.md`.
2. After shadcn init, paste the token values from `themes/garden.css` into the `:root { ... }` block in `app/globals.css` (replace the default token values; keep the rest of the file).
3. Tell Cursor: *Follow `DESIGN.md`. Use theme tokens only (`bg-primary`, `text-muted-foreground`). Do not hardcode colors. Pill-shaped primary buttons are OK.*

## Tweak (optional)

Change a hex in `app/globals.css` `:root` — e.g. `--primary` — and the whole app updates. Do not invent new colors inside components. Optional: load Plus Jakarta Sans via `next/font`.

## Colors
- Background: `#F4F7F2`
- Surface / cards: `#FFFFFF`
- Text: `#1F2A1C`
- Muted text: `#5E6B59`
- Border: `#D7E0D2`
- Brand: `#3F6F4A`
- Brand hover: `#335A3C`
- Brand on color: `#FFFFFF`
- Soft accent: `#E7F0E3`
- Success: `#3F6F4A`
- Danger: `#B4534B`

## Type
- Font: Plus Jakarta Sans, Nunito, or Inter — humanist sans
- Page title: 30px, weight 700
- Section title: 20px, weight 600
- Body: 16px, weight 400, line-height 1.55
- Small / meta: 13px, `#5E6B59`

## Shape and space
- Radius: 16px on cards, 999px (pill) on primary buttons and chips
- Soft shadow: `0 8px 24px rgba(31,42,28,0.06)`
- Page padding: 24px
- Space between sections: 28px
- Max content width: 960px
- Comfortable tap targets (min 44px)

## Components
- **Nav:** simple top bar or bottom tabs on small screens; no dense admin sidebar
- **Primary button:** sage pill, white text
- **Secondary button:** white pill, sage border
- **Cards:** white, rounded, soft shadow, generous padding (20px)
- **Empty states:** short friendly sentence, not an error dump
- **Avatars / chips:** circular, soft accent background

## Do
- Make it feel kind and unhurried
- Use the soft accent green for selected states and tags
- Keep copy short and human

## Don’t
- Harsh red error walls
- Sharp 0px corners
- Dark mode or neon
- Tiny dense tables as the first screen
