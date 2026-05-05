# Restock monitoring — the infrastructure layer

🔴 **Advanced.** Restock monitoring is the second half of the Restock/Monitor strategy. KPF surfaces the candidate ASINs. Monitors are how you catch the actual restock event the moment it fires.

> **The infrastructure has to be in place BEFORE the window opens.** You can't build the monitor after the restock happens. By the time you notice manually, the inventory is gone and the price is back up.

## Why monitors exist

A restock event is fast:

- Amazon restocks 50 units of a chronically-OOS SKU at \$45 (down from 3P price of \$140)
- Within 60 seconds, deal-finders' bots pick it up
- Within 5–10 minutes, the listing is OOS again
- Within 30 minutes, price has reset back up

If you're not pinged in real-time, you miss it. **Manual checking does not work for this strategy.** You need automated infrastructure that watches a list of ASINs/SKUs and pings you the moment any of them comes back in stock — at any retailer.

## The two monitor tools

The BoxedUp Discord uses two complementary monitor systems. Both run 24/7 and post into Discord.

### Tempo

The primary restock monitor. Scans Amazon, Walmart, Best Buy, Newegg, Target, B&H Photo, and a number of others.

**Command format:**
```
!m add [retailer] sku1 sku2 sku3 sku4...
```

All SKUs go on **one single line** — never multiple lines. Whitespace between SKUs.

**Supported retailers include:**
- `amazonus` — Amazon US
- `walmart` — Walmart.com
- `bestbuy` — Best Buy
- `newegg` — Newegg
- `target` — Target
- `bhphoto` — B&H Photo
- (others — check the Tempo bot's `!m help` for the current list)

**Example for an Amazon US watchlist:**
```
!m add amazonus B081XWLQKS B0C79S2CHW B07ZPLM1R1 B0C79QT9DT B09HW9886B
```

That single command sets up monitors on five RAM ASINs at Amazon. Tempo will ping the channel where you ran the command the moment any of them goes back in stock.

### Blaze

Secondary monitor with its own API and a different scraping strategy. Useful for redundancy — if Tempo misses an event due to retailer rate-limiting or scraper drift, Blaze often catches it.

Setup is API-driven (not chat-command). You'll be onboarded to it inside the Discord with the appropriate channel access.

## The standard workflow

End-to-end, from KPF query to inventory in hand:

### 1. Run the KPF Restock query

See [KPF deep dive](../tools/keepa-product-finder.md#the-restock-filter-set--filter-by-filter) for the full filter set.

### 2. Triage the results

Score and rank using the [restock-frequency scoring model](../tools/keepa-product-finder.md#a-working-restock-frequency-scoring-model). Take the top 20–50.

### 3. Manual chart verification on each survivor

For each candidate:
- Year view of Keepa chart
- Confirm 4-phase pattern (healthy → supply signal → collapse → monitor phase)
- Confirm at least one tiny-orange-sliver event in the last 30–60 days (proof of active demand absorption)
- Confirm offer count near zero
- Confirm 3P price is meaningfully elevated above historical Amazon retail

### 4. Build the Tempo command

Format all surviving ASINs into one Tempo command per retailer:

```
!m add amazonus ASIN1 ASIN2 ASIN3 ASIN4 ASIN5 ...
```

If the SKU is also worth monitoring at other retailers (Walmart, Best Buy, etc.), add a second command line per retailer.

### 5. Post to the appropriate Discord channel

Run the command in the channel where Tempo will ping you. Pin the message so you can find it later.

### 6. Wait

Monitors run 24/7. When a restock fires:
- You get pinged in the Discord channel
- The ping includes the buy URL
- You have **seconds to minutes** to act

### 7. Buy and ship

When a ping fires:
- Click the buy URL immediately
- Buy the maximum quantity Amazon allows (note: limits reset when the item goes OOS and restocks)
- Use **box packaging** at Amazon checkout, not retail packaging
- **Don't use Prime shipping for resale purchases** (against Amazon's TOS for resellers)
- Ship into FBA same day if possible
- Save the Amazon invoice — it can defend ungating and IP complaints

### 8. List

If you already have a listing on that ASIN, your inventory will go live as soon as it's received at FBA. If not, create the listing while waiting for the inbound shipment.

Price strategy on a Restock/Monitor win:
- **Match the elevated 3P price** if you want to maximize per-unit profit (but you'll sell slower)
- **Undercut by 5–10%** if you want to clear inventory faster and ride the wave
- **Watch the chart** — if Amazon comes back in stock at historical retail, undercut hard and clear out

## What "good monitor list" looks like

A healthy restock monitor list:

- **20–80 ASINs** at any given time (more than ~80 and your conviction starts to dilute)
- **Mix of price points** — some \$50–\$100 ASINs for volume, some \$200–\$500 for ticket
- **Mix of restock frequencies** — some "hot" SKUs that fire weekly, some "deep" SKUs that fire once a month with bigger margins
- **All in categories you can actually move** — no monitors on gated categories you can't list in
- **Pruned weekly** — dead monitors come off the list (no fires in 60 days, or restock pattern broken)

## Pruning — when to remove a monitor

Take an ASIN off your monitor list when:

- Amazon has been **steadily back in stock for 30+ days** (the shortage is over)
- Offer count has **recovered to 10+ FBA sellers** (saturation is back)
- 3P price has **collapsed back to historical retail** (no margin left)
- The ASIN has **fired a restock alert but the price wasn't profitable** for 3 cycles in a row
- A higher-conviction replacement comes along and you need the slot

Don't be sentimental. The monitor list is a working tool, not a wishlist.

## Common monitor mistakes

### Mistake 1 — Setting up monitors with no chart verification

KPF surfaces candidates. The chart confirms them. **Skipping the chart-verification step puts dead listings on your monitor list and dilutes your alert signal.**

### Mistake 2 — Trying to act on every ping manually

If you're pinged 50 times a day and have to manually evaluate each one, you're going to miss the real winners. **Tighter pre-filtering = fewer pings = faster action on the ones that matter.**

### Mistake 3 — Leaving monitors on saturated SKUs

A SKU that used to be a monopoly play is now monitored by 30 other resellers. Restocks get vacuumed up by everyone simultaneously. Your average win rate per ping drops to near zero.

When you see this happen — when a SKU you've been monitoring for months stops being profitable on alerts — **prune it.** Move on to the next one.

### Mistake 4 — Forgetting Amazon's quantity limits

Amazon caps how many units of a given ASIN you can buy. Limits reset when the item goes OOS and restocks. So:

- Cap = 5? Buy 5 on the first restock
- Wait for the next OOS event
- Limit resets to 5
- Buy 5 more

Across 5–10 restock events, you can accumulate substantial inventory on a high-frequency restocker.

### Mistake 5 — Using Prime for resale purchases

Don't. It's against Amazon's TOS for resellers and gets accounts flagged. Use standard shipping with box packaging.

## Free / DIY monitoring options

Before paying for monitor services, two free tactics worth knowing:

### Restock-tracker websites (Tier-0 sourcing discovery)

Public restock-tracker sites surface OOS items + restock alerts at scale. Free to use, useful as a discovery substrate before Keepa-validating:

- **NowInStock** (`nowinstock.net`) — broad retailer coverage, organized by product category
- **Trackalacker** — alerts on hot products
- **Zoolert** — restocks across major retailers
- **RestockTracker.io** — multi-retailer
- **StockInformer** — UK-leaning but covers US too
- **HotStock** — gaming/electronics-focused

Workflow:
1. Browse a category that's currently in shortage
2. Note SKUs that are showing repeated OOS-then-restock
3. Pull up the Amazon listing for each
4. Run the [KPF restock filter logic](../tools/keepa-product-finder.md) on the candidate
5. If it survives Keepa validation, add it to your Tempo / Blaze monitor list

This costs you nothing and surfaces leads you wouldn't get from a paid monitor — because nobody is monitoring these specific SKUs yet.

### Distill.io webhook recipe (for one-off retailers)

When the SKU you want to monitor isn't on a major retailer's plugin path (Tempo doesn't cover every retailer), you can DIY-monitor it via the **Distill.io** Chrome extension:

1. Install the Distill Chrome extension (`distill.io`)
2. Navigate to the product page on the retailer's site
3. Click the Distill icon → "Select an element to monitor"
4. Highlight the "Sold Out" / "Out of Stock" text on the page
5. Set check interval (e.g., 5 minutes)
6. Configure **Discord webhook URL** as the notification target
7. Save

When the page text changes from "Sold Out" → "Add to Cart" / "In Stock", Distill fires a webhook to your Discord channel. You react in seconds, just like with Tempo.

Limits:
- Distill's free tier limits how many monitors you can run simultaneously (~25)
- Doesn't include browser-session-based scrapes (so no logged-in retailers)
- Long-tail solution, not a primary tool

For BoxedUp scale: Tempo + Blaze cover the high-volume retailers; Distill fills in the gaps.

## Beyond Tempo and Blaze

If you're scaling and want redundancy beyond what the Discord ships, the major commercial monitor services are:

- **NotMyKid** — popular Discord-based restock monitor
- **Hayha** — Tempo competitor with a different scraping engine
- **Custom monitors** — for specific retailers, you can build with proxies + a scraper + a Discord webhook

Most members never need anything beyond Tempo + Blaze. Those two cover 95% of the surface.

## The bigger picture

Monitors are **the action layer** of the methodology. Without them, the methodology can't fire — you can have the best KPF queries in the world, but if you can't catch the restock the moment it happens, you can't act.

Three things compound over time:

1. **Your monitor list quality** — every pruning cycle makes it better
2. **Your reaction speed** — practice means you click the buy URL within seconds
3. **Your chart-reading speed** — you can verify a candidate in 90 seconds by month 6

That compounding is the moat. Beginners can't replicate it overnight.

***

*Last updated: 2026-05-05*
