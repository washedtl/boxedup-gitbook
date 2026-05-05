# A2A — Amazon-to-Amazon (price anomaly plays)

🟡 → 🔴 — the first of the two foundational BoxedUp sourcing strategies. Buy *from* Amazon at a temporarily wrong price, sell *on* Amazon when it corrects.

## What it is

You buy an item **from Amazon** at a price that is temporarily lower than its historical norm, then **resell it on Amazon** through your seller account when the price corrects back up.

The key word is **anomaly**. You're not buying because it's cheap — you're buying because the current price represents a **statistically unusual deviation** from what the market considers the normal price for that item.

## The core logic

Keepa proves this visually: if you look at 1 year of price history and the current price is notably below the orange Amazon line's historical trend, that is the anomaly. The bet is that price will revert to mean.

If the historical norm is \$80 and Amazon is currently selling at \$32, you buy at \$32 and list at the historical norm. Once enough A2A buyers have absorbed the bug-priced inventory, Amazon's algorithm corrects and the price snaps back up. You profit on the gap.

## How Amazon randomly creates A2A opportunities

Amazon's pricing algorithm makes mistakes. It will sometimes:
- Drop a product 40–60% below its own historical retail price without warning
- This happens across 20,000+ items every day
- Windows are brief — hours to a day or two
- The price corrects back up as the algorithm recalibrates

These windows are random and unannounced. Your job is to be set up to catch them.

## The cardinal A2A rule

You're exploiting a **pricing gap**, not a supply gap. The item is available. Amazon is in stock. **The price is just temporarily wrong and will correct.**

This is the line that separates A2A from Restock/Monitor. **Never confuse them.**

## What an A2A chart looks like

When you click into a Keepa chart for a candidate, you should see:

- **Orange Amazon shading is present and mostly continuous** — Amazon has been a consistent supplier
- **The current price (right edge of chart) is visibly lower** than the 90-day, 180-day, or 365-day average
- **Both the blue New line and the orange Amazon line are depressed** below historical norms
- **No massive long white gap** — this is NOT an OOS item, Amazon is simply pricing it low right now

If the chart shows a big white gap (Amazon OOS), this is not A2A — it's a Restock/Monitor candidate. Different strategy.

Full chart-reading framework: [Reading a Keepa chart like a pro](../tools/keepa.md).

## How to surface A2A opportunities — Keepa Deals

A2A doesn't run through KPF. It runs through **Keepa Deals**.

Keepa.com → **Deals** tab. Configure:

| Setting | Value | Why |
|---|---|---|
| **Drop %** | 30% – 60% | Window where algorithm bugs typically appear |
| **Drop Interval** | 1 day / 1 week | How recent the drop has to be |
| **Price Range** | \$15 – \$300 | Avoid noise at extremes |
| **Sales Rank** | Top 1–5% of category | Velocity floor |
| **Categories** | Your domains | Limit to what you can analyze fast |

The Deals tab streams items hitting these thresholds in real time.

## The A2A buying workflow

End-to-end:

### 1. Stream Keepa Deals

Keep the Deals tab open in a browser tab during active sourcing hours. Items hitting your filter pop into the feed in real time.

### 2. Click into a candidate, year view first

Always year view, never 3-month-only. You're confirming the anomaly is genuinely unusual versus the full historical price story.

### 3. The 3-question test

For each candidate, run through:

- ☐ Is the current price meaningfully (≥30%) below the 90/180/365-day historical Amazon average?
- ☐ Is Amazon currently in stock?
- ☐ Has the price been at or near the historical norm for most of the last year?

All three yes = confirmed A2A anomaly.

### 4. ROI math

Use SAS or your scanner. Apply the [profit equation](../deal-analysis/profit-equation.md):

- Sell price = historical Amazon price (the mean it'll revert to)
- Cost = current Amazon price
- Subtract referral, FBA, inbound, returns reserve
- Need ≥ 30% ROI to commit

### 5. Buy

Speed matters. A2A windows close in hours.

**Rules at checkout:**
- ✅ NOT against Amazon's TOS for resellers
- ❌ Cannot use Prime shipping for resale purchases
- ❌ Cannot use multiple buying accounts to bypass quantity limits
- 🔁 Quantity limits reset when an item goes OOS and restocks (so check back later if you maxed your initial buy)
- 📦 Request **box packaging** at checkout, not retail packaging
- 🧾 Save the Amazon invoice — useful for ungating and beating IP complaints

### 6. Inbound to FBA

Same-day if possible. The faster your inventory is live on the listing at the elevated price, the more units you sell into the corrected-price window before competition catches up.

### 7. List and ride

Once Amazon's algorithm corrects, the listing's Buy Box snaps back to the historical norm. Your inventory rides that price up. Sell through.

## A2A cadence

- **Real-time** — Keepa Deals streams continuously when you're at your desk
- **Decision time per deal** — 60–120 seconds (chart check + ROI math)
- **Action speed** — buy within minutes; A2A windows close fast
- **Volume** — typically 1–5 buys per active hour of monitoring
- **Cash flow** — fast — A2A inventory typically clears in 2–4 weeks

## When A2A fails

- **The "anomaly" is actually a permanent price drop.** The product is being phased out and the new lower price is the new normal. There's no mean to revert to. The chart will show price stepping down repeatedly over 60–90 days, not just a single recent drop.
- **You bought before checking gating.** A2A doesn't bypass restricted categories. Verify ungated status before clicking buy.
- **Amazon's quantity limit was lower than your buy estimate.** Some windows let you buy 1, others let you buy 50. Plan accordingly.
- **The price corrects faster than your inbound.** If Amazon corrects within 2 days and your inbound takes 7, by the time your inventory is live the price might be back at the dip again because you sent supply into a corrected market.

## A2A vs Restock — quick reference

| | A2A | Restock/Monitor |
|---|---|---|
| Surface | Keepa Deals | KPF + monitor infrastructure |
| Trigger | 30–60% price drop event | Sustained OOS pattern with restock evidence |
| Amazon status when you buy | In stock | OOS, occasionally restocking |
| Buy from | Amazon | Wherever supply appears |
| Typical hold time | 2–4 weeks | 1–8 weeks (until next restock or sell-through) |
| Cadence | Real-time, hours-to-days | Set up monitors, wait days-to-weeks |

➡️ Next: [Restock/Monitor — availability scarcity plays](restock-monitor-strategy.md)

***

*Last updated: 2026-05-05*
