---
title: Brand assets
description: Official wordmarks, responsive favicons, and transparent figurines ready to place.
sidebar:
  icon: image
  order: 3
---

Identity files live under `/brand/shaughv/`. Link them. Do not redraw the mark or recrop a figurine unless you are producing a new named asset.

## Wordmark

The static fallback when the animated mark is not loaded.

![Official SHAUGHV wordmark](/blume-assets/content/docs/images/wordmark.svg)

SHAUGHV-Official.svg

```html
<img
  src="https://cdn.shaughv.com/brand/shaughv/logos/SHAUGHV-Official.svg"
  alt="SHAUGHV"
/>
```

On dark surfaces, invert the SVG with CSS rather than shipping a second file:

```css
.wordmark-on-olive {
  filter: brightness(0) invert(1);
}
```

## Favicons

The pair follows the visitor's color scheme: dark mark on light browser chrome, light mark on dark chrome.

<div class="cdn-swatch-row">
  <div class="cdn-swatch" style="background:#fafaf8;color:#5c5446;">
    ![Dark SHAUGHV favicon](/blume-assets/content/docs/images/favicon-dark.svg)
    <strong>Dark favicon</strong>
    <small>Light scheme</small>
  </div>
  <div class="cdn-swatch" style="background:#5c5446;color:#f5f5f0;">
    ![Light SHAUGHV favicon](/blume-assets/content/docs/images/favicon-light.svg)
    <strong>Light favicon</strong>
    <small>Dark scheme</small>
  </div>
</div>

```html
<link rel="icon" href="https://cdn.shaughv.com/brand/shaughv/favicons/SHAUGHV-Favicon-Dark.svg" media="(prefers-color-scheme: light)">
<link rel="icon" href="https://cdn.shaughv.com/brand/shaughv/favicons/SHAUGHV-Favicon-Light.svg" media="(prefers-color-scheme: dark)">
```

Alternate marks also exist:

- `SHAUGHV-Favicon-Dark-Alt.svg`
- `SHAUGHV-Favicon-Light-Alt.svg`

## Figurines

Transparent WebP files sit on cream, color, or photography without a baked-in background.

Transparent set under /brand/shaughv/figurines/transparent/.

![Figurine of Shaughv pointing at his vintage Mac.](/blume-assets/content/docs/images/figurine-look-at-this.webp)

figurine-look-at-this.webp

![SHAUGHV figurine header pose.](/blume-assets/content/docs/images/figurine-header.webp)

figurine-header.webp

![SHAUGHV figurine with mail.](/blume-assets/content/docs/images/figurine-mail.webp)

figurine-mail.webp

```html
<img
  src="https://cdn.shaughv.com/brand/shaughv/figurines/transparent/figurine-look-at-this.webp"
  alt="Figurine of Shaughv pointing at his vintage Mac."
/>
```

Non-transparent counterparts live one directory up, for cases that already provide a solid stage.

- brand/shaughv/
  - logos/SHAUGHV-Official.svg
  - favicons/
    - SHAUGHV-Favicon-Dark.svg
    - SHAUGHV-Favicon-Light.svg
    - SHAUGHV-Favicon-Dark-Alt.svg
    - SHAUGHV-Favicon-Light-Alt.svg
  - figurines/
    - figurine-header.webp
    - figurine-look-at-this.webp
    - transparent/
      - figurine-header.webp
      - figurine-look-at-this.webp
