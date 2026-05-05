# The RAM shortage — a worked case study

🔴 **Advanced.** This is the canonical worked example of the BoxedUp methodology — the DDR4/DDR5 RAM shortage of late 2024 / early 2025, **spotted from Keepa data alone, weeks before it became public knowledge.**

It shows every part of the methodology working together: data discovery → category-level pattern recognition → external research as confirmation → action.

## The setup

The play started during routine KPF browsing — running standard restock/monitor queries in the Computer Memory category. Nothing exotic, nothing pre-planned. Just the same query template you'd run any week, against rootCategory `172282` (Electronics) → category `172500` (Computer Memory).

This is important: **the discovery happened during normal work.** It wasn't because anyone was hunting for a shortage. The data surfaced the signal during routine pattern recognition.

## Step 1 — Normal KPF browsing

Standard Restock/Monitor filters running against Computer Memory:

```json
{
  "title": "-axiom -patriot",
  "current_SALES_gte": -1,
  "current_SALES_lte": -1,
  "current_AMAZON_gte": -1,
  "current_AMAZON_lte": -1,
  "rootCategory": ["172282"],
  "categories_include": ["172500"],
  "outOfStockPercentage90_gte": 5,
  "outOfStockCountAmazon90_gte": 2,
  "sort": [["current_SALES","asc"],["monthlySold","desc"]],
  "page": 0,
  "perPage": 100
}
```

In English: "Computer Memory items where current rank is suppressed AND Amazon is currently OOS AND Amazon was OOS at least 5% of the last 90 days AND went OOS at least 2 times. Excluding Axiom and Patriot. Sorted by best historical rank with monthly sold as tiebreaker."

This was a routine, well-tuned query — see the [filter-by-filter reasoning](keepa-product-finder.md#the-restock-filter-set--filter-by-filter).

## Step 2 — The pattern across multiple SKUs

Browsing the results, the same pattern was visible **across multiple RAM SKUs simultaneously**:

- Offer counts declining from 30–40 sellers → near zero over 60–90 days
- Amazon orange shading starting to show gaps (Amazon going in and out more frequently)
- 3P prices beginning to separate from Amazon's price (spread growing)
- Some SKUs: offer count had already reached near-zero with price already climbing

This was not one product having a problem. It was **the entire category showing the same signal at the same time.**

## Step 3 — The key insight: category-level, not product-level

A single SKU with a declining offer count could mean many things:
- Brand-specific issue
- Listing problem
- IP complaint
- Product discontinuation

But when **many different SKUs in the same subcategory all show the same decline simultaneously**, that **rules out product-specific explanations.** The cause must be upstream — at the supply chain level.

This is the most important pattern-recognition rule in the methodology:

> **"Is this one product or a category?"**
>
> One product = product-specific issue (not actionable at scale)
> A category = supply chain event (highly actionable, often historic)

When you spot the second one, **you've found something the broader market hasn't seen yet.**

## Step 4 — External confirmation

After identifying the Keepa signal, the next step was to research **why.**

What turned up:
- UBS analyst reports warning of severe DRAM shortage in 2026
- Korean manufacturers (Samsung, SK Hynix, Micron) stopping quotes for certain die configurations
- Server DRAM prices rising 40–50% in spot markets
- DDR5 16Gb die prices jumping from \$7–8 to \$13 on spot markets
- Consumer DDR5 inventory at distributors already thinning

**The data discovered the opportunity. The research explained the why.**

This is the order. Always. Keepa first, news second. By the time it's news, the margin is gone.

## Step 5 — Action

The finding was shared with the BoxedUp Discord on October 30, 2025, with Keepa chart screenshots showing the exact signals:
- Offer-count decline arrows
- Amazon OOS gaps appearing in the orange line
- Price beginning to separate from Amazon's historical retail

Members who acted on this information **bought RAM at \$100–130 that subsequently went to \$400–500+.**

## The teachable framework

Distilled:

1. **Browse KPF with restock filters running on a regular basis** — the discovery has to happen while you're there, so be there
2. **When you see a pattern, ask:** *"Is this one product or a category?"*
3. **If it's a category — the cause is upstream** (supply chain event)
4. **Confirm via external research** (the why, not the what)
5. **Act before the market catches up**
6. **The data discovers. The research explains. Speed is the edge.**

## Top 15 picks from the same KPF run

For reference, this was the actual Top 15 list from a Keepa API + scoring-model run during the shortage. Shows what real data from this kind of query looks like:

| Rank | Item | OOS30 | OOS90 | Sold/Mo | FBA | FBM | Now | Avg365 | Why |
|---|---|---|---|---|---|---|---|---|---|
| 1 | CORSAIR Vengeance RGB PRO 32GB DDR4 3200 | **57** | 131 | 50 | 0 | 3 | \$281 | \$141 | Highest restock frequency in dataset |
| 2 | Crucial 16GB DDR5 Kit 5600MHz Desktop | **32** | 63 | 500 | 1 | 11 | \$266 | \$81 | Best demand + restock combo |
| 3 | CORSAIR Vengeance LPX 32GB DDR4 3600 | **23** | 111 | 100 | 0 | **1** | \$328 | \$156 | **1 FBM seller. Near monopoly.** |
| 4 | Crucial 16GB DDR5 Laptop Kit 5600MHz | **21** | 33 | 200 | 0 | 2 | \$295 | \$84 | Sells through nearly instantly |
| 5 | Crucial 32GB DDR5 Kit 5600MHz Desktop | **22** | 46 | 100 | 0 | 5 | \$448 | \$153 | High ticket + high frequency |
| 6 | Crucial Pro 32GB DDR5 6000MHz | 3 | 35 | **1000** | 2 | 25 | \$390 | n/a | #9 BSR. 1000 buyers/month. |
| 7 | Crucial 32GB DDR5 Kit 4800MHz | **18** | 42 | 100 | 0 | 2 | \$320 | \$130 | 2 FBM sellers only |
| 8 | Crucial 16GB DDR4 3200MHz SODIMM | confirmed | confirmed | 200 | 0 | 4 | \$147 | \$31 | Laptop DDR4 demand |
| 9 | Crucial 32GB DDR4 Kit 3200MHz | confirmed | confirmed | 200 | 0 | 4 | \$255 | \$63 | 4× price jump |
| 10 | G.SKILL Flare X5 32GB DDR5 6000MHz | confirmed | confirmed | 200 | 3 | 0 | \$420 | \$330 | Price stable, low competition |
| 11 | Crucial Pro 64GB DDR5 6400MHz | confirmed | confirmed | 100 | 0 | 4 | \$1000 | \$307 | High ticket, 3× price jump |
| 12 | Crucial Pro 64GB DDR5 6400MHz v2 | confirmed | confirmed | 100 | 0 | 2 | \$799 | \$342 | 2 FBM sellers only |
| 13 | G.SKILL Trident Z5 RGB 32GB DDR5 | confirmed | confirmed | 100 | 3 | 0 | \$480 | n/a | Premium G.SKILL, scarce |
| 14 | Crucial 8GB DDR4 3200MHz | confirmed | confirmed | 400 | 0 | 12 | \$80 | \$20 | 400 buyers/month, highest volume DDR4 |
| 15 | Kingston FURY Beast 16GB DDR4 3200 | confirmed | confirmed | 100 | 0 | **2** | \$130 | \$69 | **2 FBM sellers. Best monopoly play.** |

Notice the patterns:
- **OOS30 column** — items that went OOS 20+ times in 30 days = Amazon was restocking almost daily and selling through every time
- **FBA = 0** on most rows — when you catch a restock here, you own the listing
- **3–6× spreads** between current and historical price (Avg365)
- **Demand evidence everywhere** — Monthly Sold of 100–1000 even with rank suppressed

Item #1 — CORSAIR Vengeance RGB PRO 32GB — went OOS 57 times in 30 days. Amazon was restocking nearly twice per day and the market absorbed every restock instantly. That's the shape of a category in shortage.

## What you should take away

Three things:

1. **Routine work is what produces the big wins.** The shortage was found during a normal KPF browse, not a special hunt. Show up, do the reps, the patterns surface.

2. **Category-level pattern recognition is the highest-leverage skill in this business.** One SKU declining is noise. Twenty SKUs in the same subcategory declining together is a supply-chain event worth millions.

3. **The data confirms before the news.** By the time CNBC reports a shortage, the margin is gone. Your edge is in seeing the pattern in the offer-count decline arrows weeks before anyone writes about it.

***

Next: [Restock monitoring — Tempo, Blaze, and the infrastructure layer →](../sourcing/restock-monitoring.md)

*Last updated: 2026-05-05*
