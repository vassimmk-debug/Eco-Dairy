# AgriLait — Figma Import Files

## Files included

| File | Screen |
|------|--------|
| 01-homepage.html | Landing page with hero, process flow, features grid |
| 02-dashboard.html | Farm dashboard — KPIs, score rings, charts, alerts |
| 03-ai-advisor.html | AI recommendation engine with priority cards |
| 04-onboarding.html | 8-step farm registration form (Step 1 shown) |
| 05-benchmarking.html | Peer comparison with bar charts and radar visual |
| 06-sustainability.html | Carbon + water footprint + resource efficiency |

---

## How to import into Figma

### Step 1 — Install the plugin
In Figma, go to **Main Menu → Plugins → Browse plugins** and search for:
**"HTML to Design"** by divRIOTS

Install it (free).

### Step 2 — Create a new Figma file
Create a new Design file. Add one page per screen (right-click the page tab → "Add page").
Rename pages: Homepage / Dashboard / AI Advisor / Onboarding / Benchmarking / Sustainability

### Step 3 — Import each file
For each screen:
1. Navigate to the correct Figma page
2. Run the plugin: **Plugins → HTML to Design**
3. Click **"Import HTML file"** (or paste HTML code)
4. Upload the corresponding .html file
5. Click **Import** — the screen appears as editable Figma layers

### Step 4 — Organize frames
After importing:
- Select all imported layers and group them into a frame (A key → draw frame)
- Set frame width to **1440px**
- Apply a background fill of **#F9FAF7**
- Name each frame clearly (e.g. "Homepage — Desktop 1440")

---

## Design system reference

### Color palette
| Token | Hex | Usage |
|-------|-----|-------|
| Green Primary | #2D6A2E | CTAs, active states, scores |
| Green Medium | #3D8A3E | Hover states, secondary actions |
| Green Light | #4CAF50 | Accent, pills, positive trends |
| Green Surface | #E8F5E9 | Card backgrounds, badges |
| Teal | #1B6B5E | Sustainability accents |
| Earth | #D4790A | Warning states, medium priority |
| Red | #C0392B | Alerts, negative trends |
| Blue | #1A3C8B | Economic score |
| Ink | #0E1A0F | Primary text |
| Ink 2 | #3A5A3B | Secondary text |
| Ink 3 | #6B8E6C | Tertiary text, labels |
| Surface | #F9FAF7 | Page background |
| Surface 2 | #F0F4ED | Section backgrounds |

### Typography
- **Display / Headlines**: DM Serif Display (serif, italic for emphasis)
- **UI / Body**: Inter (400 regular, 500 medium, 600 semi-bold)
- **Scale**: 48px hero → 38px section → 22px card → 16px body → 13px small → 11px label

### Spacing
- Page padding: 32px (compact) / 64px (homepage)
- Card padding: 20–28px
- Grid gap: 14–20px
- Component gap: 8–16px

### Border radius
- Cards: 12px
- Buttons: 7–9px
- Chips/badges: 5–6px
- Score rings: circular

---

## Notes
- All screens are 1440px wide (desktop)
- Fonts load from Google Fonts — ensure network access during import
- Charts use SVG/CSS bar visuals (no JavaScript needed)
- For full interactivity, use the HTML artifact version in Claude
