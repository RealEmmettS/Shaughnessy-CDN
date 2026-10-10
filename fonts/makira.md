---
title: Makira
description: The standard SHAUGHV sans — one face for titles, interfaces, body copy, and controls.
sidebar:
  icon: type
  order: 2
---

Makira is the versatile sans in the standard pair. It is not reserved for headlines. Use it anywhere the surface should feel owned without a fixed-pitch grid.

<div class="cdn-specimen">
  <span class="cdn-specimen-label">Display / 700</span>
  <p class="cdn-makira cdn-display">One address. Every asset.</p>
</div>

<div class="cdn-specimen">
  <span class="cdn-specimen-label">Body / 400</span>
  <p class="cdn-makira cdn-body">Fonts, marks, favicons, figurines, and browser-ready motion for SHAUGHV projects. Link the exact thing you need. Use it anywhere.</p>
</div>

<div class="cdn-specimen">
  <span class="cdn-specimen-label">UI label / 700</span>
  <p class="cdn-makira" style="margin:0;font-size:0.72rem;letter-spacing:0.14em;text-transform:uppercase;font-weight:700;">Asset delivery / CDN</p>
</div>

## Load it

The standard bundle already includes Makira. A project that only wants this family can still link the dedicated file:

```html
<link rel="stylesheet" href="https://cdn.shaughv.com/fonts/makira/makira.css" />
```

## CSS families

| Name | Use |
| --- | --- |
| `"Makira"` | Static cuts, 400–900 |
| `"Makira VF"` | Variable 400–900 |

```css
.hero-title {
  font-family: "Makira", system-ui, sans-serif;
  font-weight: 800;
  letter-spacing: -0.04em;
  text-transform: uppercase;
}
```

## Files on the CDN

- fonts/makira/
  - makira.css
  - woff2/ — browser-first webfonts
  - woff/
  - ttf/
  - otf/
  - variable/ — `"Makira VF"`

Static filenames follow `Makira-Regular.woff2`, `Makira-Medium.woff2`, `Makira-SemiBold.woff2`, `Makira-Bold.woff2`, `Makira-ExtraBold.woff2`, and `Makira-Black.woff2`.

:::tip
If a cut ever needs a hint regen or a glyph addition, ship a new filename. Binary objects are cached as immutable. Never overwrite `Makira-Bold.woff2` in place.
:::

## License

Makira is commercially licensed for authorized SHAUGHV use. Public font URLs do not grant permission to redistribute its binaries. Use the hosted CSS rather than committing it to public repositories.
