# InventoryLab for accounting & prep

🟡 **Intermediate.** InventoryLab (IL) replaces three tools at once: shipment building, FNSKU labeling, and cost-of-goods-sold (COGS) accounting. The \$69/mo subscription pays for itself in time savings within the first 5 shipments.

## What InventoryLab does

Three integrated functions:

### 1. Stratify (listing + shipping)
- List new ASINs in batch (paste UPCs, IL pulls Amazon data)
- Build FBA shipments faster than native Seller Central
- Print FNSKU labels directly to your thermal printer
- Generate 2D barcodes (Amazon's preferred receive format)
- Print shipping labels via Amazon Partnered Carrier

### 2. COGS tracking
- Tag every unit shipped with your cost basis
- Track per-SKU profit + ROI in real time
- Allocate landed cost (purchase price + inbound shipping + prep) per unit
- Export to QuickBooks for full accounting

### 3. Reports
- Per-SKU profit by month / quarter / year
- Inventory aging dashboard
- Sales velocity by SKU
- Reimbursement-eligible discrepancies (similar to SellerBoard)

## Setting up IL

### Step 1: Subscribe
inventorylab.com → \$69/mo. Has a free trial.

### Step 2: Connect Amazon
SP-API integration. Read-only access. 2-3 minutes to authorize.

### Step 3: Configure cost defaults

In Settings → Costs:
- **Default inbound shipping cost per pound:** \$0.40 (typical Amazon Partnered Carrier rate)
- **Default prep cost per unit:** \$0.50 (small items) to \$1.00 (oversize)
- **Default storage allocation:** \$0.10–\$0.30 per unit
- **Returns reserve:** 3–5% of revenue (haircut for expected returns)

These are baselines — you'll override per shipment.

### Step 4: Connect printer

For thermal label printing:
- DYMO LabelWriter 450/550 — most popular
- Zebra ZP450 / ZD420 — for high-volume sellers
- IL detects the printer; click "Test print"

### Step 5: Bulk-import historical COGS

If you've been selling without IL, you have phantom inventory at FBA without cost data. Two paths:

**Path A: Manual batch import**
- Export your historical orders from Seller Central
- Match each SKU to your purchase records
- Upload as CSV to IL

**Path B: Approximate from SellerBoard**
- If you set up SellerBoard first, export their cost data
- Import to IL

Without historical COGS, IL's P&L starts from when you began using IL. Older data is just a sales tally.

## The Stratify workflow

For each shipping plan:

### Step 1: Add products

Three ways:
1. **Scan UPC with phone** — IL mobile app, like SAS
2. **Paste UPCs in bulk** — desktop, fastest for >10 SKUs
3. **Manual lookup** — search by ASIN

For each SKU:
- IL auto-fetches the ASIN, title, image, BSR, Buy Box
- Confirm the matched listing is correct
- Set quantity to ship
- Set your **Buy Cost** (per unit)
- Set **List Price** (what you'll sell at)
- Specify **Condition** (New, Used Like New, etc.)

### Step 2: Print FNSKU labels

For each SKU with quantity > 0:
- Click "Print FNSKU"
- Select print quantity
- IL sends labels directly to your thermal printer

If using 2D Workflow's 2D-barcode mode: instead of FNSKU per unit, print a single 2D barcode label per box that encodes all contents.

### Step 3: Build shipment

Click "Create Shipment Plan":
- Specify ship-from address
- Choose Amazon-Optimized splits (default; cheapest)
- Confirm box count + estimated dimensions

IL submits to Amazon, which assigns warehouses.

### Step 4: Print shipping labels

After Amazon confirms the plan:
- Print FBA shipment label (top of each box)
- Print carrier label (UPS via Amazon Partnered Carrier)
- Both go on the box

### Step 5: Mark "shipped"

When carrier picks up, mark in IL. Track via the tracking number link.

Once Amazon receives + counts:
- IL updates inventory automatically
- Sales begin tracking against your COGS

## COGS tracking in detail

When a sale happens:

```
Sale price:        $25.00
- Referral fee:    -$3.75
- FBA fee:         -$3.86
- Storage (pro-rata): -$0.20
- Inbound (pro-rata): -$0.31
- Prep cost:       -$0.50
- Buy cost (COGS): -$8.00
─────
Net profit:         $8.38
ROI:                91%
```

IL's reports show this for every order. Aggregate by SKU, month, quarter, etc.

## Reports that matter

### Inventory by Age
Shows units at FBA grouped by age (0–90 days, 91–180, 181–270, 271–365, 365+).

Use to:
- Spot inventory aging into surcharge brackets
- Plan removals or price drops before LTSF hits
- See which SKUs are slow movers vs replens

### Profit by SKU
Best/worst sellers ranked by net profit, not revenue.

Use to:
- Identify SKUs to expand (top 10 by profit)
- Identify SKUs to drop (negative or marginal profit)
- Validate replen decisions (is it actually making you money?)

### Profit by Brand
Same idea but grouped by brand.

Use to:
- Spot brand-level decay (entire brand losing margin)
- Identify which brands you should pursue wholesale relationships with

### Profit by Source
If you tag where each SKU was sourced (RA: Walmart, OA: Target, Wholesale: Distributor X):
- See which sourcing channels actually produce profit
- Reallocate time to the highest-yield channel

### Cash Flow View
Estimates incoming Amazon deposits + outgoing supplier payments.

Use to:
- Avoid reordering when cash will be tight
- Plan large wholesale orders around Amazon disbursement dates

## IL vs SellerBoard

Both track P&L; both find reimbursements. Key differences:

| Feature | InventoryLab | SellerBoard |
|---|---|---|
| Listing creation | ✅ Yes | ❌ No |
| Shipment building | ✅ Yes | ❌ No |
| FNSKU label printing | ✅ Yes | ❌ No |
| Real-time profit dashboard | OK | ✅ Best-in-class |
| Reimbursement automation | OK (basic) | ✅ Excellent |
| Per-SKU profitability | OK | ✅ Best-in-class |
| Multi-marketplace support | Limited | Better |
| Cost | \$69/mo | \$15–\$50/mo |

**The BoxedUp combo:** IL for listing + shipping, SellerBoard for P&L + reimbursements. Total \$80–\$120/mo for both, replaces 3+ tools.

## When to skip IL

Some scenarios where IL isn't necessary:

### You ship <10 SKUs/month
The native Seller Central interface is slow but adequate. IL's time savings don't justify \$69/mo at low volume.

### You use 2D Workflow instead
2D Workflow (\$15/mo) covers shipment building + FNSKU labels for less. You'd still need separate P&L tools (SellerBoard).

### You have a 3PL doing everything
If your prep service builds shipments, lists products, and does FNSKU labels for you, IL is redundant. Skip and just use SellerBoard for P&L.

### You're scaling past \$100K/month
At enterprise scale, you'll outgrow IL anyway and move to dedicated bookkeeping (Bookskeep, NetSuite).

## Shipping plan tips for IL

Three things that save time:

### Use templates

For repeating shipments (replens), save the SKU list as a template. Next shipment: load template, adjust quantities, submit.

### Pre-populate cost data

Before shipping, ensure every SKU has:
- Buy cost
- Prep cost
- Sale condition

Missing data = pre-shipment error block. Fill in upfront, not at submit time.

### Match condition with listing

If you're listing as "Used Like New" but typed "New" in IL, your COGS records will be wrong. Double-check Condition every shipment.

## Reimbursement handling in IL

IL has a "Reconcile" feature that scans for:
- Sales without inventory deduction
- Inventory adjustments (lost / damaged units)
- Refunds that didn't return inventory

When discrepancies appear:
- IL shows the discrepancy with order ID + suggested action
- You manually file a case in Seller Central
- IL marks the case as "filed" once you confirm

Less automated than SellerBoard but workable. For pure reimbursement automation, SellerBoard wins.

## Workflow optimization

After 30 days using IL, optimize:

### Standardize SKU naming
Your IL SKU codes should follow a pattern:
- `WMT-12345-LEGO-MARIO` (sourced Walmart, item 12345, LEGO Mario set)
- `OA-TGT-ROYALE-MUG` (online arb Target, Royale brand, mug product)

Patterns help filter reports and identify patterns later.

### Tag sourcing source
Tag every shipment with:
- Source channel (RA / OA / Wholesale / Liq)
- Specific source (Walmart / Target / Brand X)
- Date sourced

Powerful for analyzing source-level profitability quarterly.

### Batch shipments

Instead of shipping every 3 days with 10 SKUs each, ship weekly with 30 SKUs. Saves time on:
- Shipment building setup
- FNSKU printing
- Label printing
- UPS scheduling

## Common IL issues

### Sync delays
Sometimes IL takes 1–6 hours to update after a sale. Don't panic — refresh and check the next day.

### COGS mismatch
If your IL P&L doesn't match SellerBoard's, the issue is usually missing or wrong COGS in IL. Audit a sample of orders manually.

### Printer issues
DYMO drivers occasionally hiccup. Solutions:
- Restart DYMO software
- Reinstall drivers
- Use Zebra (more reliable for heavy printing)

### Stranded inventory blocking shipments
If old listings have stranded inventory in IL, new shipments can hang. Periodically clean up:
- IL Inventory → filter "Stranded" → resolve or delete

***

Next: [SellerBoard — profit dashboard & reimbursements →](sellerboard.md)

*Last updated: 2026-05-05*
