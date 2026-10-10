# AGENTS.md — CDN documentation mirror

This repository publishes cdn.emmetts.dev through GitHub Pages (main, root).
Preserve CNAME, .nojekyll, and every legacy font or asset URL.

The Blume source lives in the private RealEmmettS/shaughv-cdn repository,
locally at C:/Users/hey/git/shaughv-cdn. Do not edit generated HTML here.
For every update, review and update all affected canonical Blume docs, examples,
agent URLs, commands, font defaults, catalog metadata, and discovery contracts.
Regenerate tree.json, the header table, README URL table, and the complete Blume
build there; run its docs checks, strict link validation, and tests before pushing.

Publish the validated dist with scripts/publish_pages.py from the canonical
repository. The .blume-published.json ownership manifest identifies generated
files; preserve unrelated assets when updating. Do not copy private source,
credentials, internal maintenance files, or licensed font binaries here.

Commit and push the mirror, verify GitHub Pages finished successfully, then
check its homepage, nested pages, search, Markdown exports, and discovery URLs.
Verify the matching Vercel publication on cdn.shaughv.com as part of the same
change. No scheduled documentation task is used.
