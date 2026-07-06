# Deploying the ELLIS regional-comparison dashboard (password-protected)

One file: `index.html` — a self-contained, encrypted dashboard. Same password as the
CAISI version.

- **URL (after deploy):** https://ariankhorasani.github.io/ellis-ai-safety/
- **Password:** `AISafety-Jinesis`
- Anyone with the URL + password can view and re-share it. Client-side gate — good for
  a controlled draft, not a guarantee against a determined attacker.

## Deploy (no terminal)
1. Repo **`ellis-ai-safety`** → **Add file → Upload files** → upload `index.html` → commit to `main`.
2. **Settings → Pages →** Source: *Deploy from a branch* → Branch: `main` / `/(root)` → Save.
3. Wait ~1 minute → open the URL → enter the password → hard-refresh (Ctrl/Cmd+Shift+R) if you cached an old version.

## Only commit `index.html`
Do **not** add `index_inner_UNENCRYPTED_do_not_publish.html` (the readable source) to
the public repo. `index.html` alone is safe — its contents are encrypted.

## What this dashboard is
A **regional comparison of the world's top-tier ML research** (general ML, NOT AI safety),
in the spirit of comparing economies: **Europe vs US vs China** (+ Canada + Rest of world),
with **ELLIS units highlighted**. Three sections:
1. Growth of all accepted ML papers (the pie is growing).
2. Who produces it — regional composition + Europe/US/China trend.
3. Europe & ELLIS in focus (participation, ELLIS share, European funders).

Regional split from author affiliations on a stratified random sample of **all** accepted
papers (300/venue), across ICLR/ICML/NeurIPS 2025–2026. A sampled lower bound; total
accepted counts are exhaustive. Different from the CAISI page, which is a safety dashboard.
