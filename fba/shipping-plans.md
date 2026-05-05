# Building shipping plans

🟢 → 🟡 — How to take inventory in your hand and turn it into a clean shipment Amazon will receive without errors.

## The shipping plan flow

A "shipping plan" is what Amazon calls the workflow of sending inventory to FBA. The path:

```
Inventory in hand → Create shipment → Print labels → Ship → Receive at FBA
```

We covered the high-level lifecycle in [Shipment lifecycle](shipment-lifecycle.md). This page goes deeper on building the plan itself.

## Tools to build with

Two options, ranked:

### Option 1: Inventory Lab (recommended)
Handles box content, FNSKU labels, and dimensions in one screen. ~5 minutes per shipment for 50 SKUs.

### Option 2: Native Seller Central
Slow, multi-step, error-prone, but free. ~25 minutes per shipment for 50 SKUs.

For this page, examples assume you're using Inventory Lab.

## Building the plan: step by step

### Step 1: List products

For each SKU you're shipping:
- Confirm the listing exists on Amazon (or create if new ASIN)
- Set your **Selling Price** (this is what you'll list at, not your cost)
- Set your **Cost** (your COGS — used for P&L)
- Set **Quantity** to ship

If the listing doesn't exist yet:
- Click "Create listing"
- Match the existing ASIN if it's already on Amazon
- For brand-new ASINs (very rare for arbitrage): full listing creation with title, images, etc.

### Step 2: Print FNSKU labels

Amazon assigns each listing an FNSKU (Fulfillment Network SKU) — your unique barcode for that ASIN.

In your shipping tool:
- Print FNSKU labels on thermal sticker paper (DYMO 30334 or 30330)
- Apply one label per unit, on a flat surface
- Cover the existing UPC if possible (not strictly required but reduces commingle risk)

For a 50-unit shipment: ~10 minutes of label-printing + applying.

### Step 3: Build the shipment

Now you tell Amazon:
- **Ship from** your warehouse / home address
- **Ship to** Amazon's network (they'll auto-assign warehouses)
- **Box dimensions** for each box you'll send
- **Box weights** for each box
- **Box contents** — which SKUs go in which box, and quantities

This is the most error-prone step. Get it wrong and:
- Wrong dimensions → oversize charges
- Wrong weights → re-bill
- Wrong box contents → "received less than expected" claims

### Step 4: Choose placement option

Amazon offers three "shipment splits":

| Option | Inbound fee | Speed | When to use |
|---|---|---|---|
| **Amazon-Optimized** | \$0–\$0.30/unit | Fastest | Default for most shipments |
| **Partial Splits** | \$0.50–\$1.00/unit | Medium | When you want fewer boxes but still some splits |
| **Minimal Splits** | \$1.00–\$1.50/unit | Slowest | Single-box shipments to one warehouse |

Math: for a 50-unit shipment of \$15-cost items, the difference between optimized (\$0.20/unit) and minimal (\$1.20/unit) is \$50 in fees. **Always pick optimized unless you have a specific reason.**

### Step 5: Print box and shipping labels

For each box, you get:
- **FBA shipment label** (put on top) — Amazon's QR code
- **Carrier shipping label** (UPS, FedEx, etc.) — usually on side or top

Most modern tools print both at once. If your tool generates a 2D barcode label that combines content + shipment info, even better — that's the [2D barcode workflow](third-party-tools.md#what-is-2d-barcode-shipping) Amazon prefers.

### Step 6: Submit and ship

After printing:
- Submit the shipment in your tool (this confirms with Amazon)
- Pack boxes physically
- Schedule UPS pickup OR drop off at carrier
- Tracking number activates automatically

## The "box content" decision

Amazon offers two ways to declare box contents:

### Option A: Web Form (default for new sellers)

You manually type each SKU + quantity per box. Tedious for >5 SKUs per box.

### Option B: Box Content Information File (CSV upload)

You upload a spreadsheet listing every SKU + quantity per box. Faster for >10 SKUs per box.

### Option C: 2D Barcode (best)

The 2D barcode encodes the box contents directly. Your tool generates it. Amazon scans it on receipt. **No web form, no CSV.**

Inventory Lab supports 2D barcodes. **Enable it as the default in your tool's settings** — saves time + faster receive at FBA.

## Common shipping plan mistakes

### Mistake 1: Wrong dimensions or weights

You estimated "small box, ~3 lbs." It's actually 4 lbs. Amazon's billing system catches this and re-bills you.

**Fix:** weigh every box on a postal scale before submitting. Don't guess.

### Mistake 2: Mixed conditions in one box

You have 5 "New" units of SKU A and 3 "Used - Like New" of SKU B in the same box. Amazon's commingled receiving may treat them all as one condition.

**Fix:** keep distinct conditions in distinct boxes.

### Mistake 3: Hazmat in same box as non-hazmat

Some hazmat units (lithium batteries, aerosols) require segregation from non-hazmat. Mixed boxes get sent to a hazmat-only warehouse, slowing receive for everything.

**Fix:** ship hazmat in dedicated boxes.

### Mistake 4: Over-packing single boxes

A 100 lb box of small items takes ~7 days to receive at FBA. The same 100 units in 2× 50 lb boxes receives in 3–4 days.

**Fix:** target 30–40 lb per box. Faster receive, lower handling damage rate.

### Mistake 5: Ship-from address mismatch

Your seller account address says "123 Main St, Apt 4" but you're shipping from "123 Main St, Unit 4." Some carriers mishandle this.

**Fix:** keep ship-from address consistent across Seller Central, your shipping tool, and the carrier label.

## Pre-Q4 shipment timing

A specific Q4 calendar:

| Date | Action |
|---|---|
| Sep 1–30 | Q4 prep — clean up IPI, build replen inventory |
| Oct 1–14 | First Q4 shipping wave; deliver by Oct 25 |
| Oct 15–31 | Last shipping for Black Friday inventory; deliver by Nov 15 |
| Nov 1–14 | Final shipping for Christmas-week inventory |
| Nov 15+ | Q4 receive times exceed 2 weeks; risky |
| Dec 1–24 | Don't ship; sell what's at FBA |
| Dec 26–Jan 15 | Cleanup wave (returns, removals, low IPI rescue) |

Shipping in late November is gambling. By December 1, expect units to receive in January — too late for Christmas.

## Shipping plan templates

For repetitive shipments (same SKUs, same quantities), most tools support **templates:**
- Save a recurring shipment plan as a template
- Next time, click "use template" → adjust quantities → submit
- Saves 5–15 minutes per repeat shipment

Use templates aggressively for replens. After 5 cycles, you'll thank yourself.

## When to outsource

The math on outsourcing prep / shipment building:

- Your time at \$50/hour → 30 min per shipment = \$25/shipment cost in time
- Prep service at \$0.75/unit × 40 units = \$30/shipment
- Roughly break-even

Below \$10K/month: do it yourself.
\$10K–\$30K/month: consider outsourcing prep specifically (you keep building shipments, prep service preps + ships).
\$30K+/month: full outsource (prep service does everything; you just send inventory to them).

***

Next: [IPI score deep dive →](ipi.md)

*Last updated: 2026-05-05*
