# Deploying the ELLIS / European AI-safety dashboard (password-protected)

One file: `index.html` — a self-contained, encrypted dashboard. Same password as the
CAISI version.

- **URL (after deploy):** https://ariankhorasani.github.io/ellis-ai-safety/
- **Password:** `AISafety-Jinesis`
- Anyone with the URL + password can view and re-share it. Client-side gate — good for
  a controlled draft, not a guarantee against a determined attacker.

## Option A — GitHub website (no terminal)
1. Create a new **public** repo named **`ellis-ai-safety`** under your account.
2. **Add file → Upload files** → upload `index.html` → commit to `main`.
3. **Settings → Pages →** Source: *Deploy from a branch* → Branch: `main` / `/(root)` → Save.
4. Wait ~1 minute → open the URL above → enter the password.

## Only commit `index.html`
Do **not** add `index_inner_UNENCRYPTED_do_not_publish.html` (that's the readable
source) to the public repo. `index.html` alone is safe — its contents are encrypted.

## What differs from the CAISI version
Growth and topic charts are identical (same AI-safety papers). The third chart is the
**European & ELLIS footprint** instead of the Canadian one:
- **European affiliation** (institutions + country) and **European funder** in
  acknowledgments (ERC, Horizon Europe, Marie Skłodowska-Curie, ELLIS, DFG, ANR, EPSRC, …).
- **ELLIS units** are highlighted separately (KPI, note, and a column in the table view).
- Same stratified-sample methodology and lower-bound caveat.
