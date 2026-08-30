# Ai Lab(h) - Prompt se Portfolio Tak

Not an AI workshop — an investment discipline workshop, using AI

This design system was generated mechanically from the onboarding brand form — no AI was involved. Every token in `styles.css` traces to a form input or a documented default, so it is a faithful starting point, not an interpretation. Edit `styles.css` to retune the look; keep this guide in step with what the CSS actually does.

## How to use this

- Link the one stylesheet from every page — `<link rel="stylesheet" href="styles.css">` (adjust the relative path) — and take every color, font, spacing, radius and shadow from its variables (`var(--color-*)`, `var(--font-*)`, `var(--space-*)`, `var(--radius-*)`, `var(--shadow-*)`). Never hard-code a hex, a font name or a px value the tokens already carry.
- Each color role carries a 100-900 tonal ramp (`--color-neutral-100` … `--color-accent-2-900`) generated in OKLCH on a shared perceptual lightness scale. On this dark ground use the dark steps (700-900) for tinted fills, hovers and subtle borders, 500 as a role base, and the light steps (100-300) for text on those tints.
- For elevation use `--shadow-sm/md/lg` (already tuned to the ground) rather than ad-hoc box-shadows.

## Color

Page ground `#031831` with text `#ede8dc`, surface `#1c2734`, and accents `#53678a` / `#b8872a`.

The form's brand colors, in the order given, and the role each was assigned (assignment is by documented rules — ground-suitability by luminance, accents by chroma, text by contrast):

- `#031831` — page background (--color-bg)
- `#ede8dc` — body text (--color-text)
- `#1a2b4a` — primary accent (--color-accent) (stored as `#53678a`: lightness adjusted until it reads at 3:1 on the page background; hue and saturation kept)
- `#b8872a` — secondary accent (--color-accent-2)
- `#596376` — kept as an extra brand color (--color-brand-1)
- `#d5bc90` — kept as an extra brand color (--color-brand-2)
- `#836736` — kept as an extra brand color (--color-brand-3)
- `#9c9fa3` — kept as an extra brand color (--color-brand-4)

## Type

- Headings (--font-heading): Archivo (loaded from Google Fonts by styles.css)
- Body (--font-body): Inter (loaded from Google Fonts by styles.css)

## Assets

- Logo: `assets/logo.png` (preview card: `brand/logo.html`)
- Reference screenshot: `assets/reference/01-Screenshot 2026-07-28 at 9.19.21 AM.png` (preview card: `brand/reference-01.html`)

The reference screenshots are stored for consultation — the generator does not analyze them (it uses no AI), so nothing in the tokens was derived from them. When designing with this system, open them for layout and mood cues.
