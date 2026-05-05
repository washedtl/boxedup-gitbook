# Reading a Keepa chart like a pro

🟡 **Intermediate / 🔴 advanced.** This is the BoxedUp way of reading a Keepa chart. The chart does not lie. Learn to read it and trust it.

> **Core belief:** the Keepa chart tells the full story. Social media, news, and industry reports confirm the *why*. Discovery always starts in the data. **Keepa discovers. The news confirms. Speed is the edge.**

## What Keepa actually is

Keepa has been silently scraping Amazon every few minutes since 2010. The full database has:

- Price history for every active ASIN, going back years
- BSR (sales rank) history
- Buy Box history (who's been winning, when, at what price)
- Number of FBA / FBM / Amazon offers over time
- Review counts, ratings, listing changes
- Variation history
- Stock level estimates
- A massive **product database** queryable via Product Finder (KPF) — see [KPF deep dive](keepa-product-finder.md)

The free Keepa overlay covers single-chart reading. The **\$19/mo paid plan** is required for KPF, multi-year history, CSV exports, alerts, and API access.

**If you source seriously, get the paid plan.** Both core BoxedUp strategies — A2A and Restock/Monitor — depend on it.

## The two strategies the chart is telling you about

Every profitable Amazon flip the BoxedUp methodology produces is one of two distinct plays. **Never confuse them — the sourcing logic, buying timing, and risk profile are completely different.**

| | **A2A — pricing anomaly** | **Restock/Monitor — availability scarcity** |
|---|---|---|
| **What you exploit** | Price is temporarily wrong | Item is hard to get |
| **Amazon orange line** | Present, mostly continuous, currently *depressed* below historical norm | Has gaps; recent long white stretch (Amazon currently OOS) |
| **The bet** | Price reverts to mean | Demand exceeds supply; you catch a restock |
| **Buy from** | Amazon itself | Wherever supply appears (retailers, wholesale, restock alerts) |
| **Sell on** | Amazon (your seller account) | Amazon, at the elevated 3P price |
| **Window** | Hours to days | Weeks to months of monitoring |

### The A2A test

Ask: *"Is this profitable because the price is lower than normal, or because it's hard to get?"*

- Lower than normal → **A2A**
- Hard to get (OOS, scarce) → **Restock/Monitor**

Never conflate them.

## The three chart sections — what each tells you

When you open a Keepa chart, **always go to Year view first.** Never analyze on 3-month view without seeing full history. The full story requires the full timeline.

### Section 1 — Price history (top)

This is the primary analysis zone. You're establishing one thing: **what was "normal" price for this item?** That baseline is your reference. Everything after is deviation, and deviation is opportunity.

What you read here:

- **Where has Amazon historically priced this?** (long orange line)
- **What's the spread between Amazon and 3P prices?** (orange vs blue separation)
- **When did the price break from historical norms?** (the inflection point)
- **Are there random price drops visible?** (sudden vertical drops in the orange or blue line)
- **How wide is the white gap?** (longer white = deeper supply vacuum)

⚠️ **Do not use the "New" line for ROI math.** That's the lowest current new price, often from FBM sellers you'll never compete with. Use Buy Box, or Amazon's historical orange.

### Section 2 — BSR / Monthly Sold (middle)

This section tells you about **demand and sales velocity.**

- **Green BSR line dropping** = a sale just happened (rank improved)
- **Green BSR climbing** = item is losing relative popularity
- **Yellow-gold Monthly Sold line** = Keepa's estimate of monthly buyers (where available, ~3M+ ASINs)
- **Subcategory rank** = relative popularity within a tighter category — often more useful than top-level BSR

> **Critical: BSR disappearing does NOT mean the item stopped selling.** It means all sellers may be OOS simultaneously, so the algorithm has no current sales data to rank against. The rank reappears the instant supply does. Demand is still there. Buyers are still there.

### Section 3 — Offer count (bottom)

The **supply-chain intelligence section.** Read this as carefully as price.

The purple line = New Offer Count = number of sellers currently on the listing.

| Pattern | What it means |
|---|---|
| Offer count rising steadily | More sellers discovering — competition increasing |
| Offer count declining steadily | Sellers can't resupply — supply drying up upstream |
| Sharp sudden drop | One or more sellers sold through entire inventory |
| Decline with no bouncebacks | **Classic shortage pattern** — not temporary fluctuation |
| Flat near zero | Market is dry — 1–2 sellers remain or none |
| Spike upward after zero | New supply entered — potential restock moment |

> **The most important pattern:** sustained, one-directional decline in offer count across **multiple SKUs in the same category simultaneously.** When many different products in a subcategory all show the same decline at the same time with no bouncebacks, that's a category-level supply event. Not product-specific. **This is how the RAM shortage was identified.** See the [RAM shortage case study](the-ram-shortage-case-study.md).

## Reading velocity without a BSR

Items without a current BSR can be among the fastest-selling items on Amazon. **No sales rank does NOT mean no sales.** Five signals that work when BSR is absent or suppressed:

### Signal 1 — Offer count drops
Each drop = a seller ran out of inventory. They were selling, which means buyers were buying. Falling offer count on a "no rank" item is direct evidence of sales activity.

### Signal 2 — Offer count fluctuation patterns
Rapid up-and-down cycling (count appearing, disappearing, appearing) = high turnover. Sellers buy → list → sell out → fall off. The speed of that cycle tells you velocity.

### Signal 3 — Subcategory rank
Even when top-level BSR is suppressed, a subcategory rank may still be visible. An item ranked #5 in "DDR5 Desktop Memory" is selling extremely well regardless of what the top-level Electronics rank shows. **Always check the subcategory.**

### Signal 4 — Monthly sold data
When Keepa has it (yellow-gold line, middle section), this is the most direct demand signal available. No interpretation needed — Amazon estimates exactly how many buyers per month.

### Signal 5 — "Bought in past month" badge
Amazon displays this on product pages when purchase volume is meaningful (50+, 100+, 500+, 1000+). Pulled from real transaction data. Real and current.

> **What NOT to use:** Review count growth. For OOS / shortage items, reviews are completely unreliable — there's nothing to buy, so reviews can't accumulate. Absence of review growth on a scarce item tells you nothing about demand.

## The tiny orange sliver — the highest-conviction signal

When you see a chart with months of white (Amazon OOS) and a tiny sliver of orange appears, immediately going OOS again — **that is one of the highest-conviction demand signals in the methodology.**

Why:
- Amazon restocked (however briefly)
- That restock sold out **instantly** at whatever price Amazon set
- This confirms demand exists right now, in the current market, at current prices
- If you'd had inventory at that moment as 3P, you would have sold it

The fact that there was no time for review growth, no BSR impact, and no offer-count recovery doesn't matter. The data is telling you: **buyers are waiting. The second supply appears, it gets absorbed.**

When you see this pattern → add to the [Restock/Monitor list](../sourcing/restock-monitoring.md).

## The 6-step Keepa read

When you open a new Keepa chart, this is the exact mental process:

### Step 1 — Set the time range
Year or All view first. Never 3-month-only without seeing the full history.

### Step 2 — Read the orange (Amazon history)
- Is there orange anywhere? **No orange ever = not a restock candidate.** Required.
- Where does orange start and end? When did Amazon first stock it? When did they stop?
- Stable and flat = established supply chain. Choppy = always inconsistent.
- What price was Amazon at historically? **That's your baseline "true retail."**

### Step 3 — Read the white gaps
- Are there gaps in the orange? How long?
- Recent long white gap = Amazon has been OOS for an extended period
- Tiny orange slivers in the white = Amazon trying to restock but selling through instantly (the gold signal)

### Step 4 — Read the offer count
- Peak offer count? (more = more competitive market)
- Declining? Sustained decline with no bouncebacks = supply drying up
- Where is it now? Near-zero = almost no supply
- Sellers appearing/disappearing rapidly? = high velocity even without a rank

### Step 5 — Establish the price story
- Historical Amazon price = baseline
- Current 3P price = the shortage premium
- Multiple? (2× = moderate shortage, 4×+ = severe shortage)
- Visible price-drop events? (sudden vertical drops = algorithm resets — A2A opportunities)

### Step 6 — Make the call

Six checks:

- ☐ Historical orange present?
- ☐ Amazon currently OOS (or temporarily mispriced)?
- ☐ Offer count near zero (for restock) or stable (for A2A)?
- ☐ Demand evidence (monthly sold, offer-count drops, subcategory rank)?
- ☐ Price elevated vs historical (restock) or dipped below it (A2A)?
- ☐ Pattern consistent across the full year view?

All six check out → add to monitor list (Restock) or buy now (A2A).

## A2A — what the chart looks like and how to act on it

The A2A chart story is different from the Restock story. You're looking for:

- **Orange line is present and mostly continuous** — Amazon is a consistent supplier
- **Current price is visibly lower** than the 90-day, 180-day, or 365-day average
- **Blue New line and orange Amazon line are both depressed** below historical norms
- **No massive long white gap** — this is NOT an OOS item, Amazon is just temporarily mispricing

The cardinal A2A rule: **you're exploiting a pricing gap, not a supply gap.** The item is available. Amazon is in stock. The price is just temporarily wrong and will correct.

### Where A2A opportunities come from

Amazon's pricing algorithm makes mistakes. It will:

- Drop a product 40–60% below its own historical retail price without warning
- This happens across 20,000+ items every day
- Windows are brief — hours to a day or two
- The price corrects back up as the algorithm recalibrates

### How to surface A2A opportunities — Keepa Deals

A2A doesn't run through KPF. It runs through **Keepa Deals**.

Keepa.com → **Deals** tab. Configure:

| Setting | Value | Why |
|---|---|---|
| **Drop %** | 30% – 60% | Window where algorithm bugs typically appear |
| **Drop Interval** | 1 day / 1 week | How recent the drop has to be |
| **Price Range** | \$15 – \$300 | Avoid noise at extremes |
| **Sales Rank** | Top 1–5% of category | Velocity floor |
| **Categories** | Your domains | Limit to what you can analyze fast |

The Deals tab streams items hitting these thresholds in real time. You're betting on **mean reversion** — if the historical norm is \$80 and Amazon is currently selling at \$32, you buy at \$32 and list at the historical norm.

### A2A buying rules

- ✅ NOT against Amazon TOS
- ❌ Cannot use Prime shipping for resale purchases
- ❌ Cannot use multiple buying accounts to bypass quantity limits
- 🔁 Quantity limits reset when an item goes OOS and restocks
- 📦 Request box packaging at checkout (not retail packaging)
- 🧾 Amazon invoices can work for ungating and beating IP complaints

### A2A cadence

- **Real-time** — Keepa Deals streams continuously when you're at your desk
- **Decision time per deal** — 60–120 seconds (chart check + ROI math)
- **Action speed** — buy within minutes; A2A windows close fast
- **Volume** — typically 1–5 buys per active hour of monitoring

## Restock/Monitor — what the chart looks like

The ideal Restock chart tells a 4-phase story:

### Phase 1 — The healthy period
- Long stretch of orange shading at a stable price
- Amazon and 3P prices tracking closely
- Offer count building steadily
- Item clearly selling (BSR drops or Monthly Sold active)

### Phase 2 — The supply signal
- Offer count begins sustained, **one-directional decline**
- No bouncebacks — sellers can't replenish
- Orange shading starts showing gaps (Amazon going in and out)
- 3P prices start to separate from Amazon's price (spread grows)

### Phase 3 — The collapse
- Orange disappears entirely (Amazon goes OOS)
- Offer count reaches near-zero
- 3P prices spike 2×, 3×, 4×+ above historical Amazon retail
- Sales rank may disappear (BSR suppressed)

### Phase 4 — The monitor phase (where you live)
- Occasional tiny orange slivers → instant OOS again
- These slivers are the most valuable data: they confirm **active demand absorption**
- 3P market maintains elevated pricing because no real supply exists
- Your monitors are live, waiting for the next restock event

This is when you set up [Tempo / Blaze monitors](../sourcing/restock-monitoring.md) and wait.

### Non-negotiable: historical orange required

For Restock/Monitor, the chart MUST show orange (Amazon in stock) at some point in history. Not optional. Without historical orange:

- Can't confirm Amazon ever carried this
- Can't know if the supply-chain relationship is established
- Can't know if Amazon will ever restock

More white than orange is fine. Even a tiny sliver of orange months ago qualifies. The point: prove Amazon has had a supplier relationship with this product.

## Common chart traps

### Trap 1 — "No BSR = not selling"
**Wrong.** BSR disappears during deep shortages when all sellers are simultaneously OOS. Demand is still real. Read velocity through offer count, subcategory rank, and monthly sold instead.

### Trap 2 — "Reviews growing = selling well"
**Doesn't apply to OOS / shortage items.** When there's no inventory, there are no orders, so no reviews. Absence of review growth on a scarce item tells you nothing.

### Trap 3 — "Amazon 100% OOS over 90 days = great signal"
Could mean Amazon truly stocked it and has been gone — but **could also mean Keepa never captured an Amazon offer at all.** Use the 5–99% range in KPF to ensure Keepa has captured at least some Amazon activity. See [KPF deep dive](keepa-product-finder.md).

### Trap 4 — "High offer count = opportunity"
**Wrong direction.** High offer count usually means commoditized, low-margin, heavy competition. **Low offer count + high OOS + high demand = the real opportunity.**

### Trap 5 — "Wait for news to confirm the shortage before acting"
By the time it's news, the margin is gone. The data confirms before the news. Act on the Keepa signal.

### Trap 6 — The variation ASIN trap
You scan a UPC, get an ASIN, but the BSR shown is for the **parent ASIN** (the listing as a whole), not your specific child variation. Always click into "Variations" in the Keepa Data tab to verify.

### Trap 7 — Single-seller manipulation
One seller alone can hold the Buy Box at any price. Looks beautiful: stable, high price, decent rank. You buy in. Now there are two sellers, and the original drops 30% to keep Buy Box share. **Always check seller-count history, not just current count.**

## The Data tab — the cheat sheet

Below the chart, Keepa has a Data tab nobody reads. Should be the second thing you check.

| Field | Why it matters |
|---|---|
| Sales Rank — Current / 30/90/180-day avg | Trend direction (improving or decaying?) |
| Sales Rank drops (30/90/180) | Velocity proxy |
| Buy Box — 30/90/180-day avg | What you can model your ROI off |
| Buy Box — Lowest / Highest | Worst case / stockout-driven peaks |
| % Buy Box won by FBA / FBM / Amazon | Whether FBA can realistically compete |
| Offer count (current + 90-day high) | Competition saturation |
| Out-of-stock count (Amazon, 30/90 day) | **Restock-frequency signal — see KPF page** |
| Out-of-stock percentage (Amazon, 30/90 day) | Same — confirms the pattern |
| Variations | Other ASINs in same listing family |
| Listed since | New listings (<90 days) are unreliable |

**The 30s vs 180s rule:** compare the 30-day BSR average to the 180-day average. If 30 is *higher* (worse rank), the product is decaying. If 30 is *lower*, it's accelerating.

## Where charts end and KPF begins

Charts answer: "is this specific ASIN a buy?"

KPF answers: "give me 500 ASINs that match my criteria, and I'll filter from there."

Both are essential. Charts validate. KPF discovers.

➡️ Next: [Keepa Product Finder (KPF) — sourcing at scale](keepa-product-finder.md)

***

*Last updated: 2026-05-05*
