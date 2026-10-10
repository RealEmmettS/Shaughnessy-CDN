---
title: Gail Rock
description: The previous SHAUGHV monospace, retained for compatibility — a full interface voice with a true fixed-pitch grid.
sidebar:
  icon: code
  order: 3
---

Paper Mono is the preferred monospace for new installations. Gail Rock remains in the combined stylesheet for existing designs.

Gail Rock is a true monospace: every encoded glyph shares the same 650-unit advance. It is still a full interface family. Titles, body, buttons, and data can all wear it. The grid is a capability, not a restriction to code blocks.

<div class="cdn-specimen">
  <span class="cdn-specimen-label">Display / 700</span>
  <p class="cdn-gail cdn-display">Make the headline count.</p>
</div>

<div class="cdn-specimen">
  <span class="cdn-specimen-label">Code preset / unmarked O + slashed zero</span>
  <p class="cdn-gail cdn-body" style="font-feature-settings:'zero' 1;">const token = 0x00A0;<br />font-family: "Gail Rock";</p>
</div>

## Load it

Included in `fonts/fonts.css`. Solo import:

```html
<link rel="stylesheet" href="https://cdn.shaughv.com/fonts/gail-rock/gail-rock.css" />
```

## CSS families

| Name | Use |
| --- | --- |
| `"Gail Rock"` | Static 100–700 |
| `"Gail Rock VF"` | Variable 100–700 |

Static files on the CDN: Thin, Extralight, Light, Regular, Medium, Semibold, Bold.

## OpenType voices

The grid never changes. Features switch the drawing of specific glyphs.

| Feature | Effect | Use |
| --- | --- | --- |
| default | Unmarked O/o | Body and the recommended code look |
| `ss01` | Center-marked O/o, single-storey a/g, alternate Q/4 | Signature display |
| `ss02` | Slashed O/o and accented forms | A sharper display voice |
| `zero` | Slashed numeral 0 | Code and data |
| `dlig` | FI, LI, ft, tr ligatures | Short display copy |

:::warning
Choose `ss01` or `ss02` for expressive O forms, not both. `zero` and `dlig` can layer independently.
:::

<div class="cdn-specimen">
  <span class="cdn-specimen-label">Default O o · a g 4 Q</span>
  <p class="cdn-gail cdn-display">O o a g 4 Q</p>
</div>

<div class="cdn-specimen">
  <span class="cdn-specimen-label">ss01 signature</span>
  <p class="cdn-gail cdn-display" style="font-feature-settings:'ss01' 1;">O o a g 4 Q</p>
</div>

<div class="cdn-specimen">
  <span class="cdn-specimen-label">ss02 slash</span>
  <p class="cdn-gail cdn-display" style="font-feature-settings:'ss02' 1;">O o Ó ó</p>
</div>

<div class="cdn-specimen">
  <span class="cdn-specimen-label">zero · capital O beside slashed 0</span>
  <p class="cdn-gail cdn-display" style="font-feature-settings:'zero' 1;">O 0 00A0</p>
</div>

## Best for code

Keep the default, unmarked O/o and enable `zero` so numeral 0 cannot be confused with capital O. The feature name is literal: `zero` changes 0, while `ss01` is the option that puts a center mark in O/o.

```css
.gail-code {
  font-family: "Gail Rock", ui-monospace, monospace;
  font-feature-settings: "zero" 1;
}
.gail-signature { font-feature-settings: "ss01" 1; }
.gail-slashed-o { font-feature-settings: "ss02" 1; }
.gail-ligatures { font-feature-settings: "dlig" 1; }
```

The font guide at <a href="https://cdn.shaughv.com/site/fonts.html">visual font guide</a> includes a live weight-axis specimen and copyable CSS for every switch.
