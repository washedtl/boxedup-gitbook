# How to import this into your GitBook

These files are GitBook-formatted Markdown ready to drop into `simplecops-organization.gitbook.io/boxedup`.

## What's in this folder

```
c:/tmp/boxedup-gitbook/
├── README.md                  # Cover / landing page
├── SUMMARY.md                 # The TOC GitBook reads to build the sidebar
├── .gitbook.yaml              # Tells GitBook this is the root
├── assets/
│   └── custom.css             # Dark BoxedUp theme (purple #BE8AFF accent)
├── getting-started/           # How to use, mental model, glossary
├── seller-account/            # Pro vs Individual + 5 stub pages (sidebar entries)
├── fba/                       # 7 stub pages
├── sourcing/                  # A2A, Restock/Monitor, Restock-Monitoring + 7 stubs
├── tools/                     # Keepa, KPF, RAM case study, SellerBoard + 2 stubs
├── deal-analysis/             # Profit equation + 5 stubs
├── seller-central/            # 6 stubs
├── business-setup/            # 6 stubs
└── anti-patterns/             # IP complaints + 5 stubs
```

**Pages with real content (~3,000–8,000 words each):**
- README.md
- getting-started/how-to-use.md
- getting-started/mental-model.md
- getting-started/glossary.md
- seller-account/pro-vs-individual.md
- sourcing/retail-arbitrage.md
- sourcing/a2a.md
- sourcing/restock-monitor-strategy.md
- sourcing/restock-monitoring.md
- tools/keepa.md
- tools/keepa-product-finder.md
- tools/the-ram-shortage-case-study.md
- tools/sellerboard.md
- deal-analysis/profit-equation.md
- anti-patterns/ip-complaints.md

**Pages referenced in SUMMARY.md but not yet written** (GitBook will create empty pages or 404 for these — fill in over time):
- All sub-pages under fba/, seller-central/, business-setup/, anti-patterns/* (except IP), reference/, and the remaining sourcing/*, tools/*, deal-analysis/*, seller-account/* slugs.

## Three ways to import

### Option 1 — GitBook web editor, page by page (slowest, no setup)

1. Open https://simplecops-organization.gitbook.io/boxedup
2. Click `+ New page` for each page in `SUMMARY.md`, in order
3. Paste the Markdown body of each file
4. Save

Tedious for 80+ pages, but works without git.

### Option 2 — Connect a fresh GitHub repo (recommended)

1. Create a new GitHub repo, e.g. `simplecop/boxedup-gitbook`
2. From `c:/tmp/boxedup-gitbook/`:
   ```bash
   cd c:/tmp/boxedup-gitbook
   git init
   git add .
   git commit -m "Initial BoxedUp GitBook import"
   git branch -M main
   git remote add origin git@github.com:simplecop/boxedup-gitbook.git
   git push -u origin main
   ```
3. In GitBook (the BoxedUp space): Settings → **Git Sync** → connect GitHub → pick `simplecop/boxedup-gitbook` → branch `main` → root `/`
4. GitBook ingests all files and builds the sidebar from `SUMMARY.md`
5. Future edits: push to GitHub → GitBook auto-rebuilds

This is the canonical way to run a GitBook at scale.

### Option 3 — Use GitBook's import-from-Markdown feature

GitBook has an "Import" option (Settings → Import) that accepts a `.zip`. Zip the folder:

```bash
cd c:/tmp/
powershell -Command "Compress-Archive -Path 'boxedup-gitbook' -DestinationPath 'boxedup-gitbook.zip'"
```

Upload the zip via Import. GitBook will create pages from each file.

## Applying the custom theme (`assets/custom.css`)

GitBook has tiered customization:

- **Free / Personal:** limited theming — set primary color, light/dark mode in Site → Customization
- **Pro / Business:** full custom CSS injection. Paste the contents of `assets/custom.css` into Site → Customization → Custom CSS

If you're on the free tier, the custom CSS won't apply automatically. The Markdown will still render fine; it'll just use GitBook's default theme.

**Alternative:** the design tokens in `custom.css` are simple to translate to GitBook's built-in customizer:
- Primary color: `#BE8AFF`
- Brand gradient: `linear-gradient(136deg, #A052FF 0%, #4E2DD2 100%)`
- Mode: Dark

## What to do before publishing

1. **Read README.md** — confirm the welcome copy matches your voice
2. **Read getting-started/mental-model.md** — this is the methodology page; make sure it represents your approach faithfully
3. **Read tools/keepa.md** + `tools/keepa-product-finder.md` — these are the long-form methodology pages
4. **Read tools/the-ram-shortage-case-study.md** — it's the worked example pulled from the BoxedUp Context File. Confirm you're comfortable making it public.
5. **Decide what to leave private** — some content (Tempo command syntax, Blaze API references) may be Discord-members-only. Move those into a private GitBook space if you want them gated.
6. **Fill in or remove stub pages** — pages referenced in `SUMMARY.md` without content will show as empty. Either write them or remove the entries.

## Things to double-check / customize

- The Discord webhook + Blaze API key in the original BoxedUp Context File are NOT included in any GitBook page (they shouldn't be public). If they ended up in any draft, do a final grep before publishing.
- Brand exclusions in `tools/keepa-product-finder.md` are illustrative — replace with your actual exclusion list if you want it canonical.
- Top-15 picks table in `tools/the-ram-shortage-case-study.md` is from late-2024 / 2025 data — note in the page that pricing is historical and not actionable today.
- The `last updated` dates at the bottom of each page are placeholder `2026-05-05`. Update as you edit.

## Sequence to fill in remaining stubs

The pages already-written give the spine. Suggested order to fill in the stubs:

1. **Glossary remaining terms** in `reference/glossary-full.md`
2. **FBA mechanics** — fba/* (referenced from RA + A2A pages)
3. **Deal analysis remaining** — velocity.md, competition.md, when-to-walk.md
4. **Seller Central operations** — reimbursements is highest-leverage; the rest can wait
5. **Anti-patterns remaining** — gating, hijackers, suspension
6. **Discord internals** — channels, roles, bot commands (only if you want this public)
7. **Business setup** — LLC, sales tax, reseller certs
8. **Reference appendices** — fee tables, prep matrix

## When you publish

The live URL will be:
```
https://simplecops-organization.gitbook.io/boxedup
```

Each page has a stable URL based on its file path, e.g.:
```
https://simplecops-organization.gitbook.io/boxedup/tools/keepa
https://simplecops-organization.gitbook.io/boxedup/sourcing/restock-monitor-strategy
```

You can link to individual pages from Discord — `#guide` channel pinned messages, server rules, role-gate pages, etc.

Good luck shipping.
