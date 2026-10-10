---
title: Recipes
description: Copy-paste setups for the pages SHAUGHV projects actually ship.
sidebar:
  icon: book-open
  order: 6
---

These are complete, boring recipes. Swap colors and sizes; keep the URLs.

## A marketing page

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>SHAUGHV project</title>
    <link rel="stylesheet" href="https://cdn.shaughv.com/fonts/fonts.css" />
    <link rel="icon" href="https://cdn.shaughv.com/brand/shaughv/favicons/SHAUGHV-Favicon-Dark.svg" media="(prefers-color-scheme: light)">
    <link rel="icon" href="https://cdn.shaughv.com/brand/shaughv/favicons/SHAUGHV-Favicon-Light.svg" media="(prefers-color-scheme: dark)">
    <style>
      :root {
        --font-makira: "Makira", system-ui, sans-serif;
        --font-paper: "Paper Mono", ui-monospace, monospace;
        --bg: #f5f5f0;
        --fg: #5c5446;
        --accent: #5b8a5b;
      }
      body {
        margin: 0;
        background: var(--bg);
        color: var(--fg);
        font-family: var(--font-makira);
      }
      h1 {
        font-family: var(--font-paper);
        text-transform: uppercase;
        letter-spacing: -0.04em;
        line-height: 0.92;
      }
    </style>
  </head>
  <body>
    <shaughv-mark style="display:block;width:72px;height:72px;color:var(--accent)" aria-label="SHAUGHV"></shaughv-mark>
    <h1>One address.<br>Every asset.</h1>
    <script src="https://cdn.shaughv.com/js/animated-brand-mark.js"></script>
  </body>
</html>
```

## A docs or app shell

Makira for chrome and body, Paper Mono for code with the recommended zero.

```css
:root {
  --font-ui: "Makira", system-ui, sans-serif;
  --font-code: "Paper Mono", ui-monospace, monospace;
}
html { font-family: var(--font-ui); }
code, kbd, pre, samp {
  font-family: var(--font-code);
  font-feature-settings: "zero" 1;
}
```

## A loading state

Keep the loader recipe intact. Change only color and box size.

```html
<div style="display:grid;place-items:center;min-height:40vh;background:#f5f5f0;color:#5b8a5b;">
  <shaughv-loader style="height:120px"></shaughv-loader>
</div>
<script src="https://cdn.shaughv.com/js/shaughv-loader.js"></script>
```

## An article with a figurine

```html
<img
  src="https://cdn.shaughv.com/brand/shaughv/figurines/transparent/figurine-header.webp"
  alt="SHAUGHV figurine"
  style="width:min(100%,22rem)"
/>
```

## Agent consumption

Do not scrape these docs for a file list. Fetch the catalog:

```js
const tree = await fetch("https://cdn.shaughv.com/tree.json").then((r) => r.json());
if (!tree.fonts?.all?.defaults) throw new Error("Missing font defaults");
const monoKey = tree.fonts.all.defaults.monospace;
const css = tree.fonts[monoKey].css_url;
```

The `/agents` skill teaches the same workflow without enumerating paths.
