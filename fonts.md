---
title: Fonts
description: Makira and Paper Mono are the standard pair. IBM Plex Mono and Unbounded stay opt-in.
sidebar:
  label: Overview
  order: 1
---

The SHAUGHV type system is two versatile families, not a headline font plus a body font. Use either one for titles, display, interfaces, body copy, or buttons. Paper Mono also gives code and data a precise grid.

**[Makira](/fonts/makira)**

Standard sans. Weights 400–900, static and variable.

**[Paper Mono](/fonts/paper-mono)**

Standard mono. Weights 100–800, static and variable.

**[IBM Plex Mono](/fonts/opt-in)**

Optional quieter mono with italics.

**[Unbounded](/fonts/opt-in)**

Optional geometric display family.

## Load the standard pair

```html HTML
<link rel="stylesheet" href="https://cdn.shaughv.com/fonts/fonts.css" />
```

```css CSS
@import url("https://cdn.shaughv.com/fonts/fonts.css");
```

That one file imports Makira and Paper Mono, plus Gail Rock for compatibility with existing sites. The live manifest records the preferred pair in `fonts.all.defaults`. It does **not** import IBM Plex Mono or Unbounded.

## Family names

| Family | Status | CSS family names | Weights |
| --- | --- | --- | --- |
| Makira | Standard | `"Makira"`, `"Makira VF"` | 400–900 |
| Paper Mono | Standard | `"Paper Mono"`, `"Paper Mono Variable"` | 100–800 |
| Gail Rock | Compatibility | `"Gail Rock"`, `"Gail Rock VF"` | 100–700 |
| IBM Plex Mono | Opt-in | `"IBM Plex Mono"` | 100–700, italic |
| Unbounded | Opt-in | `"Unbounded"`, `"Unbounded Blond"`, `"Unbounded Variable"` | 300–900 + variable 100–900 |

## Side by side

The same sentence in both standard voices:

<div class="cdn-specimen">
  <span class="cdn-specimen-label">Makira</span>
  <p class="cdn-makira cdn-display">Ready for the whole interface.</p>
  <p class="cdn-makira cdn-body">Clear at reading sizes, forceful at display sizes, and comfortable on controls.</p>
</div>

<div class="cdn-specimen">
  <span class="cdn-specimen-label">Paper Mono</span>
  <p class="cdn-paper cdn-display">Ready for the whole interface.</p>
  <p class="cdn-paper cdn-body">Expressive at display sizes, readable in body copy, and precise for code and data.</p>
</div>

:::warning
Do not add another family to the standard bundle without an explicit brand decision. Opt-in stylesheets exist so a project can ask for a third voice on purpose.
:::

## Recommended CSS variables

```css
:root {
  --font-makira: "Makira", system-ui, sans-serif;
  --font-paper: "Paper Mono", ui-monospace, monospace;
  --font-mono-alt: "IBM Plex Mono", ui-monospace, monospace;
  --font-brutal: "Unbounded", system-ui, sans-serif;
}
```

The live font guide at <a href="https://cdn.shaughv.com/site/fonts.html">visual font guide</a> shows both families across display, body, interface, and control roles, plus Gail Rock's compatibility specimens.
