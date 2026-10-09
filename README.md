# APEX ACCESS — The Accessibility Grand Prix

An interactive, single-page accessibility lab built with plain HTML, CSS and JavaScript. It teaches and tests WCAG 2.1 concepts through hands-on exercises, wrapped in a racing-themed interface.

No build step, no dependencies, no external requests — just open `index.html` in a browser.

## Features

The lab is organised into four tabs:

1. **Keyboard and ARIA** — practise keyboard navigation and screen reader patterns (tabs, accordion, menu, dialog, live-region toasts, forms with error handling).
2. **Contrast and zoom** — test colour contrast, text spacing, magnification and colour-vision-deficiency simulations (protanopia, deuteranopia, tritanopia, achromatopsia).
3. **Fix the UI** — a WCAG 2.1 remediation workshop with a side-by-side *Before (broken)* and *After (fixed)* sample interface.
4. **Audit report** — a checklist and printable audit report.

### Themes

Switch themes from the theme selector. Every theme is built from CSS design tokens and designed to keep text at 4.5:1+ contrast and UI borders at 3:1+.

- Ocean Blue, Blossom Pink, Lavender, Mint Green, Sunset
- McLaren, Mercedes, Ferrari, Porsche
- Midnight (dark) and High contrast

## Accessibility highlights

- Page language declared (`lang="en"`) and a skip link
- Visible focus indicators on all interactive elements
- Roving-tabindex tabs with proper ARIA roles
- Minimum 44px touch targets
- `prefers-reduced-motion` respected
- Print stylesheet for the audit report
- Safe-area insets for notched mobile devices

## Getting started

```bash
git clone <your-repository-url>
cd apex-access
```

Then open `index.html` in any modern browser, or serve it locally:

```bash
python3 -m http.server 8000
# visit http://localhost:8000
```

## Project structure

```
.
├── index.html   # The entire app (markup, styles and scripts)
└── README.md
```

## Deploying

Because it is a static page, it works on GitHub Pages, Netlify, Vercel or any static host. For GitHub Pages: **Settings → Pages → Deploy from branch → `main` / root**.
