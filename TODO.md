# TODO

## Step 1 — Verify cloud-sync wiring

- [x] Read `sync.js`, `index.html`, `topbar.js`.
- [ ] Verify whether other pages (`health.html`, `po-water.html`, `finance.html`) contain `initCloudSync(...)` blocks.

## Step 2 — Fix cloud-sync placeholders (required)

- [ ] Replace placeholder `SUPABASE_URL` and `SUPABASE_KEY` in `sync.js` with real values (or disable sync cleanly if secrets not available).

## Step 3 — Ensure each page uses the correct appKey + prefixes

- [ ] Confirm `index.html` uses `appKey: "goals"` + prefix `goals:`.
- [ ] Decide the correct appKey/prefix mapping for:
  - health / water (`po_water_v1`)
  - stack (`stack:*`)
  - finance/net worth/orders/subs/wishlist

## Step 4 — Validate by running in browser

- [ ] Open each page and ensure no JS errors.
- [ ] Confirm two-tab sync works (edit in one tab, see update in the other).
