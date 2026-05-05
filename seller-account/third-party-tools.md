# Inventory Lab, 2D Workflow, SellerAmp setup

🟢 → 🟡 — The four tools that take you from "fumbling with Amazon's clunky default UI" to "shipping 50 SKUs/hour like a pro."

## What you actually need

The minimum essential reseller toolset:

| Tool | Cost | What it does |
|---|---|---|
| **Keepa** (paid) | \$19/mo | Chart history, KPF, API access |
| **SellerAmp SAS** | \$22/mo | Real-time scanning + deal analysis |
| **Inventory Lab** OR **2D Workflow** | \$69/mo IL, \$15/mo 2D | Listing creation + shipment building |
| **SellerBoard** | \$15–\$50/mo | P&L + reimbursement automation |

Total: ~\$75–\$160/month.

For most members past the first 3 months, this combo pays for itself in a single week of saved time + reimbursements found.

## Setting up SellerAmp SAS

The scanner that runs on your phone (and desktop). Most-used tool in the BoxedUp community.

### Subscription tiers

- **Standard** (\$22/mo) — full features, good for solo sellers
- **Multi-user** (\$30+/mo) — adds team logins for VAs / partners

### Setup

1. **Sign up** at sellamp.com
2. **Connect Amazon SP-API** — read-only access via Seller Central
3. **Connect Keepa** — paste your Keepa API key (Keepa.com → Settings → API Access)
4. **Configure default ROI thresholds:**
   - Min ROI: 30% (RA), 20% (OA), 15% (wholesale)
   - Min profit per unit: \$3
   - Max FBA seller count: 5
   - Max BSR: top 5% of category
5. **Install Chrome extension** for desktop scanning
6. **Install mobile app** (iOS / Android) for in-store scanning
7. **Test scan** — visit any Amazon listing → click the SAS extension → it should populate Buy Box, fees, ROI, gating

### What SAS shows you

A typical SAS scan returns:
- ✅ **Eligibility** — gated / restricted / open
- 💰 **Buy Box price** — current
- 📊 **BSR + category rank** — current + 30/90 day averages
- 👥 **Offer count** — total / FBA / FBM
- 💵 **Fees breakdown** — referral + FBA + storage estimate
- 📈 **ROI calculator** — input your cost, get net profit
- 📅 **Keepa chart** — quick visual check
- 🚨 **Brand IP risk** — green/yellow/red flag

The ROI calculator is the fastest part. Type your cost, see profit instantly. Don't even need a separate fee calculator.

### Scanning workflow

In-store:
1. Open SAS app
2. Camera mode
3. Scan UPC barcode on the unit
4. Wait ~1 second for results to populate
5. Decision in <60 seconds

Desktop / online:
1. Visit Amazon listing
2. Click SAS Chrome extension
3. Adjust input cost
4. Decision in <30 seconds

After 100 scans, you're at <10 seconds per decision.

## Setting up Inventory Lab

Inventory Lab (IL) handles listing creation, shipment building, and bookkeeping.

### What it does

- **Stratify** — list new ASINs in batch (paste UPCs, IL pulls Amazon data + your costs)
- **Shipment workflow** — ship to FBA in fewer clicks than Seller Central
- **Reports** — P&L by SKU, sales velocity, inventory aging
- **Print** — FNSKU labels, box content forms, shipping labels

### Setup

1. **Sign up** at inventorylab.com (\$69/mo)
2. **Connect Amazon SP-API**
3. **Calibrate cost defaults:**
   - Inbound shipping (your average per-pound cost to FBA)
   - Prep cost (your time + materials per unit)
   - Misc per unit (bags, labels, tape)
4. **Print thermal label setup** — DYMO 450/550 connection
5. **Test with a small shipment** — list 5 SKUs, build a shipment, print labels

### The IL workflow advantage

Compare native Amazon Seller Central vs IL for shipping 50 SKUs:

| Step | Seller Central | Inventory Lab |
|---|---|---|
| Add new ASINs | One at a time | Bulk paste UPCs |
| Enter costs | Type per item | Bulk CSV |
| Print FNSKU labels | Generated PDFs, manual | Direct to thermal printer |
| Shipment building | Multi-page wizard | Single screen |
| Time for 50 SKUs | 90+ minutes | 25–35 minutes |

After ~5 shipments, IL pays for itself in time saved every month.

## 2D Workflow — the alternative

2D Workflow is a newer entrant, often preferred by high-volume sellers.

### Why some prefer 2D Workflow

- ✅ **Cheaper** (\$15/mo vs \$69/mo)
- ✅ **2D-barcode-based shipping** — Amazon's preferred mode, faster receive times
- ✅ **Simpler interface** — fewer features, less learning curve
- ❌ **Less bookkeeping** than IL — you'll need SellerBoard for P&L

### What is "2D barcode" shipping?

In 2024, Amazon rolled out 2D barcodes (QR codes) on FBA shipments. The 2D barcode encodes box content directly — Amazon's warehouse scanners read it instantly, eliminating manual counting.

Benefits:
- ⚡ **Faster receive times** at FBA — sometimes same-day instead of 3–7 days
- 📋 **Fewer "mis-counted" disputes** — Amazon trusts the 2D content
- 🏷️ **Single label per box** combines shipment + content info

To use 2D barcodes, your shipping software must generate them correctly. **Both Inventory Lab and 2D Workflow support it.** Native Seller Central also supports it but the workflow is clunkier.

If you're shipping >5 boxes/week, **enable 2D barcodes via your shipping tool** — pure speed win.

### 2D Workflow setup

1. **Sign up** at 2dworkflow.com
2. **Connect SP-API** + Keepa
3. **Configure printer** (DYMO or Zebra)
4. **Set cost defaults**
5. **Run a test shipment**

Same playbook as IL, just simpler.

## SellerBoard setup

For P&L + reimbursements. Already covered in detail at [SellerBoard page](../tools/sellerboard.md).

Quick setup checklist:

1. ✅ Sign up at sellerboard.com
2. ✅ Connect SP-API
3. ✅ Wait 24 hours for historical data ingest
4. ✅ Bulk-upload COGS (export from IL if you're using it)
5. ✅ Set per-unit prep + shipping costs
6. ✅ Verify P&L on a few orders

## Browser extensions stack

Beyond SAS, three Chrome extensions are common:

### Keepa Browser Extension
Free with Keepa subscription. Adds the Keepa chart inline on every Amazon product page.

- Install from Chrome Web Store: "Keepa - Amazon Price Tracker"
- Sign in with your Keepa account
- Chart appears below the buy box on every Amazon listing

### Camelizer
Backup price-tracker. Sometimes catches things Keepa misses, especially for short-term Amazon-direct prices.

### Honey / Capital One Shopping
For sourcing — find coupon codes when buying inventory online. Free.

## Mobile setup

Two apps you should have:

### SellerAmp (mobile)
For in-store scanning. iOS and Android.

### Amazon Seller (mobile)
Amazon's official app. Useful for:
- Quick inventory checks
- Responding to customer messages
- Receiving urgent account-health notifications

Don't use it for primary work — desktop Seller Central is better. But have it installed for emergencies.

## Cost summary

A starter toolkit:

| Tool | Annual cost |
|---|---|
| Keepa (paid) | \$228 |
| SellerAmp SAS | \$264 |
| 2D Workflow | \$180 |
| SellerBoard | \$300 (mid-tier) |
| **Total** | **\$972/year** |

If you're netting >\$10K/month, this is <1% of revenue. Cheaper version (Keepa free + SAS only): \$264/year for the bare minimum.

## What NOT to buy initially

Save your money on:

❌ **Aura / RepricerExpress** — only useful past \$25K/month
❌ **Helium 10 / JungleScout** — designed for PL, overkill for arb
❌ **AMZ Tracker / similar** — feature-overlap with what you already have
❌ **Paid courses ("\$2000 Amazon FBA Mastery!")** — this guide replaces 90% of them; the rest is in your Discord

## When to upgrade

Triggers to add new tools:

| Trigger | Add |
|---|---|
| Shipping >100 units/week | Aura repricer |
| Sourcing >\$5K/month from one supplier | Wholesale-specific tools (Forecastly, Restock Pro) |
| Operating with VAs | Time-tracking + multi-user SAS |
| Past \$25K/month revenue | Bookskeep / dedicated CPA |
| Past \$50K/month | 3PL prep services replacing IL prep |

***

Next: [Surviving your first 90 days →](first-90-days.md)

*Last updated: 2026-05-05*
