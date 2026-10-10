---
title: SHAUGHV CDN
description: One address for fonts, brand assets, motion drop-ins, and packages across SHAUGHV projects.
sidebar:
  label: Overview
  icon: house
  order: 1
---

Use the CDN to load fonts, brand assets, motion components, and downloads across authorized SHAUGHV projects. Link the original asset instead of copying it into each app.

These searchable docs are published at both **cdn.shaughv.com** and **cdn.emmetts.dev**. Use **cdn.shaughv.com** for current asset URLs; the older domain preserves its existing files. Public access does not grant redistribution rights.

<a href="https://cdn.shaughv.com/site/index.html">Open the visual website</a>
·
<a href="https://cdn.shaughv.com/site/fonts.html">Open the font guide</a>

**[Quickstart](/quickstart)**

Paste one URL and start using fonts, marks, or packages.

**[Fonts](/fonts)**

Makira + Paper Mono are standard. Gail Rock stays compatible; two other families are opt-in.

**[Brand](/brand)**

Wordmarks, favicons, and transparent figurines with live previews.

**[Motion](/motion)**

Browser-ready animated mark and loader drop-ins.

## What lives here

| Path | What you get |
| --- | --- |
| `/fonts/` | Family stylesheets plus web and desktop font files |
| `/brand/` | Official wordmarks, favicons, and figurines |
| `/js/` | Animated brand mark and loader custom elements |
| `/site/` | The visual CDN website and font guide |
| `/` | This documentation; `/docs` redirects here |

:::tip
If you do not know the filename, fetch [`/tree.json`](https://cdn.shaughv.com/tree.json) instead of guessing. It lists every hosted file with a paste-ready URL.
:::

## How delivery works

```mermaid
flowchart LR
  A[Your site] -->|HTTPS GET| B[cdn.shaughv.com]
  B --> C[Vercel edge cache]
  C -->|miss| D[Static deployment]
  D --> C
  C --> A
```

There is no application server in front of the files. Each object keeps the `Content-Type` and `Cache-Control` set by the static deployment. Binaries are immutable for a year. CSS and JavaScript use a one-day cache with a seven-day stale-while-revalidate window.

## Visual identity

The website and these docs share the same cream, olive, and sage system.

- **Cream 200**: `#F5F5F0`

- **Sage**: `#5B8A5B`

- **Olive**: `#5C5446`

- **Bamboo**: `#C4A876`

- **Action**: `#4A7A4A`

Use the SVG from /brand/shaughv/logos/.

![SHAUGHV wordmark](/blume-assets/content/docs/images/wordmark.svg)

Official SHAUGHV wordmark

## Standard type pair

Makira and Paper Mono can both carry titles, interfaces, body copy, and buttons. Paper Mono is also the preferred monospace for code and data.

<div class="cdn-specimen">
  <span class="cdn-specimen-label">Makira / sans</span>
  <p class="cdn-makira cdn-display">One face. Any surface.</p>
  <p class="cdn-makira cdn-body">Clear at reading sizes, forceful at display sizes, and comfortable on controls.</p>
</div>

<div class="cdn-specimen">
  <span class="cdn-specimen-label">Paper Mono / mono</span>
  <p class="cdn-paper cdn-display">Same range. Fixed pitch.</p>
  <p class="cdn-paper cdn-body">Expressive at display sizes, readable in body copy, and naturally precise for code.</p>
</div>

Load both families with one stylesheet:

```html
<link rel="stylesheet" href="https://cdn.shaughv.com/fonts/fonts.css" />
```

## Next

**[Start coding](/quickstart)**

Copy the first working snippets.

**[Recipes](/recipes)**

Common page setups for fonts, icons, and motion.

**[Website layout](/website)**

How the public CDN pages are structured and how they reflow.

**[Reference](/reference)**

Namespaces, cache tiers, and discovery files.
