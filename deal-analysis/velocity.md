# Reading sales velocity (BSR drops, sold counts)

🟡 **Intermediate.** Sales velocity = how fast a product sells. It's the difference between a 30%-ROI flip that prints money and a 100%-ROI flip that sits unsold for a year. Mastering velocity reading is the highest-leverage skill in arbitrage.

## What "velocity" actually means

Three different velocity signals:

### 1. BSR drops
Each downward green line in Keepa's middle chart = approximately one sale across the entire listing. Track 30-day or 90-day drop count.

### 2. Monthly sold (where shown)
Amazon's own estimate of monthly buyers, displayed on some listings as "X+ bought in past month" badges (50+, 100+, 500+, 1000+, 5000+).

### 3. Subcategory rank
Often the most useful signal. Top 5% of subcategory = strong velocity, regardless of overall BSR.

## The velocity tiers

By 30-day BSR drops:

| Drops/30 days | Interpretation | Per-seller velocity |
|---|---|---|
| 0–5 | Slow seller | <1 sale/mo for you (skip unless ROI massive) |
| 6–15 | Modest velocity | 1–3 sales/mo if 3 sellers |
| 16–50 | Strong velocity | 3–10 sales/mo if 5 sellers |
| 50–150 | Hot seller | 10–30 sales/mo if 5–10 sellers |
| 150+ | Top tier | Constant motion |

## Per-seller share calculation

When you see velocity, divide by competition to estimate YOUR share:

```
Your monthly sales ≈ (Total monthly drops × Buy Box %) / (FBA seller count + 1)
```

Example: 60 drops/month, 4 FBA sellers besides you, ~85% Buy Box won by FBA:
```
Your sales ≈ (60 × 0.85) / 5 = ~10 units/month
```

Multiply by per-unit profit. If profit is \$5/unit, that's \$50/month from this listing.

Now ask: is \$50/month worth tying up capital + storage on this SKU?

## When BSR is suppressed

Sometimes BSR doesn't show — common with new listings (<90 days) and listings in deep stockout periods.

When BSR is missing:
- ❌ **Don't assume "no sales"** — see [reading velocity without BSR](../tools/keepa.md#reading-velocity-without-a-bsr)
- ✅ Check **subcategory rank** instead
- ✅ Check **monthly sold** badge
- ✅ Check **offer count drops** in Keepa
- ✅ Check **review velocity** (only useful for in-stock products, not OOS)

## The "Bought in past month" badge

Amazon shows this on listings with significant purchase volume:
- `50+ bought in past month`
- `100+ bought in past month`
- `500+ bought in past month`
- `1K+ bought in past month`
- `5K+ bought in past month`

This is Amazon's own data (not estimated). When you see it, you know there's real demand.

If a listing shows "1K+ bought" but BSR seems low, **trust the badge over the BSR**. The BSR algorithm sometimes lags or miscalibrates; the badge is direct transaction data.

## Subcategory rank — the underused signal

Top-level BSR can be misleading. A toy ranked #45,000 in Toys & Games sounds slow.

But check subcategory:
- "Building Toys" subcategory: rank #350
- "LEGO Sets" sub-sub-category: rank #45

Now you know it's actually a top performer in its specific niche — even though the top-level rank looks unremarkable.

**Always click into subcategories** before judging velocity.

## Velocity vs price stability

Two listings can have identical velocity but different stability:

### Stable velocity
- 60 drops/month for 6 months running
- Buy Box trends upward or flat
- Supply consistent

This is the dream — predict revenue, plan inventory.

### Volatile velocity
- 200 drops in March, 5 drops in April, 80 drops in May
- Buy Box swings 30%+
- Supply / demand shocks repeatedly

Volatile = harder to predict but sometimes more profitable in spikes.

For replens, prioritize stable. For one-time A2A buys, volatile is fine if you catch the right moment.

## The Keepa BSR drops counter

In Keepa's right panel "Data" tab:
- 30-day BSR drops: most actionable
- 90-day BSR drops: confirms 30-day is real (not a flash)
- 180-day BSR drops: long-term picture
- 365-day BSR drops: full year (helps spot seasonal)

For most decisions: 30-day drops > 6 = decent enough to consider.

## Seasonal adjustment

A toy that shows 0 drops in July but 200 drops in November isn't dead — it's seasonal.

Always check the 12-month chart for:
- Holiday spikes (Q4 toys, Christmas decor)
- Back-to-school (August–September: school supplies, dorm items)
- Summer (June–August: outdoor, beach, summer apparel)
- Spring (March–May: gardening, allergy products)

If the SKU shows a seasonal pattern, ask yourself:
- Is the next spike soon enough to justify storage?
- Can you sell through before peak storage costs hit?

Q4 storage premium (Oct–Dec) is **3× off-peak rates.** Buying summer items in March and storing for November may cost more in storage than the profit upside.

## Velocity confidence over time

The longer the velocity has been consistent, the more you can trust future projections.

| Track record | Confidence |
|---|---|
| 1 week of data | Very low — could be a flash |
| 1 month | Low — still might be promotional |
| 3 months | Medium — early replenishability signal |
| 6 months | Good — stable enough to plan inventory |
| 12+ months | High — trustworthy for replens |

For RA / OA buys: even 1-month confidence is okay if other signals (Buy Box stability, low offer count) align.

For wholesale: demand 6+ months of consistent velocity before signing a wholesale agreement. Anything shorter is too risky.

## Velocity decay signals

When a previously hot SKU starts decaying, look for:

### Signal 1: BSR climbing
30-day average BSR > 90-day average = velocity slowing.

### Signal 2: Buy Box sliding
Steady downward trend in Buy Box price = sellers cutting prices to clear inventory = supply > demand.

### Signal 3: Offer count rising
More sellers piling in faster than demand grows = future tank.

### Signal 4: Review velocity slowing
Reviews per week declining = fewer purchases = decaying velocity (only useful for in-stock products).

### Signal 5: Stockouts becoming rare
If a SKU never goes OOS anymore, supply has caught up with demand → margins erode.

When you see 2+ of these signals on a replen: stop reordering. Sell through inventory and move on.

## Velocity acceleration signals

The opposite — when a SKU is heating up:

- BSR average drops (30-day < 90-day < 180-day)
- Buy Box trends upward (often signaling supply constraint)
- Offer count drops (sellers can't replenish)
- Reviews accelerate (more sales)
- Amazon stockouts increase (demand outpacing supply)

When you see 2+ accelerators: lean in. This is the early signal of a Restock/Monitor opportunity. Set up a Tempo monitor before everyone else notices.

## Velocity per-seller misconception

Many beginners assume "high BSR = high profit for me." Reality: high BSR = high competition.

A listing at BSR #500 with 30 FBA sellers means:
- Total monthly sales: huge
- Your share if you enter: tiny (1/31 of total)
- Per-seller profit might be lower than a BSR #15,000 listing with 2 sellers

**Always think per-seller share, not total velocity.**

## Velocity by Amazon presence

Amazon's "presence" on a listing changes velocity dynamics:

### Amazon currently selling
- Amazon usually wins Buy Box
- Your share: <10%
- Effectively, you don't sell

### Amazon out of stock 1–30 days
- 3P sellers absorb demand
- Your share: depends on FBA count
- Buy Box price often elevated 10–30%

### Amazon out 30+ days
- Pent-up demand visible in 3P pricing
- Your share: largest if you enter early
- Restock event = volatile (Amazon comes back, kills 3P prices)

### Amazon never been on listing
- 3P market has set its own equilibrium
- More predictable for replenishability
- Often the best replen opportunities

## Real-world velocity scenarios

### Scenario 1: New listing, BSR 50,000, 1 seller
- Brand new launch
- Don't trust the velocity number — it's volatile
- Could be a sleeper hit OR a dud
- Skip until 3+ months of history

### Scenario 2: Established listing, BSR 5,000, 8 FBA sellers
- 30-day drops: 100
- Per-seller share: ~12 units/mo
- High velocity, moderate competition
- If profit/unit is \$3: \$36/month from this SKU
- Worth it if scaled across 50 SKUs

### Scenario 3: Niche listing, BSR 80,000, 2 sellers
- 30-day drops: 8
- Per-seller share: ~3 units/mo
- Low velocity but you own most of it
- If profit/unit is \$15: \$45/month
- Better per-effort than scenario 2

### Scenario 4: Hot listing, BSR 100, 40 FBA sellers
- 30-day drops: 5,000+
- Per-seller share: ~125 units/mo
- High velocity but cutthroat competition
- Margins likely thin (30+ sellers race-to-bottom)
- Often less profitable than Scenario 3

The lesson: **niche dominance > popular saturation.**

## Velocity in your sourcing decision

Combine velocity with other factors:

```
Score = (Per-seller monthly velocity × Profit per unit)
        × Confidence factor (0–1 based on track record)
        / Capital tied up (your buy cost × buy quantity)
        × Risk adjustment (lower if Brand Registered or volatile)
```

Higher score = better source.

After 100+ flips, you'll do this math intuitively in 10 seconds per scan.

***

Next: [Competition: FBA, FBM, Amazon-on-listing →](competition.md)

*Last updated: 2026-05-05*
