

# CDN Overview

The [**Shaughnessy CDN**](https://cdn.emmetts.dev) is a private CDN for use only on [**Shaughnessy**](https://shaughnessy.irish) sponsored websites and web-apps. This CDN _does_ include third-party fonts, images, and files that were _neither created_ _nor_ _commissioned_ by the [**Shaughnessy Group**](https://shaughnessy.irish) or its associates.

The [**Shaughnessy CDN**](https://cdn.emmetts.dev) is designed to make [**Shaughnessy**](https://shaughnessy.irish) web-based projects quicker and more responsive by loading a font through a CDN, rather than directly on the web-server.

_**DO NOT USE THE SHAUGHNESSY CDN WITHOUT EXPLICIT PERMISSION; THIS IS NOT A PUBLIC-USE CDN.**_

## Documentation publishing

The homepage is the Blume documentation built from `RealEmmettS/shaughv-cdn`.
GitHub Pages publishes this repository's `main` branch root at `cdn.emmetts.dev`.
The same documentation runs on `cdn.shaughv.com`; current asset examples use
that primary CDN. Existing files in this repository remain at their original URLs.

Edit documentation in the canonical repository, validate it, run its
`scripts/publish_pages.py` against this checkout, then commit and push.
Keep `.nojekyll`, `CNAME`, and `.blume-published.json`. The last file records only
generated documentation so later updates preserve legacy files.

Every update must keep affected Blume pages, agent URLs and commands, the asset
tree, and generated discovery files synchronized before pushing; see `AGENTS.md`.
