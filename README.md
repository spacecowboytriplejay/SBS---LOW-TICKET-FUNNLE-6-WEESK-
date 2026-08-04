# SelfBuiltSystems.io — Content Factory Protocol (v1)

International 6-week protocol funnel. Static site: `index.html` + `avatars/`.

## Deploy (first time)
```bash
cd deploy
git init && git add -A && git commit -m "v1: content factory protocol funnel"
gh repo create selfbuiltsystems-io --private --source=. --push   # or push to an existing repo
```
Then in Vercel: **Add New Project → Import the repo → Deploy** (no build step, framework = Other).
Finally: Vercel → Project → Settings → Domains → add `selfbuiltsystems.io`.

Fast path without GitHub: `npx vercel deploy --prod` from this folder.

## Before ads run — wire these in index.html (CONFIG block, bottom <script>)
- [ ] `WAITLIST_URL`  — Atlas / GHL waitlist form
- [ ] `CHECKOUT_URL`  — GHL checkout, pay in full ($297)
- [ ] `SPLIT_URL`     — GHL checkout, 2-pay (2×$167)
- [ ] `VSL_EMBED`     — hero VSL embed URL (page works without it)
- [ ] `PAGE_MODE`     — "waitlist" now → flip to "cart" when doors open
- [ ] Dates: `CART_OPEN`, `DOORS_CLOSE`, `COHORT_START`

## Proof still pending (drop in when received)
- Buntu Majaja photo (avatars/) + IG handle · Dean White photo · Edgars story/handle · Jandre IG handle
- Real journey screenshots → the 4 dashed slots in "receipts from the journey"
