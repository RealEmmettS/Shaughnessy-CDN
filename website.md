---
title: Website layout
description: How the public CDN pages are built, how the catalog reflows, and how to preview every width.
sidebar:
  icon: layout
  order: 8
---

Blume 2.2.2 powers the documentation homepage on both CDN domains, with local search, navigation, Markdown exports, and agent discovery. The original visual guides remain available separately as two HTML pages plus shared CSS and JS:

- site/
  - index.html — CDN overview
  - fonts.html — complete typography guide
  - site.css — layout, type, breakpoints
  - site.js — nav, copy buttons, motion, reveals

Both pages share the header, cream field, sage accents, and Paper Mono display titles. Catalog labels on the homepage use Makira so four columns stay one family instead of four competing mono letterforms.

## Header

Links: Fonts, Assets, Downloads, **Docs**, and the Start coding action. Below 960px the bar collapses to a 44px hamburger with keyboard dismiss, outside click, and Escape.

<a href="https://cdn.shaughv.com/site/index.html">Open the visual overview</a> to confirm the Docs item lands on these pages.

## Homepage catalog

The "Four ways in." section is a four-column grid on wide screens and two columns below 1280px. Each card is a container: the title scales from the card width (`cqi`) so TYPE, IDENTITY, MOTION, and PACKAGES stay inside the rules at every width.

| Width | Catalog |
| --- | --- |
| ≥ 1280px | Four columns |
| 481px–1279px | Two columns |
| ≤ 480px | One column |

Cell borders are right + bottom on every card, so changing the column count never leaves a missing or doubled rule.

## Other reflow points

| Width | What changes |
| --- | --- |
| 1080px | Hero stacks, section headings stack, font-brief stacks |
| 960px | Header becomes a menu |
| 760px | Asset grids, specimens, downloads, and footer stack |
| 480px | Hero actions stretch, receipt chrome stacks, catalog is one column |

Display titles use `overflow-wrap` and `text-wrap: balance` so long Paper Mono words wrap inside the measure instead of painting through the next column.

## Preview locally

```bash
python3 scripts/serve-site.py
```

Check the visual overview and font guide at 1440, 1280, 1024, 768, and 390. The catalog, hero receipt, and font specimens are the places overflow used to show up first.

:::note
Screenshots from those widths belong next to this page when a pass is captured during review. The live pages remain the source of truth.
:::

## Shared asset cache markers

`site/index.html` and `site/fonts.html` load `site.css` and `site.js` with the first 12 characters of each file's SHA-256 as `?v=`. Tests fail if a marker drifts after an edit.
