# IPI score deep dive

🟡 **Intermediate.** IPI (Inventory Performance Index) is Amazon's score of how well you manage FBA inventory. It controls your **storage limits** — a low IPI caps how much inventory you can keep at FBA, which caps your scale.

## What IPI is

Amazon scores you 0–1000 on four sub-metrics:

| Sub-metric | What it measures | Weight |
|---|---|---|
| **Excess inventory** | % of stock that's older / overstock | High |
| **Sell-through rate** | Units sold ÷ avg inventory over 90 days | High |
| **Stranded inventory** | % of inventory unsellable (listing issue) | Medium |
| **In-stock rate** | % of time your top SKUs are in stock | Medium |

A weighted blend gives your IPI score, recalculated every Monday.

## The score thresholds

| IPI | Status | Restock limit |
|---|---|---|
| 0–399 | 🔴 At risk of restock cap | Cap (Amazon decides) |
| 400–499 | 🟡 Warning zone | Cap (lower than 500+) |
| **500+** | 🟢 **Good standing** | No cap |
| 700+ | 🟢 Excellent | No cap, faster receiving |

**The magic number is 500.** Below 500, Amazon caps how many units you can have in FBA. Cap is based on category-volume forecasts and your account history. Hit it and you can't ship in more inventory — even if you have buyers waiting.

> **The cap moves quarterly.** Even if you're under the cap today, you might wake up Monday and find Amazon raised your storage commitment. Plan inventory levels with 20% headroom.

## Why IPI tanks

The four most common patterns:

### 1. Slow-moving long tail
You sourced a "great deal" 6 months ago at 50% off. It moves 1 unit/week. The other 49 units sit. Amazon flags as **excess inventory** → IPI drops.

### 2. Hot SKU stockouts
Your replen winner is out of stock for 30+ days. **In-stock rate** sub-metric drops → IPI drops. Even if your other inventory sells fast, missing top SKU drags the score.

### 3. Stranded units
You changed a listing, deleted a SKU, or had a listing suppressed. Inventory in FBA is "stranded" — can't sell because the listing is broken. This is a silent IPI killer.

### 4. Q4 hangover
You shipped tons of inventory in October for Christmas. Most sold. The leftover tail sits at FBA in January, racking up storage and counting as excess.

## How to fix a low IPI

The 4-week recovery plan:

### Week 1: Audit stranded inventory
- Inventory → Manage Inventory → filter "Stranded"
- For each stranded item: find the cause (deleted listing, suppressed listing, image issue, hazmat flag)
- Either fix the listing or submit a removal order
- This is the **single fastest IPI lift** — sometimes +50 points overnight

### Week 2: Liquidate excess
- Filter "Excess Inventory" in the IPI dashboard
- For SKUs with 270+ days of supply at current sales velocity:
  - **Drop price aggressively** to clear (sometimes below your cost — accept the loss)
  - Or submit a **removal order** (return to you)
  - Or a **disposal order** (Amazon destroys; cheaper than return)
- The trade-off: short-term cash hit for IPI rescue. Worth it.

### Week 3: Fix stockouts
- Reorder your top 10 SKUs aggressively — get them back in stock
- For replens, set up auto-reorder logic

### Week 4: Don't ship junk
- Stop sending in slow-velocity SKUs
- For new sourcing: only ship SKUs where you can sell within 60 days at current velocity

## The "70% of new inventory must be a winner" rule

A pattern from BoxedUp members who maintain 700+ IPI:

> **Of every 100 units you ship in, at least 70 must be SKUs you've already proven sell ≥ 4/month at current price.**

The other 30 can be experiments — new sourcing tests, longshot replens, seasonal plays. Keep that ratio and IPI stays healthy. Flip it (70% experiments) and you'll get capped within a quarter.

## Storage cap mechanics

When IPI is below 500, Amazon assigns a "Storage volume" cap (in cubic feet) for your account:
- Calculated from your trailing-12-month sales volume
- Adjusted by category mix
- Re-evaluated each Monday

You can see your cap in: Inventory → Inventory Performance → "Capacity Manager."

**You can't beg or appeal it lower.** You can only:
1. Get your IPI to 500+ (cap removed entirely)
2. Reduce inventory volume below the cap (so you can ship more in)
3. Apply for a category-specific increase if you have evidence (rarely granted)

## Q4 strategy

Q4 (Oct–Dec) is when IPI rules are most punishing — you're shipping in 3× normal volume but Amazon's cap doesn't auto-adjust. Plan ahead:

| Date | Action |
|---|---|
| **Sept 1–15** | IPI cleanup — submit removals for slow movers; aim for 600+ score |
| **Oct 1** | Ship in Q4 inventory; bake in 20% headroom under cap |
| **Oct 15** | Last shipping plan that's likely to receive before Black Friday |
| **Nov 15** | Last shipping plan for guaranteed Christmas-week receiving |
| **Dec 1** | Stop shipping; manage what's already at FBA |
| **Dec 26** | Plan post-Christmas removals if needed |
| **Jan 15** | Post-holiday IPI cleanup |

## Disposal vs removal vs liquidation

When your IPI is hurting from excess inventory:

| Option | Cost per unit | When to use |
|---|---|---|
| **Removal** | ~\$0.97 (small) → \$3.50 (oversize) | Inventory worth recovering; you have storage at home |
| **Disposal** | ~\$0.30–\$0.85 | Inventory not worth shipping back (cheap items, damaged) |
| **Amazon Liquidation** | Amazon takes ~85%+ off retail; you get ~15% | Bulk-rid; lazy but cheapest |
| **Aggressive price drop on listing** | Free | If you can move it via price; preserves listing rank |

**Disposal is cheapest IPI-rescue tool.** Beginners hate the idea of "wasting" inventory, but if it's a \$5 cost item that's eating IPI and storage fees → disposal saves you money.

## What good IPI looks like in practice

Members with 750+ IPI tend to share these habits:

- **<60 day average inventory age** across the catalog
- **Top 10 SKUs in stock** 95%+ of the time
- **Zero stranded inventory** (audited weekly)
- **Aggressive disposal** — they don't tolerate units sitting >180 days
- **Clear sourcing discipline** — they don't ship in losers just to "see what happens"

It's not magic. It's discipline applied weekly.

***

Next: [Storage fees, aged inventory, removals →](fees-and-removals.md)

*Last updated: 2026-05-05*
