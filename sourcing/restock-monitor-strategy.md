# Restock/Monitor — availability scarcity plays

🔴 **Advanced.** The second of the two foundational BoxedUp sourcing strategies. Identify items where Amazon is OOS and demand is real, monitor for restocks, catch supply when it appears, and sell into elevated 3P pricing.

## What it is

You identify items that Amazon has **historically stocked** but is currently **out of stock on**, then set up monitors to catch the moment Amazon (or any retailer carrying the item) restocks. You buy inventory the second it appears and sell at:

1. **The elevated 3P market price** (because while Amazon was OOS, third-party sellers ran the price up), or
2. **Amazon's price** if their algorithm randomly drops back to historical retail when they restock

Either way, you profit because demand exceeds supply and you have the infrastructure in place to catch inventory the moment it appears.

## The core logic

This is an **availability play**, not a pricing play. You're not exploiting a price dip — you're exploiting the fact that an item is **hard to get** while demand remains high or is growing.

The bet is one of two things:
1. Amazon will restock at historical retail pricing → you buy and sell at the elevated 3P market price
2. Amazon will restock at the current elevated price → you watch for random algorithm drops back to historical retail and catch those

Either way, profit comes from being the rare seller with inventory when buyers are queued up.

## The non-negotiable: historical orange

For an item to qualify as a Restock/Monitor candidate, the Keepa chart MUST show orange (Amazon in stock) at some point in its history. **Not optional.** Without historical orange:

- You can't confirm Amazon has ever carried this item
- You can't know if Amazon's supply-chain relationship is established
- You can't know if Amazon will ever restock

More white than orange is fine. Even a tiny sliver of orange months ago qualifies. The point: prove Amazon has had a supplier relationship with this product.

## The 4-phase ideal chart

A textbook Restock/Monitor candidate's chart tells this 4-phase story over a year:

### Phase 1 — Healthy period
- Long stretch of orange shading at a stable, predictable price
- Amazon and 3P prices tracking closely together
- Offer count building steadily (sellers finding the product)
- Item clearly selling (BSR drops visible, or Monthly Sold data active)

### Phase 2 — The supply signal
- Offer count begins a sustained, **one-directional decline**
- No bouncebacks — sellers are selling through and cannot replenish
- Orange shading starts showing gaps (Amazon going in and out)
- 3P prices start to separate from Amazon's price (the spread grows)

### Phase 3 — The collapse
- Orange disappears entirely (Amazon goes OOS)
- Offer count reaches near-zero
- 3P prices spike 2×, 3×, 4×+ above historical Amazon retail
- Sales rank may disappear (BSR suppressed)

### Phase 4 — The monitor phase (where you live)
- Occasional **tiny orange slivers** → instant OOS again
- These slivers are the most valuable data: they confirm **active demand absorption**
- 3P market maintains elevated pricing because no real supply exists
- Your monitors are live waiting for the next restock event

The full chart-reading framework: [Reading a Keepa chart like a pro](../tools/keepa.md).

## The tiny orange sliver — the highest-conviction signal

When you see a Keepa chart with months of white (Amazon OOS) and a tiny sliver of orange appears — immediately going OOS again — **that is one of the highest-conviction demand signals in the methodology.**

Why:
- Amazon restocked (however briefly)
- That restock sold out **instantly** at whatever price Amazon set
- This confirms demand exists right now, in the current market, at current prices
- If you'd had inventory at that moment as 3P, you would have sold it

The fact that there was no time for review growth, no BSR impact, and no offer-count recovery does not matter. The data is telling you: **buyers are waiting. The second supply appears, it gets absorbed.**

## How to surface Restock candidates — KPF

Restock candidates come from Keepa Product Finder (KPF). The full filter set, with reasoning for every filter, lives here: [KPF Restock filter set](../tools/keepa-product-finder.md#the-restock-filter-set--filter-by-filter).

The non-negotiable filters:

| Filter | Value | Why |
|---|---|---|
| Historical Sales Rank Month | A specific past month | Proof item was actively selling pre-shortage |
| Current Sales Rank | `-1` (no rank) | Rank suppressed = deep OOS pattern |
| Current AMAZON | `-1` (OOS) | Amazon currently out |
| AMAZON OOS % 90-day | **5% – 99%** | Amazon stocked AT LEAST sometimes |
| AMAZON OOS Count 90-day | **≥ 2** | Confirms restock pattern, not a one-off |
| Sort | SALES_RANK ASC, monthlySold DESC | Best historical demand first |

Then you triage with the [restock-frequency scoring model](../tools/keepa-product-finder.md#a-working-restock-frequency-scoring-model).

## The end-to-end Restock workflow

### 1. Run the KPF query
Weekly, in your primary categories. See [KPF deep dive](../tools/keepa-product-finder.md).

### 2. Triage with the scoring model
Take the top 20–50 by score.

### 3. Verify each chart (Year view)
Confirm 4-phase pattern, look for tiny-orange-sliver evidence, near-zero offer count, elevated 3P pricing.

### 4. Set up monitors
Tempo, Blaze, or both. See [Restock monitoring infrastructure](restock-monitoring.md) for command syntax and workflow.

### 5. Wait
Monitors run 24/7. When a restock fires, you get pinged in Discord with the buy URL.

### 6. Buy fast
Click within seconds. Buy the maximum quantity Amazon allows. Box packaging, not retail. Save the invoice.

### 7. Ship into FBA same-day if possible
Speed matters. Each day your inventory isn't live, the elevated 3P price is at risk of collapsing.

### 8. List at elevated 3P pricing
Match or undercut by 5–10% depending on whether you want max margin or fast clearance.

### 9. Sell through and watch the chart
If Amazon comes back consistently in stock, the elevated price will collapse. Clear out before that happens.

## Sub-strategy: Price Drop Monitors

Even on items where Amazon's current retail is inflated (e.g., a part that went from \$100 to \$400), Amazon's pricing algorithm will occasionally:
- Randomly drop the price back to historical retail
- Sometimes for minutes, sometimes hours
- The item sells out immediately at the old price
- The algorithm corrects and the price spikes back up

This creates a sub-strategy: **Price Drop Monitors** for items where Amazon IS in stock but at inflated pricing. You watch for the algorithm to randomly reset to historical retail.

Different from standard Restock Monitors (where Amazon is fully OOS) but the monitoring infrastructure is the same. Tempo / Blaze / commercial monitor services all support both.

## Category-level pattern recognition

The most powerful application of this strategy isn't catching individual restocks — it's recognizing **category-level supply events** while they're forming.

The pattern: **a sustained, one-directional decline in offer count across multiple SKUs in the same subcategory simultaneously.**

When many different products in the same category all show this decline at the same time with no bouncebacks, that rules out product-specific explanations. The cause must be upstream — at the supply chain level. **This is how the [DDR4/DDR5 RAM shortage was identified weeks before it became public knowledge](../tools/the-ram-shortage-case-study.md).**

The teachable framework:
1. Run KPF Restock queries on a regular cadence
2. When you see a pattern, ask: *"Is this one product or a category?"*
3. If it's a category, the cause is upstream
4. Confirm via external research
5. Act before the market catches up

## Restock vs A2A — quick reference

| | Restock/Monitor | A2A |
|---|---|---|
| Surface | KPF + Tempo/Blaze monitors | Keepa Deals |
| Trigger | Sustained OOS pattern with restock evidence | 30–60% price drop event |
| Amazon status | OOS, occasionally restocking | In stock |
| Buy from | Wherever supply appears | Amazon itself |
| Sell on | Amazon | Amazon |
| Hold time | 1–8 weeks | 2–4 weeks |
| Cadence | Set up monitors, wait days-to-weeks | Real-time, hours-to-days |

## When Restock plays fail

- **No historical orange.** You skipped the chart-verification step. Amazon never stocked it. There's no restock to wait for.
- **The shortage is over.** Amazon has been steadily back in stock for 30+ days. The 3P premium has collapsed. **Prune the monitor.**
- **Saturation.** Too many resellers are monitoring the same SKU. Restocks get vacuumed instantly by everyone simultaneously and your win rate per ping drops to zero. Move on.
- **You weren't fast enough.** Manual reaction can't compete with monitor bots. **Let the bots ping you, then react in seconds.**
- **Amazon's quantity limit was 1.** You bought 1 unit and the unit margin doesn't cover the time spent. Some restocks don't have enough scale to be worth your monitor slot. Drop them.
- **The category has been published.** Once a shortage is on CNBC, the margin is gone. The methodology works *before* the news, not after.

## What "good monitor list" looks like

A healthy restock monitor list:

- **20–80 ASINs** at any given time
- **Mix of price points** — some \$50–\$100 for volume, some \$200–\$500 for ticket
- **Mix of restock frequencies** — some "hot" SKUs that fire weekly, some "deep" SKUs that fire once a month with bigger margins
- **All in categories you can actually move** — no monitors on gated categories you can't list in
- **Pruned weekly** — dead monitors come off, fresh candidates take their place

Don't be sentimental. The monitor list is a working tool, not a wishlist.

***

Next: [Restock monitoring — Tempo, Blaze, and the infrastructure layer →](restock-monitoring.md)

*Last updated: 2026-05-05*
