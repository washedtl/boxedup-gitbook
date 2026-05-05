# Storage fees, aged inventory, removals

🟡 **Intermediate.** The fees that quietly eat your margin if you don't manage inventory aggressively. Most beginners don't realize how much storage costs until their Q1 statement arrives.

## The three storage fees

Amazon charges three different storage fees, sometimes simultaneously on the same unit:

### 1. Monthly inventory storage fee

The base fee, charged on the 7th–15th of each month for the previous month's storage.

**Standard size:**
- Off-peak (Jan–Sep): \$0.87/cuft/month
- Peak (Oct–Dec): \$2.40/cuft/month

**Oversize:**
- Off-peak: \$0.56/cuft/month
- Peak: \$1.40/cuft/month

A typical small-standard product (4×3×2", 0.014 cuft):
- Off-peak: ~\$0.012/month
- Peak: ~\$0.034/month

Sounds tiny — multiply by 1,000 units for a year and you're looking at real money.

### 2. Aged inventory surcharge

Charged in addition to monthly storage when inventory ages past certain thresholds:

| Age | Standard surcharge | Oversize surcharge |
|---|---|---|
| 271–365 days | +\$1.50/cuft | +\$1.00/cuft |
| 365+ days | +\$6.90/cuft | +\$3.50/cuft |

For a small-std item (0.014 cuft) aged >365 days: +\$0.097/month — a tenth of a dollar **per unit per month**, on top of base storage.

A 100-unit position at 365+ days = \$9.70/month bleeding while it sits.

### 3. Long-Term Storage Fee (LTSF) — the killer

The cliff edge. Charged twice yearly (Aug 15, Feb 15) on units that have been at FBA for 365+ days:

- **\$6.90 per cubic foot OR \$0.15 per unit, whichever is greater**

For a small-std unit:
- Calculation A: 0.014 cuft × \$6.90 = \$0.097
- Calculation B: \$0.15 (the unit minimum)
- Amazon charges the **higher** = \$0.15

LTSF + monthly + aged surcharge can compound to **\$2–\$5 per year per stagnant unit.** A unit you bought for \$5 that doesn't move can cost more in fees than it cost to acquire.

## When to remove vs dispose vs liquidate vs drop-price

Decision matrix when a unit's been at FBA 180+ days:

```
Unit retail value > $5?
├─ YES →
│  Velocity > 1/month at current price?
│  ├─ YES → Hold; aggressive price drop to accelerate
│  └─ NO →
│     Can you sell it elsewhere (eBay, Craigslist) at >$5?
│     ├─ YES → Removal order (~$0.97 std, ~$3.50 oversize)
│     └─ NO → Disposal (~$0.30 std, ~$0.85 oversize) OR Liquidation
└─ NO (low-value) →
   Disposal — cheapest exit
```

The math comparison for a typical small-std unit:

| Action | Cost | Recovers |
|---|---|---|
| Hold 12 more months | \$2–\$5 fees | \$0 if it doesn't sell |
| Remove + try eBay | \$0.97 + your shipping/time | Whatever you can get |
| Dispose | \$0.30 | \$0 |
| Liquidation | Free + Amazon takes 85% | ~15% of estimated retail |
| Aggressive drop-price | Free | Whatever the market pays |

**Aggressive drop-price first. If no movement in 30 days, dispose.**

## Removal mechanics

Removal order = Amazon ships your inventory back to you (or destroys it).

How to submit:
1. Inventory → Manage Inventory
2. Select SKUs (filter by aged inventory)
3. Action → Create removal order
4. Choose **Return to address** or **Disposal**
5. Confirm — Amazon processes in 7–14 days

You'll receive in 1–3 boxes shipped via UPS to your address. Amazon's box is usually different from how you originally shipped — so if you needed pristine retail packaging, removals can damage it.

> **Removal-as-flip strategy:** some BoxedUp members use removals to recover hot inventory during stockout periods. They remove, photograph as "open box," and resell at a discount. This is fine if disclosure is clear.

## Disposal mechanics

Disposal = Amazon destroys the inventory. Cheaper than removal, no return.

Amazon's process:
- Items are sent to e-waste / recycling / dumpster depending on category
- You get a confirmation in 14 days
- **No refund** — disposal cost is final

This is the fastest IPI-rescue tool. Don't be sentimental about \$5 inventory.

## Amazon Liquidation

A relatively new option. Amazon partners with liquidators to bulk-buy your unsellable inventory:

- You opt in via Inventory → Manage Inventory
- Set a price floor (e.g., 10% of retail)
- Amazon takes 85%+, gives you the remainder
- Inventory leaves FBA same week

When to use: you have a large position (50+ units) of dying inventory and want speed > value recovery. Otherwise, drop-price first.

## The aged inventory dashboard

In Seller Central → Inventory → Inventory Age:

| Bucket | Amazon's traffic light |
|---|---|
| 0–90 days | Green |
| 91–180 days | Yellow |
| 181–270 days | Orange |
| 271–365 days | Red — surcharge active |
| 365+ days | Severe red — LTSF imminent |

**Review every Monday.** Items entering the 271-day bucket = action this week (drop price, remove, or dispose). Letting things slide into the 365+ bucket is how IPI tanks and fees compound.

## A real example

A BoxedUp member's January 2025 statement showed:

| Line item | Amount |
|---|---|
| Monthly storage (Q4 inventory still onsite) | \$1,247 |
| Aged inventory surcharge | \$184 |
| Disposal fees (rescue removals) | \$67 |
| Long-term storage fee | \$398 |
| **Total fee bleed** | **\$1,896** |

Their gross margin on Q4 was \$23K — fees ate 8.2% of profit. After they implemented the weekly aged-inventory review, the same fee bleed dropped to ~\$340/month — saving \$1,500/month in pure margin recovery.

## The aging discipline

Three habits that compound:

1. **Don't ship in losers.** If a SKU can't sell in 60 days at current velocity, don't ship it. Period.
2. **Drop price at 90, 180, 270 days.** Cut 15% at each milestone. Force movement before fees compound.
3. **Dispose at 270.** If 15% drops haven't moved it after 9 months, it's not going to. Eat the loss.

> **The opposite mistake** is over-pruning. Some replens are seasonal and look like aging losers in their off-season. Don't dispose Christmas decor in March — that's Q4 inventory at off-peak storage cost. Look at trailing-12-month velocity, not 30-day.

***

Next: [Multi-pack & bundle rules →](bundles.md)

*Last updated: 2026-05-05*
