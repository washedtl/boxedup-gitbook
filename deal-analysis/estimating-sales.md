# Estimating monthly sales

🟡 **Intermediate.** A core sourcing skill: take what you see in Keepa + on the listing, and turn it into a credible monthly sales estimate for YOU specifically.

## Why you need this

Without an estimate, you're guessing whether to buy 5 units, 50, or 500. Wrong-direction guesses mean:
- Too many → inventory sits, fees pile up, IPI tanks
- Too few → you sell out fast, lose Buy Box momentum, miss profit

The estimate is your inventory-decision driver.

## The simple formula

```
Your estimated monthly sales = 
    (Total monthly units sold) 
    × (FBA Buy Box share) 
    / (FBA seller count + 1)
```

Each piece broken down:

### Total monthly units sold

Three sources, in order of accuracy:

**Source 1: "Bought in past month" badge** — Amazon's own data
- "50+ bought" ≈ 50–99 units
- "100+ bought" ≈ 100–499
- "500+ bought" ≈ 500–999
- "1K+ bought" ≈ 1,000–4,999
- "5K+ bought" ≈ 5,000–9,999
- "10K+ bought" ≈ 10,000+

**Source 2: Keepa BSR drops**
30-day BSR drops ≈ total monthly sales (across all sellers including FBM).

**Source 3: BSR-to-sales conversion**
Older method, less reliable now. Various tools claim BSR # → sales/day mappings, but Amazon's algorithm has shifted. Use as last resort.

### FBA Buy Box share

What % of sales went through FBA offers (vs FBM, vs Amazon)?

- If Amazon currently in stock: FBA share could be 5% (Amazon dominates)
- If only FBA sellers + few FBM: FBA share ≈ 85–95%
- If many FBM with low prices: FBA share could drop to 60–70%

Default assumption: if no Amazon, no SFP, just FBA + FBM resellers: **85% FBA share.**

### FBA seller count + 1

You + the existing FBA sellers competing for Buy Box rotation.

Worth noting: "FBA seller count" you see on a listing is the CURRENT count. It can change. Estimating future is harder. Use current as a proxy for the next 30 days.

## Worked examples

### Example 1: Hot replen

```
"500+ bought in past month" badge   → 500 total monthly sales (low end)
FBA share: 90% (no Amazon, mostly FBA)  → 450 FBA-fulfilled sales
FBA sellers competing: 5 (you + 4)      → 450 / 5 = 90 sales/month

Your estimate: ~90 units/month
```

If profit/unit is \$3, that's \$270/month from this SKU. Solid.

Inventory plan: hold 30–45 days of supply at FBA. So 90–135 units to start.

### Example 2: Niche / low velocity

```
30-day BSR drops: 12                     → 12 total monthly sales
FBA share: 85%                            → 10 FBA-fulfilled
FBA sellers: 1 (just you)                 → 10 / 1 = 10 sales/month

Your estimate: ~10 units/month
```

If profit/unit is \$10, that's \$100/month. Worth it if it's a stable replen.

Inventory: 15–20 units initially, restock when you hit 5.

### Example 3: Saturated listing

```
"5K+ bought in past month"               → 5000 total monthly sales
FBA share: 75% (some Amazon presence)    → 3750 FBA
FBA sellers: 25 (you + 24)               → 3750 / 25 = 150 sales/month

Your estimate: ~150 units/month
```

Sounds good — but 25 FBA sellers means race-to-bottom pricing. Margin/unit might be \$1 (if \$5 originally, war-driven down). That's \$150/month for huge competition headache.

Skip — better SKUs out there with similar revenue but less competition.

### Example 4: Amazon present, occasional gaps

```
30-day BSR drops: 200                    → 200 total monthly sales
Amazon orange line: present 80% of month → Amazon takes 60% of sales
FBA share when Amazon out: 90%
FBA sellers: 4

Calculation:
- Sales when Amazon out (20% of time): 200 × 0.20 × 0.90 / 5 = 7.2/month
- Sales when Amazon in (80% of time): 200 × 0.80 × 0.05 / 5 = 1.6/month
- Total your share: ~9 sales/month
```

Lower than it appeared. Amazon's presence eats most of the demand.

## Adjustments for special cases

### New listings (<90 days)
Multiply by 0.5 — early data is unreliable. Estimate cautiously.

### Listings with stranded inventory
Inflated drop count from your competitors' inventory issues. Multiply by 0.7.

### Q4 vs off-peak
Q4 sales can be 2–3× off-peak for many categories. If you're estimating in October for Christmas inventory: multiply by 2.

### After an offer-count spike
A pile-on lowers per-seller share immediately. If FBA count went from 3 to 10 in a week, recalculate using new count.

### Brand-Registered with brand selling
Brand owner often takes 50–80% of Buy Box. Multiply your estimate by 0.2–0.5.

### Variation listings
Total sales are spread across all variations. Estimate per-variation, not per-parent. A "5K bought" parent listing might mean 50 sales for your specific size/color variation.

## Confidence intervals

Single-number estimates feel false-precise. Use ranges:

| Confidence | Range relative to estimate |
|---|---|
| High (12+ months stable history) | ±20% |
| Medium (3–12 months) | ±35% |
| Low (1–3 months) | ±60% |
| Very low (new listing, volatile) | ±100% |

If your estimate is "10 units/month" with ±60% range, the actual could be 4 or 16. Plan inventory and capital for the worst case (4) but don't refuse to source the upside (16).

## Reverse estimation: how much inventory should you ship?

Once you have the estimate:

```
Inventory at FBA = (Estimated monthly sales) × (Days of supply / 30)
```

Default: 30 days of supply. Rationales:
- FBA storage at off-peak is cheap; 30 days don't cost much
- Faster than that = stockout risk
- Slower than that = aged inventory + IPI hit

For replens you've proven over 3+ months: bump to 45–60 days.

For seasonal: 90+ days (seasonal storage premium acceptable for replens you'll sell through).

## When estimates fail

Common ways estimates go wrong:

### Failure 1: New competitor enters

Your estimate assumed 4 FBA sellers. Two weeks after you ship, 3 more enter. Per-seller share drops 60%.

**Fix:** monitor offer count weekly. If it changes meaningfully, drop price or move to clear inventory.

### Failure 2: Brand IP claim

You projected 50 units/month. Day 12, brand files inauthentic complaint. Sales go to 0 while you appeal.

**Fix:** include this risk in your inventory decision. Don't ship 90-day supply on Tier 1 brand.

### Failure 3: Buy Box price tanks

Your estimate assumed \$25 Buy Box. Sellers race-to-bottom to \$18. Profit/unit halves.

**Fix:** your estimate should include "if Buy Box drops 15%" stress test. Decide if you're still sourcing.

### Failure 4: Seasonal fade

You sourced August expecting "summer demand." It's now September, demand drops 70%. Inventory sits until next summer.

**Fix:** check 12-month chart for seasonality before sourcing summer/winter items.

### Failure 5: Listing suppression

Brand or Amazon suppresses the listing entirely. Your inventory is "stranded" at FBA, can't sell.

**Fix:** monitor listing health. If suppressed, file removal order before LTSF hits.

## Pro estimation tools

Beyond manual math:

### Third-party PL-research tools
- "Sales estimator" tools that estimate monthly sales from BSR + category
- Less accurate post-2024 due to algorithm shifts
- Good as sanity-check vs your manual math

### SellerAmp's profit calculator
- Includes velocity estimate inline with ROI
- Good integrated view

### Keepa Product Finder
- For batch-scoring 100+ ASINs at once
- Pull stats from API, run scoring formula across all
- See [KPF page](../tools/keepa-product-finder.md)

## The estimation discipline

After 200+ sourcing decisions, you'll estimate intuitively. The discipline early on:

1. **Always do the math before buying** — don't shortcut to "feels like a good deal"
2. **Write it down** — note your estimate next to the SKU in your records
3. **Compare to actuals** — 30 days later, look at actual sales vs your estimate
4. **Calibrate over time** — your estimates get better as you build pattern recognition

After ~50 estimates, you'll know your typical bias (over-estimator vs under-estimator) and adjust.

***

Next: [Seasonal vs evergreen ASINs →](seasonality.md)

*Last updated: 2026-05-05*
