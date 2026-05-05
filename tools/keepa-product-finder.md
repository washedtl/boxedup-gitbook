# Keepa Product Finder (KPF) — sourcing at scale

🔴 **Advanced.** KPF is where serious BoxedUp sourcers find leads at volume. It queries the entire Amazon catalog against ~1,360 typed filter dimensions — and once you can write KPF queries, your sourcing time-per-profitable-flip drops 5–10×.

> **The data discovers. News confirms. Speed is the edge.**
>
> The browser KPF is limited to visual inspection of one item at a time. The API lets you pull 100 ASINs in a single call, access raw numerical data (exact OOS counts, exact prices, exact timestamps), and build scoring models that rank thousands of items in seconds.

## The two queries that matter

The BoxedUp methodology runs on **two strategies**: A2A (price anomalies) and Restock/Monitor (availability scarcity). Each one has its own query template — and **never confuse the two.**

| | A2A — price anomaly | Restock/Monitor — scarcity |
|---|---|---|
| Surface | Keepa Deals (not KPF) | KPF |
| Trigger | Drop % + Drop Interval | Sustained OOS pattern with restock evidence |
| Purchase from | Amazon itself | Wherever supply appears |
| Cadence | Real-time deals feed | Daily/weekly KPF runs + monitor alerts |

This page covers both. The presets in detail: [The 2 KPF presets we actually use](kpf-presets.md). The infrastructure for catching restocks: [Restock monitoring](../sourcing/restock-monitoring.md).

## What KPF actually is

Officially: "Keepa Product Finder."

Practically: a SQL-like query interface on top of Keepa's complete database. You write a filter and Keepa returns every ASIN that matches.

Live at **`keepa.com/#!finder/`**. Requires the paid Keepa subscription (\$19/mo) — without paid you're capped at trivial filters.

## Why it changes the game

| Manual sourcing | KPF sourcing |
|---|---|
| Walk into a Walmart, scan 200 items, find 3 buys | Run one KPF query, get 500 ASINs that already match your criteria |
| Limited to what's on the shelf nearby | Limited to whatever exists on Amazon |
| Replens are accidents you stumble onto | Replens are query results you systematically extract |
| Single product at a time | Pattern recognition across hundreds of SKUs simultaneously |

The catch: **KPF tells you Amazon is undersupplied or mispriced.** It doesn't tell you where to source from. That's [reverse sourcing](reverse-sourcing-method.md) and [restock monitors](../sourcing/restock-monitoring.md).

## The Restock filter set — filter by filter

This is the canonical Restock/Monitor query, with reasoning for every filter. Each one is non-negotiable for a reason.

### Filter: Historical Sales Rank Month (e.g. `202509` = September 2025)

**What it does:** Only returns items that had an active, recorded sales rank in that specific month.

**Why this filter matters:** This is the **proof-of-past-sales filter.** It confirms the item was actively selling before the shortage hit. Without it, the search surfaces items that were never selling to begin with — dead listings that happen to be OOS because they were always slow movers.

**The logic:** if it was selling in September, and it's OOS now, and Amazon used to stock it → that's a real opportunity. If it was never selling in September, OOS now just means it was always nobody-wanted-it.

Set this to a month *before* whatever shortage you're investigating intensified.

### Filter: No Sales Rank (`SALES_outOfStock = true` / `current_SALES = -1`)

**What it does:** Returns items where the current sales rank is suppressed/absent.

**Common misconception:** This does NOT mean the item has no sellers or doesn't sell. It means the item has been comprehensively out of stock across enough sellers that Amazon's ranking algorithm has insufficient current sales data to generate a rank.

**Why pair it with the historical rank filter:** "had an active rank in September" + "no rank right now" = the item was selling before, and the rank disappeared because it went so comprehensively OOS that even the rank tracking went dark. **This is a deep supply-vacuum signal, not a dead-item signal.**

For reading velocity without a rank, see [the 5-signal framework on the chart-reading page](keepa.md#reading-velocity-without-a-bsr).

### Filter: Amazon OOS checkbox (`current_AMAZON = -1`)

**What it does:** Only returns items where Amazon is currently out of stock.

**Why:** Core filter for restock plays. You only want items where Amazon is actually OOS right now. If Amazon is in stock, it's a different play (price drop monitor or A2A). Every result needs to be monitored for a restock event.

### Filter: Amazon OOS % 90-day — range **5% to 99%**

**What it does:** Filters by the percentage of the last 90 days that Amazon was out of stock.

**Why NOT 100%:** Critical insight. If Amazon has been 100% OOS for the entire 90 days with no activity, it might mean Keepa **never captured an Amazon offer at all** — the item was never on Amazon's radar. The 99% cap ensures results include items where Amazon was in stock *some* of the time in the last 90 days. That "some of the time" = proven restock pattern. Keepa saw Amazon come back.

**Why a minimum of 5%:** Ensures Amazon has actually been OOS at some point. 0% OOS = continuously in stock = not what you're looking for.

**Sweet spot: 20–80% OOS over 90 days** — Amazon is actively trying to supply but keeps selling through. Clearest restock pattern.

### Filter: Amazon OOS Count (90-day ≥ **2**)

**What it does:** Only returns items where Amazon went out of stock at least 2 times in the last 90 days.

**Why ≥ 2:** One OOS event could be a fluke, listing error, or one-time supply issue. **Two or more confirms a pattern.** Amazon is stocking → selling through → going OOS → restocking → selling through again. That's a live restock cycle — exactly what your monitor wants.

**The higher the count, the better:** an item that went OOS 20+ times in 30 days = Amazon is restocking almost daily and selling through every time. Extreme demand and extreme restock frequency.

### Filter: Title Exclusions (e.g. `-axiom -patriot`)

**What it does:** Excludes any item with those words in the title.

**Why:** Some brands have distribution channels that don't follow consumer restock dynamics. In Computer Memory, Axiom serves enterprise/business customers (bulk IT sales, different pricing); Patriot has lower retail market presence and different distribution channels. Their OOS patterns don't match the thesis. **Including them contaminates the results.**

The principle generalizes: **brand exclusions clean up results by removing items whose market behavior doesn't fit the strategy.** Add other exclusions as you identify brands that consistently produce false signals in your category.

### Sort: Sales Rank ASC, Monthly Sold DESC

**What it does:** Best (lowest = most popular) historical rank first, ties broken by monthly sold volume.

**Why this order:** You want highest-demand items at the top. If two items both have OOS patterns that qualify, the one with better historical rank and higher monthly sold is the more valuable opportunity — more buyers waiting, more velocity when supply appears, more profit potential.

## A worked Restock query (Computer Memory)

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
  "productType": [0,1,2],
  "page": 0,
  "perPage": 100
}
```

In English: "Computer Memory items where current sales rank is suppressed AND Amazon is currently OOS AND Amazon was OOS at least 5% of the last 90 days AND went OOS at least 2 times. Excluding Axiom and Patriot brands. Sorted by best historical rank with monthly sold as tiebreaker."

This typically returns the highest-conviction restock candidates in the category.

## The KPF schema — what you can filter on

Keepa exposes ~1,360 typed fields. They cluster into 9 families:

### 1. Categories
- Root category (Toys & Games, Beauty, Home, Electronics, etc.)
- Sub-categories (multi-select)
- Multi-include AND multi-exclude

### 2. Filter rows (the bulk of the schema)
For each of ~30 series (BUY_BOX, AMAZON, NEW, USED, SALES_RANK, OFFER_COUNT, REVIEW_COUNT, RATING, NEW_FBA, NEW_FBM, etc.), you can filter on:

- `current_X` — today's value
- `avg30_X` / `avg90_X` / `avg180_X` — rolling averages
- `min_X` / `max_X` — historical extremes
- `gte` / `lte` — bound the value (≥ this, ≤ this)

That's ~600 numeric fields just from this section.

### 3. Out-of-stock filters (the gold mine)
- `outOfStockPercentage90` (Amazon OOS % over 90 days)
- `outOfStockCountAmazon90` (number of times Amazon went OOS in 90 days)
- `current_AMAZON = -1` (Amazon currently OOS)
- `current_SALES = -1` (sales rank suppressed)

### 4. Back-in-stock toggles
28 series with "did this come back in stock recently?" booleans (Amazon back in 7d / 30d / 90d, same for FBA/FBM/Used).

### 5. Categorical filters
- `brand[]` IN list / NOT-IN list
- `manufacturer[]`
- `dealType` (Lightning Deal, Coupon, etc.)
- `availabilityAmazon`
- `hasReviews` / `hasParentASIN` / `isAdultProduct` / `coupons`
- `historicalParentASIN`, `title` keyword search

### 6. Sort
Any of the above, ascending or descending. Most useful: SALES_RANK ascending (lowest = fastest movers).

### 7. Pagination
Up to 10,000 results per query if you have enough Keepa tokens.

## Common Keepa category IDs

| ID | Category |
|---|---|
| 172282 | Electronics (root) |
| 172500 | Computer Memory |
| 1254762011 | Desktop Memory |
| 1292116011 | Laptop Memory |
| 3015429011 | Internal SSDs |
| 595048 | Hard Drives |
| 165793011 | Video Games |
| 468642 | Software |

For other categories, browse keepa.com/#!finder/ in the UI — it surfaces every category and ID.

## How tokens work

KPF queries are **token-priced.** Each query consumes Keepa tokens based on:

- Query depth (more filters = more tokens)
- Result page count (paging through 10,000 results burns through fast)
- How "expensive" individual filters are

The paid plan gives **300 tokens/hour** that refill continuously. A typical KPF query costs 5–25 tokens. Heavy queries 100+.

**Practical rule:** save your good queries. Don't keep tweaking and re-running the same one — refine, save, run once.

## The Keepa API — programmatic access

The browser KPF is for visual inspection. The API is for scale.

```javascript
var xhr = new XMLHttpRequest();
xhr.open('POST', 'https://api.keepa.com/query?key=YOUR_KEY&domain=1', false);
xhr.setRequestHeader('Content-Type', 'application/json');
xhr.send(JSON.stringify(YOUR_QUERY));
var data = JSON.parse(xhr.responseText);
```

**Domain values:** `1`=US, `2`=UK, `3`=DE, `4`=FR, `5`=JP, etc.

### Pulling product data after getting an ASIN list

```javascript
var xhr2 = new XMLHttpRequest();
xhr2.open('GET', 'https://api.keepa.com/product?key=KEY&domain=1&asin=' + asins.join(',') + '&stats=90', false);
xhr2.send();
var pData = JSON.parse(xhr2.responseText);
```

### Key fields in the product response

```
product.asin                              → ASIN
product.title                             → Product title
product.monthlySold                       → Estimated monthly buyers
product.stats.outOfStockCountAmazon30     → # times Amazon went OOS in 30 days
product.stats.outOfStockCountAmazon90     → # times Amazon went OOS in 90 days
product.stats.outOfStockPercentage30      → Array; [1] = Amazon % OOS in 30d
product.stats.outOfStockPercentage90      → Array; [1] = Amazon % OOS in 90d
product.stats.avg30                       → Array; [1] = Amazon avg price 30d (÷100 for $)
product.stats.avg90                       → Array; [1] = Amazon avg price 90d
product.stats.avg180                      → Array; [1] = Amazon avg price 180d
product.stats.avg365                      → Array; [1] = Amazon avg price 365d
product.stats.offerCountFBA               → Current FBA seller count
product.stats.offerCountFBM               → Current FBM seller count
product.csv[1]                            → Amazon price history array
```

**Price-type index key:** 0=BuyBox, 1=Amazon, 2=New, 3=Used, 4=NewFBA, 5=NewFBM

**Price encoding:** All prices stored as integers × 100. A stored value of 9999 = \$99.99. Value of `-1` = OOS.

## A working restock-frequency scoring model

Once you've pulled product data via the API, score each ASIN to rank opportunities:

```javascript
score = (oosCount30 × 20)                   // primary: recent restock events
      + (oosCount90 × 4)                    // secondary: confirmed pattern
      + (oosPct30 between 1-99 ? 30 : 0)    // in and out = actively restocking
      + (oosPct30 < 50 ? 20 : 0)            // mostly in stock = restocking fast
      + Math.min(monthlySold, 500) / 5      // demand signal (capped)
      + (totalOffers ≤ 5 ? 15 : 0)          // low-competition bonus
      + (totalOffers ≤ 2 ? 15 : 0)          // near-monopoly bonus
```

What this rewards:
- **Frequent recent restocks** are weighted heaviest (oosCount30 × 20) — these are the live, active opportunities
- **Confirmed 90-day patterns** add a second layer of confidence
- **In-and-out behavior** (1–99% OOS) is rewarded — pure 100% OOS could be dead listing
- **Demand cap at 500 monthly sold** keeps super-high-volume items from dominating
- **Low offer count is a major bonus** — when you catch the restock, you own the listing

Sort by `score DESC`, take the top 20–50, set up monitors on each.

## Triage workflow for KPF results

You ran a query. 380 ASINs came back. Now what?

1. **Bulk-export** the result list. Most KPF tooling lets you export ASINs.
2. **Bulk-scan** through SellerAmp / your scanner. Adds live Buy Box, fees, offer count snapshot, IP-risk score.
3. **Sort by ROI × velocity** (most scanners surface "estimated monthly profit").
4. **Eyeball the top 30 charts.** Look for offer-count spikes (deal pile-on signal), Amazon orange creeping back, Buy Box decay trend, **and the tiny-orange-sliver signal**.
5. **Score with the formula above** if working programmatically. Take the top 20.
6. **Set up monitors** on the survivors. See [Restock monitoring](../sourcing/restock-monitoring.md) for Tempo / Blaze setup.

> **The hardest part of KPF isn't writing the query — it's discipline in triage.** Beginners try to buy half the result list. Pros throw out 95% and act on 5%.

## What a Restock/Monitor win looks like

A real Restock/Monitor win pattern:

1. KPF surfaces an item — Amazon OOS for 8 weeks, 3P price up 3× from historical
2. You verify chart pattern (4 phases all checked)
3. You set up a monitor on the ASIN
4. 3 weeks later, Amazon restocks at \$45 (down from 3P price of \$140)
5. Your monitor pings within seconds
6. You buy 10 units at \$45 from Amazon
7. You list at \$120 (undercut 3P slightly)
8. They sell out in 4–10 days
9. Net profit: ~\$50/unit × 10 = \$500 from a single restock event

Most restocks aren't this clean. But this is the shape of the play.

## Cadence — when to run KPF

| Frequency | What you're looking for |
|---|---|
| **Daily (5–10 min)** | New restocks, fresh Amazon Deals (A2A surface) |
| **Weekly (30 min)** | Restock pattern queries — anything new where Amazon OOS pattern intensifies? |
| **Monthly (90 min)** | Category-level pattern recognition (multiple SKUs declining together = supply event) |
| **Quarterly** | Re-tune saved queries, update brand exclusion lists |

Most pro sourcers have ~10–20 saved KPF queries they cycle through. The Discord shares new ones in `#kpf-queries`.

## What KPF won't tell you

- ❌ **Where to source for restocks** — KPF surfaces the opportunity. Catching the restock is monitor infrastructure (Tempo / Blaze).
- ❌ **Brand IP risk** — KPF doesn't know that some brands aggressively file complaints. Filter brands manually.
- ❌ **Restricted/gated status** — A product might match perfectly but require ungating. KPF doesn't see that.
- ❌ **The "looks too good" filter** — If 1,000 ASINs match and they all look amazing, your filter is too loose. Tighten it.

***

Next: [The 2 KPF presets we actually use →](kpf-presets.md)

*Last updated: 2026-05-05*
