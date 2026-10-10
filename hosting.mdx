---
title: Hosting and updates
description: Where the two CDN domains run, how the documentation stays current, and how to validate a change.
sidebar:
  icon: server
  order: 9
---

## Two domains, one documentation source

| Host | Role | Hosting |
| --- | --- | --- |
| `cdn.shaughv.com` | Current asset catalog and documentation | Vercel static deployment |
| `cdn.emmetts.dev` | Documentation mirror and preserved legacy assets | GitHub Pages |

Both homepages publish the same Blume build. Current font, brand, motion, and
download examples use `cdn.shaughv.com`. The older domain keeps its existing
asset paths, but it is not a second copy of the current catalog.

The primary CDN uses Vercel DNS and managed HTTPS. The documentation mirror
keeps its existing DNS and GitHub Pages custom domain. No runtime function,
database, or Blob store is required. The original R2 bucket is a historical
snapshot, not the current origin or a synchronized backup.

## Free hosting boundaries

The primary site uses Vercel Hobby. Its transfer and request allowances are
shared with other projects on the account; they are not unlimited. Check
[Vercel's current plan documentation](https://vercel.com/docs/plans/hobby)
before changing the audience or increasing traffic. GitHub Pages applies its
own service limits to the mirror. No paid subscription was added for this setup.

## Documentation follows repository changes

The private `RealEmmettS/shaughv-cdn` repository is the canonical source for
assets, the catalog, and the Markdown/MDX pages. Blume is pinned in the lockfile.
Its build produces navigation, local search, page HTML, Markdown exports,
agent discovery, social images, and the sitemap together.

Every change must update affected documentation before it is pushed. The
repository's agent instructions require checking URLs, font defaults,
examples, and workflows, followed by the docs build and strict link validation.
GitHub CI checks the same build. There is no scheduled AI maintenance job.

```bash
npm ci
npm run docs:check
bash scripts/deploy.sh --dry-run
npx blume validate --strict
bash scripts/test.sh
```

On Windows, run the shell commands through Git Bash. The public preview uses
`python3 scripts/serve-site.py` after the build and binds to localhost.

## Publishing both hosts

Deploy the complete public package to a Vercel preview and verify it before
publishing production. Then use the repository's Pages publisher to copy the
same compiled documentation into the existing `RealEmmettS/Shaughnessy-CDN`
checkout. Push its `main` branch to trigger GitHub Pages.

The publisher preserves legacy assets and `CNAME`, tracks the generated files
it owns, and removes obsolete generated files on subsequent updates. Fonts
are loaded from their canonical CDN URLs rather than copied into the public
mirror. Private source and maintenance files are excluded from both outputs.

## Verification and recovery

Check rendered pages, search, navigation, mobile layout, and actual font loading.
The primary CDN's live verifier also checks exact file bytes, response types,
cache policy, CORS, downloads, byte ranges, missing files, and cache hits.
HTTP success alone does not prove that a font rendered or a search result works.

For a broken Vercel release, roll back to a previously verified deployment.
For a broken Pages update, revert the publishing commit and wait for the Pages
build to finish. Preserve immutable asset URLs: changed binary files need new
filenames because a deployment cannot clear a visitor's browser cache.
