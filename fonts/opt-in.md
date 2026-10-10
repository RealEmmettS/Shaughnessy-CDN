---
title: Opt-in families
description: IBM Plex Mono and Unbounded stay off the standard bundle until a project asks for them.
sidebar:
  icon: sparkles
  order: 4
---

The standard stylesheet stays focused on Makira and Paper Mono. These two families are fully hosted, but each has its own CSS file.

## IBM Plex Mono

A quieter optional mono for technical labels, code, and dense metadata. Normal and italic, 100–700.

```html
<link rel="stylesheet" href="https://cdn.shaughv.com/fonts/ibm-plex-mono/ibm-plex-mono.css" />
```

```css
.meta {
  font-family: "IBM Plex Mono", ui-monospace, monospace;
  font-weight: 500;
}
```

<div class="cdn-specimen">
  <span class="cdn-specimen-label">IBM Plex Mono / 700</span>
  <p class="cdn-plex cdn-display">IBM Plex Mono</p>
  <p class="cdn-plex cdn-body">status: ready · GET /tree.json</p>
</div>

:::note
Paper Mono remains the standard code face. Reach for IBM Plex Mono when a surface wants a less expressive mono, especially if italic is required.
:::

## Unbounded

Wide geometric display cuts, plus a variable family across 100–900. Also includes the Blond cut.

```html
<link rel="stylesheet" href="https://cdn.shaughv.com/fonts/unbounded/unbounded.css" />
```

```css
.display {
  font-family: "Unbounded", "Makira", sans-serif;
  font-weight: 700;
  letter-spacing: -0.06em;
  text-transform: uppercase;
}
```

<div class="cdn-specimen">
  <span class="cdn-specimen-label">Unbounded / 700</span>
  <p class="cdn-unbounded cdn-display">Unbounded</p>
</div>

:::warning
Unbounded's embedded copyright identifies Parity Technologies. Do not describe it as SIL Open Font License unless a later license file says so.
:::

## When to opt in

| Need | Choice |
| --- | --- |
| Default SHAUGHV interface | Makira and/or Paper Mono |
| Code with a slashed zero on a brand grid | Paper Mono + `zero` |
| Italic mono, quieter texture | IBM Plex Mono |
| Extra-wide geometric display | Unbounded |
