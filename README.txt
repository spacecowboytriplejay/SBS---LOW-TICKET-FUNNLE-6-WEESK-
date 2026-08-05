STEP 2 — selfbuiltsystems.io (the "Open roles" site)
=====================================================

The .io serves different content ("Open roles" page), so it deploys from a
DIFFERENT project than sbs-3-door-funnel. Same fix, applied there:

1. Put all 7 files from "public/" into the .io project's public/static root
   (whatever folder ends up served at the domain root, so that
   https://www.selfbuiltsystems.io/favicon.ico resolves).
2. Paste the contents of head-snippet.html into the <head> of the .io
   site's index.html. All favicon links are RELATIVE, so they work as-is.
   The og:image lines use absolute .io URLs, as scrapers require absolute.
   If the .io page already has og:image tags, replace them instead of duplicating.
3. Deploy, then verify https://www.selfbuiltsystems.io/favicon.ico loads,
   and request re-indexing of the .io homepage in Search Console.

If you point me at the .io repo, I will produce an exact repo-mirrored
folder like Step 1 instead of this generic pack.
