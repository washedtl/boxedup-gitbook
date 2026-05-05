# FBA vs FBM vs SFP

🟢 **Beginner.** The choice between fulfillment models shapes your entire operation. Most BoxedUp resellers run FBA-only — here's why, and when the others make sense.

## The three models

| Model | Who ships | Prime badge | Storage | Customer service |
|---|---|---|---|---|
| **FBA** (Fulfilled By Amazon) | Amazon | ✅ Yes | Amazon warehouse | Amazon |
| **FBM** (Fulfilled By Merchant) | You | ❌ No | Your space | You |
| **SFP** (Seller Fulfilled Prime) | You | ✅ Yes | Your space | You + Amazon SLAs |

## Why BoxedUp defaults to FBA

Three reasons, in order of importance:

### 1. The Buy Box weighs FBA heavily

Amazon's Buy Box algorithm prefers FBA offers. All else equal:
- FBA at \$25 will win Buy Box vs FBM at \$24
- Sometimes even FBA at \$26 beats FBM at \$24

**Buy Box = ~85% of sales.** If you don't win it, your inventory sits.

### 2. Prime customers buy more

A Prime customer sees the badge and trusts the listing. Conversion rates on FBA listings are typically **15–30% higher** than FBM. Multiply that across hundreds of units and the math is unforgiving.

### 3. Speed = scale

When you scale past ~50 units/month, packing and shipping yourself becomes a part-time job. FBA lets you keep sourcing and let Amazon handle the boring parts. Most BoxedUp members hit this ceiling within their first 3 months.

## What FBA costs

You don't get FBA for free. The fees:

- **Pick & pack fee** — \$3.22 (small standard) → \$6+ (large standard) → \$10+ (oversize)
- **Storage fee** — ~\$0.87/cuft/month off-peak, ~\$2.40 peak (Q4)
- **Inbound placement fee** — newer fee, \$0.30–\$1.50/unit if you ship to fewer warehouses
- **Long-term storage fee** — penalty for inventory aged 271+ days
- **Returns processing fee** — applies to apparel + footwear in some categories

A typical \$25 sale with FBA pays out roughly:
```
$25.00  Sell price
-$3.75  Referral (15%)
-$3.86  FBA pick/pack (small std, ≤1 lb)
-$0.50  Inbound shipping (your cost to FBA)
-$0.30  Inbound placement fee
-$0.20  Pro-rata storage / returns / misc
─────
$16.39  Pre-COGS net
```

Always model fees with the **FBA Revenue Calculator** (free, in Seller Central) — your gut will be wrong.

## FBM tactical levers (if you do choose FBM)

Two specific tactics that move the needle for FBM operations:

### Lever 1: USPS PostalPro service-standards heat map

Amazon defaults to flat 2-4 day handling-time estimates. This is wrong for FBM — actual transit varies wildly by destination.

The fix: use **USPS PostalPro service-standards heat map** (`postalpro.usps.com/ppro-tools/service-standards-maps`).

Workflow:
1. Look up your warehouse zip's **first 3 digits**
2. Pull the heat map showing transit time to every other zip-3 in the country
3. In Seller Central → Shipping Settings, configure **per-state handling time**:
   - Nearby states: 2-4 days promised
   - Cross-country: 5-8 days promised

Result: more accurate delivery promises = fewer late-shipment defects = better LSR + Buy Box weight. **Saves money** by avoiding upgrades to faster shipping classes for far destinations.

### Lever 2: Handling time = 0

Set your shipping handling time to **0 days** (Settings → Shipping → Default Handling Time → 0).

What this does: customer sees "Get it by [tomorrow]" instead of "Get it by [3 days from now]" because Amazon's promised-delivery calc starts from order placement, not ship date.

Trade-off:
- ✅ Earlier delivery date shown to customer = higher conversion + better Buy Box weight vs FBA competitors
- ❌ You MUST actually ship same-day or you'll rack up Late Shipment Rate defects

Run this only if you can genuinely ship same-day. For most BoxedUp members shipping FBM as overflow: works mid-week (Mon-Thu); switch to 1-day handling for weekend orders.

### Lever 3: Buy Box eligibility audit

Many FBM sellers don't realize they're flagged Buy-Box-ineligible on specific ASINs.

To check:
1. Inventory → Manage Inventory
2. Click "Preferences" (top right)
3. **Tick "Buy Box Eligible" column**
4. Save

Now your inventory list shows Buy Box eligibility per-SKU. For ineligible SKUs:
1. Open Help → Contact us → "I want to sell on Amazon" → "Listing — Other"
2. Request review of Buy Box eligibility for the specific ASIN
3. Provide your performance metrics + history

This often unlocks Buy Box for SKUs you've been "selling but invisible" on.

## When FBM makes sense

FBM is the right call in these specific cases:

### Oversize / heavy items
A 25 lb piece of exercise equipment can have FBA fees > \$25. Same item via FBM with cheap freight might net you 3× more per unit — even without the Buy Box.

### Hazmat
Some hazmat is FBA-restricted entirely. If you want to sell it, FBM is your only option.

### Long-tail slow movers
If a unit will take 6+ months to sell, FBA storage fees + LTSF eat the margin. Better to ship FBM from your closet.

### Drop-shipping (rare, risky)
Some BoxedUp members FBM-fulfill from a wholesaler's warehouse using shipping integrations. **Only works if** you can guarantee 2-day shipping, accurate inventory feeds, and no late-shipment defects. Most beginners crash and burn here.

## When SFP makes sense

SFP gives you the Prime badge while shipping yourself. **The qualifying bar is brutal:**

- 99% on-time shipment rate
- ≤ 0.5% late shipment rate
- ≤ 1% cancellation rate
- 99% valid tracking rate
- Saturday delivery for most ZIPs
- Premium shipping integrations (typically UPS or FedEx contracts with negotiated rates)

If you're scaling past ~\$25K/month and have a real warehouse, SFP unlocks Prime margins on items where FBA fees are uneconomic. **Don't even apply** until you have warehouse + integrations + a 6-month track record on FBM.

## The Hybrid model

Most pro BoxedUp resellers run **FBA primarily + FBM as overflow:**

- Default everything to FBA
- When FBA inventory runs out and you have local stock, FBM at the same price to keep the listing alive
- When a customer wants overnight and you're closer to them, FBM with expedited shipping
- For oversize items where FBA economics don't work, FBM-only

The combo gives you Buy Box dominance via FBA + the flexibility of FBM for edge cases.

## Decision flow

```
Is the unit oversized (>20 lb, longest side >18")?
├─ YES → FBM (or FBA if velocity supports it)
└─ NO →
   Is the unit hazmat?
   ├─ YES → check FBA-restricted list; if restricted → FBM
   └─ NO →
      Is velocity ≥ 5/month?
      ├─ YES → FBA (Prime badge + Buy Box weighting > FBM advantages)
      └─ NO → FBM (storage fees would eat slow movers)
```

90%+ of BoxedUp flips end up on FBA via this flow.

***

Next: [How a shipment actually flows →](shipment-lifecycle.md)

*Last updated: 2026-05-05*
