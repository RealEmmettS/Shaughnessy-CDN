---
title: Reference
description: Namespaces, cache tiers, CORS, and discovery files for cdn.shaughv.com.
sidebar:
  icon: list
  order: 7
---

Short facts the website implies and `/tree.json` makes explicit.

## Origin

`https://cdn.shaughv.com`

Always HTTPS. Do not use the `public.r2.dev` development hostname in production code.

## Namespaces

| Prefix | Contents |
| --- | --- |
| `/brand/` | Wordmarks, favicons, figurines |
| `/fonts/` | Family CSS plus webfonts and desktop files |
| `/js/` | Custom elements and the React mark port |
| `/site/` | Visual website HTML, CSS, and JS |
| `/` | Blume documentation; `/docs` redirects here |
| `/tree.json` | Generated catalog |
| `/agents` | Markdown skill download |
| `/prompts` | Research archive redirect |
| `/prompts-skill` | Nested skill ZIP |

## Cache

| Kind | Policy |
| --- | --- |
| Catalog fonts, images, media | `public, max-age=31536000, immutable` |
| CSS, JS, HTML, JSON, generated documentation | `public, max-age=86400, stale-while-revalidate=604800` |

Replace a mutable CSS/JS file in place. Ship a new filename for any binary that changed.

## CORS

On `cdn.shaughv.com`, `GET`, `HEAD`, and `OPTIONS` use `Access-Control-Allow-Origin: *`. Preflight returns 204. Byte ranges return 206, and CORS exposes content length, content range, ETag, and cache metadata. Missing assets return 404 rather than an HTML success response.

These custom headers describe the primary Vercel CDN. The documentation mirror at `cdn.emmetts.dev` uses GitHub Pages caching and response headers.

## Discovery

| URL | Role |
| --- | --- |
| `/tree` and `/tree.json` | Machine-readable inventory |
| `/agents` | Skill that teaches agents to read the inventory |
| `/llms.txt` and `/llms-full.txt` | Compact index and complete Markdown documentation |
| `/index.md`, `/fonts/paper-mono.md` | Markdown page exports |
| `/.well-known/api-catalog` | API discovery linkset |
| `/.well-known/ai-catalog.json` | Agent discovery catalog |
| `/openapi.json` | Generated documentation API description |
| `/agent-readability.json` | Generated machine-readability information |

## Human pages

| Address | File |
| --- | --- |
| `/` | Blume documentation homepage |
| `/fonts` | Font documentation overview |
| `/fonts/paper-mono` | Paper Mono installation and format reference |
| `/site/index.html` | Original visual overview on the primary CDN |
| `/site/fonts.html` | Interactive visual font guide on the primary CDN |
| `/docs` | Permanent redirect to `/` on the primary CDN |

Deeper paths such as `/fonts/fonts.css` are real objects and must not be rewritten.
