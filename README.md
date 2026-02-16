# Manifest Design System

A comprehensive design system documentation page for Manifest Finance. This single-page reference documents all design tokens, typography rules, color palettes, component patterns, and interaction guidelines used across Manifest products.

## Getting Started

### Opening the Page

The simplest way to view the design system:

```bash
# Just open in your browser
open index.html

# Or serve locally (recommended for font loading)
npx serve .
```

### Adding Licensed Fonts

This project uses three custom typefaces that require licensing. The `fonts/` directory starts empty — you need to place the licensed `.woff2` files there.

**Required font files:**

| File | Family | Weight |
|------|--------|--------|
| `SeasonSerif-Regular.woff2` | Season Serif | 400 (Regular) |
| `SeasonSerif-Medium.woff2` | Season Serif | 500 (Medium) |
| `SeasonSerif-Semibold.woff2` | Season Serif | 600 (Semibold) |
| `SeasonSerif-Bold.woff2` | Season Serif | 700 (Bold) |
| `SeasonSans-Regular.woff2` | Season Sans | 400 (Regular) |
| `SeasonSans-Medium.woff2` | Season Sans | 500 (Medium) |
| `SeasonSans-Semibold.woff2` | Season Sans | 600 (Semibold) |
| `SeasonSans-Bold.woff2` | Season Sans | 700 (Bold) |
| `GTAmericaMono-Regular.woff2` | GT America Mono | 400 (Regular) |

Place all files in the `fonts/` directory. The page will automatically detect them and hide the fallback font banner.

See `fonts/README.md` for more details.

### Fallback Fonts

When licensed fonts are not installed, the page uses these Google Fonts fallbacks (loaded via CDN):

- **Season Serif** → Playfair Display → Georgia → serif
- **Season Sans** → DM Sans → system sans-serif
- **GT America Mono** → JetBrains Mono → SF Mono → monospace

## Source Figma Files

- [App Design System (WebApp)](https://www.figma.com/design/9eWdoJt2D3gt7nz04BlU9b/Design-System---WebApp?node-id=2406-102217) — Primary source for color tokens, components, UI patterns
- [Brand Foundation (Social)](https://www.figma.com/design/ClpUCdebqhgtta0HZx9e2b/Brand-Foundation---Social?node-id=0-1) — Brand colors, logo usage, typographic hierarchy

## Project Structure

```
design-system/
├── index.html              ← The design system page (single file, embedded CSS/JS)
├── fonts/                  ← Directory for licensed font files (starts empty)
│   └── README.md           ← Instructions on which font files to place here
├── assets/                 ← Logos and brand marks
│   ├── logo-color.svg      ← Full color logo
│   ├── logo-black.svg      ← Black version
│   ├── icon-color.svg      ← Icon mark only
│   └── icon-color-flat.svg ← Flat icon variant
└── README.md               ← This file
```
