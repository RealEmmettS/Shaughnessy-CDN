# Retired CDN host

The current CDN is hosted on Vercel at both [cdn.shaughv.com](https://cdn.shaughv.com/) and [cdn.emmetts.dev](https://cdn.emmetts.dev/). Both names serve the same current assets and Blume documentation.

This repository retains only a forwarding page for clients whose DNS cache still points to GitHub Pages. It forwards to the primary Vercel hostname, preserving the path, query, and fragment. It is not an asset origin or a documentation mirror.

The owner requested deletion of the 369 obsolete files: seven legacy font collections and their specimens, old website assets, and two duplicate font ZIPs. They have been removed from the current branch; Git history retains recovery copies. The previous generated documentation snapshot was also removed as part of retiring the mirror.

The canonical source is the private `RealEmmettS/shaughv-cdn` repository. Make and deploy changes there. Do not publish private source or licensed font binaries here, run the old Pages publisher, or restore the removed assets during ordinary maintenance.

The `CNAME` and `.nojekyll` files remain solely for the forwarding bridge. No subscription or scheduled job was added.
