# AGENTS.md — retired CDN host

The live CDN and documentation are maintained in the private `RealEmmettS/shaughv-cdn` repository at `C:/Users/hey/git/shaughv-cdn` and deployed to Vercel. Both public CDN hostnames alias that deployment.

This checkout is only a static forwarding bridge for cached DNS pointing to GitHub Pages. Preserve `CNAME`, `.nojekyll`, `index.html`, and `404.html` while the bridge is retained. The redirect destination is the fixed primary hostname `https://cdn.shaughv.com`; preserve the incoming path, query, and fragment without permitting another origin.

Do not regenerate the former documentation mirror or restore the 369 deleted legacy assets unless the owner explicitly requests recovery. Git history contains the former files. Never copy private source, credentials, internal maintenance files, or licensed font binaries into this public repository.

For CDN changes, follow the canonical repository's instructions, update affected Blume docs and agent contracts, validate and deploy there, then verify both Vercel hostnames. No scheduled documentation task is required.
