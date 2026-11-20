# Design tokens: Northline Plumbing (FICTIONAL EXAMPLE)

## Inspiration used
- A Copenhagen bike repair shop: generous whitespace, one strong accent colour
- A Melbourne electrician: big phone number in the header, honest pricing table
- Borrowed the *feel* only. No layouts, copy or images copied.

## Colours (all pairs pass WCAG AA)
| Token | Hex | Used for |
|---|---|---|
| --color-bg | #F7F5F0 | Page background (warm off-white) |
| --color-surface | #FFFFFF | Cards |
| --color-text | #1C2430 | Body text |
| --color-text-muted | #4F5B69 | Secondary text |
| --color-brand | #1F4E79 | Brand navy |
| --color-cta | #C2410C | Main buttons (burnt orange) |
| --color-cta-text | #FFFFFF | Text on buttons |

## Typography
- **Headings:** Archivo 700
- **Body:** Inter 400 and 600
- **H1:** 2.75rem / 1.1 desktop, 2rem / 1.15 mobile · **H2:** 2rem / 1.2, 1.5rem mobile · **H3:** 1.25rem / 1.3 · **Body:** 1.0625rem / 1.6

## UI rules
- **Radius:** 10px buttons, 12px cards, 8px inputs
- **Shadows:** cards `0 1px 2px rgba(0,0,0,.06)`, no heavy drop shadows
- **Section padding:** 96px desktop, 56px mobile
- **Max content width:** 72rem
- **Cards:** white, 1px #E4E0D8 border, no hover lift

## CSS variables
```css
:root {
  --color-bg: #F7F5F0;
  --color-surface: #FFFFFF;
  --color-text: #1C2430;
  --color-text-muted: #4F5B69;
  --color-brand: #1F4E79;
  --color-cta: #C2410C;
  --color-cta-text: #FFFFFF;
  --color-border: #E4E0D8;
  --font-heading: "Archivo", system-ui, sans-serif;
  --font-body: "Inter", system-ui, sans-serif;
  --radius-btn: 10px;
  --radius-card: 12px;
  --radius-input: 8px;
  --space-section: 96px;
  --space-section-mobile: 56px;
  --max-width: 72rem;
}
```
