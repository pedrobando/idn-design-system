# Innovative Dynamic Networks — Design System

A complete brand reference and print-ready brand book for **Innovative Dynamic Networks (IDN)** — a veteran-owned managed IT provider serving the Milwaukee and Chicago area for 20+ years.

> **We Manage Your IT, So You Can Manage Your Business**

Extracted from [idn-wi.com](https://idn-wi.com/) — colors, fonts, principles, and logo all come from the live brand, nothing invented.

## Deliverables

| File | What it is |
|------|------------|
| [`design/design-system.html`](design/design-system.html) | Scrollable reference page — color hierarchy, typography, principles, components, icons, wordmarks |
| [`design/brand-book-a4.html`](design/brand-book-a4.html) | Single A4 portrait page (the brand topline at a glance) |
| [`design/brand-book-a4.pdf`](design/brand-book-a4.pdf) | The rendered, print-ready brand book |
| [`design/idn-logo.png`](design/idn-logo.png) | The official IDN logo (embedded as-is, never redrawn) |

Both HTML files are self-contained — Google Fonts CDN + inline CSS + inline SVG, no build step.

## Brand at a glance

### Color

| Role | Name | Hex | Usage |
|------|------|-----|-------|
| Primary | IDN Blue | `#377FBF` | Links, buttons, the logo mark, key highlights |
| Secondary | Deep Blue | `#26629C` | Hover states, gradients, dimensional depth |
| Tertiary | Slate Navy | `#223645` | Headings, body text, dark surfaces |
| Neutral | Ink | `#152938` | Deepest surfaces |
| Neutral | Mist | `#B5C5D0` | Reversed text on navy, subtle accents |
| Neutral | Gray | `#7A7A7A` | Secondary text |
| Neutral | Cloud | `#F6F6F6` | Light backgrounds |

### Typography

- **Cabin** — display & body (humanist sans, calm and professional)
- **Roboto Slab** — overlines, labels, and numeric callouts

Both load free via Google Fonts.

### Principles

1. **Reliability** — proactive IT that prevents problems before they disrupt the business
2. **Problem Solving** — 35+ years of combined experience behind every fix
3. **One-Stop Shop** — comprehensive IT under one roof, one accountable team
4. **Proven Quality** — 20+ years serving 1000+ businesses
5. **Technical Expertise** — certified professionals across the full stack
6. **Competitive Pricing** — scalable solutions sized to fit the business

## Viewing

Open either HTML file in any browser:

```bash
open design/design-system.html
open design/brand-book-a4.pdf
```

## Re-rendering the PDF

If you edit `brand-book-a4.html`, re-render with a headless browser.

**macOS (Chrome):**

```bash
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" \
  --headless --disable-gpu --no-pdf-header-footer \
  --print-to-pdf="design/brand-book-a4.pdf" \
  "file://$PWD/design/brand-book-a4.html"
```

**Windows (Edge):**

```bash
"/c/Program Files (x86)/Microsoft/Edge/Application/msedge.exe" \
  --headless --disable-gpu --no-pdf-header-footer \
  --print-to-pdf="brand-book-a4.pdf" \
  "file:///absolute/path/to/design/brand-book-a4.html"
```

## How it was built

Generated with the [design-system toolkit](https://github.com/robonuggets/design-system) skill for Claude Code, which extracts a brand from any reference (URL, screenshot, or description) and produces both artifacts. The skill definition lives under `.claude/skills/design-system/` in this repo.

## License

MIT
